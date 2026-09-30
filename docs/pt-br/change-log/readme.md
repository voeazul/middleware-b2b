# Changelog

## [1.25.0] - 30/09/2026

### Adicionado
- Adicionado novo tipo de período personalizado (intervalo de datas) na extração do relatório de Pagamentos (Payment Report) na **Sales.B2B.Reports.Api**, permitindo consultas além das opções já existentes de dia, semana e mês.

  **Artefatos afetados:**
  - API: `Sales.B2B.Reports.Api`
    - Método: `POST /api/v1/orders/reports/payments`

- Disponibilizada nova versão (V2) dos métodos de cadastro e atualização do contato de IROP na **Sales.B2B.Order.Api**, **Order.Management.Api** e **Organizations.Api**.

### Modificado
- Ajustado o relatório de Reacomodação (Reaccommodation Report) na **Sales.B2B.Reports.Api** para não considerar mais reservas de GDS e de Grupos, retornando apenas reservas do contexto B2B.

  **Artefatos afetados:**
  - API: `Sales.B2B.Reports.Api`

- Corrigido o retorno dos valores monetários do relatório de Vendas (Sales Report) na **Sales.B2B.Reports.Api**, que estavam sendo exibidos sem a casa decimal correta; incluídos os campos de código e nome da organização e reorganizada a ordem de exibição dos campos.

  **Artefatos afetados:**
  - API: `Sales.B2B.Reports.Api`

- Corrigida a busca do relatório de Segmentos (Segment Report) na **Sales.B2B.Reports.Api** para considerar todos os agentes da agência solicitante, e não apenas o agente que gerou a solicitação; incluído o campo de data de criação da reserva e reorganizada a ordem de exibição dos campos.

  **Artefatos afetados:**
  - API: `Sales.B2B.Reports.Api`

- Alterada a permissão de consulta de organizações na **Sales.B2B.Organizations.Api**, permitindo que integrações internas consultem os dados de uma organização sem a exigência de vínculo com um grupo comercial.

  **Artefatos afetados:**
  - API: `Sales.B2B.Organizations.Api`
    - Método: `GET api/private/v1/organizations/{organizationCode}`

- Corrigido o retorno da verificação de alteração de nome de passageiro na **Sales.B2B.Order.Passengers.Api**, passando a indicar corretamente quais passageiros já tiveram o nome alterado em reservas com múltiplos viajantes.

  **Artefatos afetados:**
  - API: `Sales.B2B.Order.Passengers.Api`
    - Método: `PATCH api/v1/order/{recordLocator}/passengers/{passengerKey}/name`
    - Método: `PATCH api/v1/order/{recordLocator}/passengers/name/confirm`

- Excluídas da busca de reservas (SearchBy) da **Sales.B2B.Order.Management.Api** as reservas criadas pelo Portal Grupos, mantendo no resultado apenas reservas do contexto B2B.

  **Artefatos afetados:**
  - API: `Sales.B2B.Order.Management.Api`
    - Método: `SearchBy`

- Tornado obrigatório o preenchimento do contato de IROP (IropContact) na **Sales.B2B.Order.Api**, com o telefone passando a ser informado em três campos separados (DDI, DDD e número).

  **Artefatos afetados:**
  - API: `Sales.B2B.Order.Passengers.Api`
    - Método: `PUT api/v1/order/{recordLocator}/passengers/{passengerKey}`
  - API: `Sales.B2B.Order.Management.Api`
    - Método: `PATCH api/v1/order/{recordLocator}/contact`
  - API: `Sales.B2B.Organizations.Api`
    - Método: `POST api/v1/organizations/{organizationCode}/users`
    - Método: `POST api/v1/organizations/parent/{organizationCode}`

- Adicionada validação de passageiro indisciplinado na **Sales.B2B.Order.Api** e **Sales.B2B.Order.Management.Api**, impedindo a confirmação via checkout de reservas que contenham esse tipo de passageiro. Para passageiros de nacionalidade **BR**, será obrigatório informar o documento do tipo **CPF**. A validação é independente dos bloqueios existentes para o BPE e será aplicada exclusivamente a voos 100% domésticos. Voos internacionais ou itinerários com conexão internacional não estarão sujeitos a essa validação.
- Ajustadas as validações de documentos na criação de reservas: removida a trava de obrigatoriedade vinculada à BPe, mantendo-se apenas a validação de documento de viagem prevista na Resolução 800, conforme a nacionalidade do passageiro. A validação do GovId do contato também foi alterada, passando a verificar apenas se o campo foi preenchido, independentemente de país ou nacionalidade, com verificação automática de formato de CPF (11 caracteres) ou CNPJ (14 caracteres) quando aplicável.

  **Artefatos afetados:**
  - API: `Sales.B2B.Order.Api`
    - Método: `POST /sales/b2b/order/api/v1/order`

- Alterada a validação de nacionalidade do documento de viagem do passageiro, substituindo o campo `issuingCountry` por `birthCountry`, refletindo corretamente que a informação representa o país de nascimento do passageiro.

  **Artefatos afetados:**
  - API: `Sales.B2B.Order.Passengers.Api`
    - Método: `PUT /api/v1/order/{recordLocator}/passengers/{passengerKey}`
    - Método: `PATCH /api/v1/order/{recordLocator}/passengers/:passengerKey`
  - API: `Sales.B2B.Order.Payments.Api`
    - Método: `POST /api/v1/order/payments`

- Removida a validação de nacionalidade baseada no campo `country` do endereço do contato do tipo Customer na criação de reservas, mantendo apenas a obrigatoriedade de preenchimento do GovId.

  **Artefatos afetados:**
  - API: `Sales.B2B.Order.Payments.Api`
    - Método: `POST /api/v1/order/payments`

- Removida a obrigatoriedade de CPF para passageiros estrangeiros residentes no Brasil, permitindo o cadastro do contato Customer com documentos válidos de origem; passageiros brasileiros continuam seguindo as regras atuais. Ampliados também os campos aceitos na atualização do contato Customer, incluindo nome da empresa e endereço completo (linha 1, linha 2, estado, cidade e CEP).

  **Artefatos afetados:**
  - API: `Sales.B2B.Order.Management.Api`
    - Método: `POST /api/v1/order/{recordLocator}/contact/customer`
    - Método: `PATCH /api/v1/order/{recordLocator}/contact`
 
[Link para as versões anteriores](/docs/pt-br/change-log/readme.history.md)

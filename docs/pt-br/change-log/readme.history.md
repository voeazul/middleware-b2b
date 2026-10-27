# Changelog Completo

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

## [1.24.0] - 10/09/2026
 
### Modificado
- Atualização dos serviços para arquitetura REST.
- Atualização na resposta do método ***POST Authenticate*** trazendo mais informações do agente.

## [1.23.0] - 11/08/2026
 
### Adicionado
- Adicionado o metodo _PATCH Passenger_ para permitir ajuste de dados de passageiro, garantindo o mecanismo para atualização dos documentos do viajante na **Sales.B2B.Order.Passengers.Api**.
- Adicionado o metodo _POST Contact_ para permitir o cadastro e regularização das informações obrigatórias do contato quando a reserva não possuir um contato do tipo _Customer_ na **Order.Management.Api**.

### Modificado
- Alteração e bloqueio para pagamento de reserva sem travelDocuments conforme nacionalidade do viajante.
- Alteração no fluxo de criação de reservas, incluindo novo campo "GOVID" e validação de nacionalidade na **Order.Api**. 
  Caso o govId não seja informado, será retornado um warning, sem impactar a criação da reserva. A notificação permanecerá ativa até a aplicação do bloqueio definitivo, após o prazo estabelecido pela área de negócios da Azul.
- Alteração no fluxo de alteração de contato de uma reserva, incluindo novo campo "GOVID" e validação de nacionalidade na **Order.Management.Api**.

## [1.22.0] - 29/07/2026
 
### Modificado
- Alteração na validação de status de reserva.
- Alteração no fluxo de attach para pré-preenchimento automático dos dados do viajante na **Order.Api**.
- Alteração no retorno de informação de login bloqueado na **Organizations.Api**.
- Alteração no retorno do comentário de uma reserva na **Order.Management.Api**.
- Atualização na busca de _installments_.

## [1.21.0] - 31/05/2026

### Modificado
- Atualização para integrar com a versão _4.8_ da Navitaire.

## [1.20.0] - 26/03/2026
 
### Adicionado
- Adicionados métodos para troca de pagamento total e parcial na **Payments.API**.
- Adicionado um objeto **remarks** ao endpoint Retrieve _V3_, retornando comentários relevantes.

## [1.19.0] - 26/02/2026

### Modificado

- Implementado o tratamento de caracteres especiais no campo 'holderName' da API de pagamentos.
- Incluída a propriedade 'Customer' no checkout de reservas, assegurando que o e-mail com o itinerário seja enviado exclusivamente ao passageiro.
- Implementada a validação de CPF válido.
- Ajustada a regra de negócio para não aplicar DU em reservas internacionais de grupos pertencentes ao grupo DUI.
- Implementada validação para bloquear a alteração de promocode para um promocode já aplicados à reserva.

## [1.18.0] - 13/11/2025

### Adicionado
- Adição de método para remoção de Promotion Code durante a criação.
- Adição de método para remoção de Promotion Code para reservas em Hold.
- Adição de documento de viagem RE para uso exclusivo da Azul na emissão de reservas.
- Adição de documento de viagem RE para uso exclusivo da Azul na alteração de dados de passageiro.

### Modificado
- Retorno de total de bagagens para os novos tiers Diamante Unique e Azul One.
- Restrição de emissão de reservas CodeShare (G3) por IATA.
- Restrição de adição de trecho CodeShare (G3) por IATA bloqueado.
- Restrição de busca de voos CodeShare (G3) por IATA bloqueado.

## [1.17.0] - 29/09/2025

### Adicionado
- Adição do método para alteração do promotion code de uma reserva em Hold.
- Adicionado campo para envio de itinerários da reserva (Agency, All e None).
- Adicionado campo para envio de comentários na reserva.
- Adicionado método para atualizar dados dos contatos de Agency e Customer de uma reserva em Hold.
- Adicionado método para retornar as rotas válidas.

### Modificado
- Melhoria na mensagem de erro caso ocorra indisponibilidade da API de Installments.
- A 'OrganizationFeeOverride' está desabilitada, o valor enviado não irá sobrescrever a OrganizationFee durante a criação da reserva.
- Liberado a opção de solicitação de reembolso via CreditShell de reservas em reacomodação.
- Adicionado relatório de Reacomodação na ApI de Reportes.
- Bloqueio na busca, criação e alteração de reservas codeshare(G3) com mais de 4 passageiros.
- Melhorias nas validações e indisponibilidade da api de parcelamento.
- Removido método de alteração de DU de reservas internacionais.
- Adicionado a opção de geração de relatórios por mês para relatórios de Pagamentos e Segmentos.

## [1.16.1] -20/08/2025

### Modificado
- Restrição de Passageiros na Alteração de Reservas Codeshare.
- Restrição de Passageiros na Busca de Voos Codeshare.
- Restrição de Passageiros na Emissão de Reservas Codeshare.
- Melhoria nas mensagens de erro retornados na api de parcelamento.

## [1.16.0] - 12/06/2025

### Modificado
- Adição de serviço de UMNR opcional voos internacionais.
- Aplicação de Promocodes em voos Codeshare.
- Alteração do prazo de Hold para pagamentos declinados.
- Ajuste framework de sessão perfis de acesso.

## [1.15.1] - 03/06/2025

### Modificado
- Novo Codeshare HiFly (5K).

## [1.15.0] - 28/02/2025

### Adicionado
- Criação de método para adição de promotionCode na reserva em criação.

### Modificado


## [1.14.0] - 28/02/2025

### Adicionado
- Autorização de pagamento do tipo Credit File (CF) utilizando um crédito de outra reserva.

### Modificado
- Atualização da versão do framework para .NET 8.
- Atualização das tarifas de cancelamento, alteração e No-Show no método FARES.
- Atualização de novos trechos com restrição de bagagem: CUR/MDZ/BRC.

## [1.13.0] - 21/01/2025

### Adicionado
- Apresentação da Taxa de YQ de forma separada.
- Criação de método para alteração de dados PAX.
- Novo Codeshare EuroAtlantic (YU).

### Modificado
- Tratamento de case inSensitive no Localizador das rotas
- Melhoria de performance geral de pagamentos
- Melhoria no retorno do método get organization
- Contatos de Reserva - Capturar dados do Usuário logado e atualizar os campos E-mail e Telefone

## [1.12.0] - 09/12/2024

### Adicionado
- Adicionado campo overrideDuFee no array de passenger acima do campo nationality.
- Novo método para realizar override da DU em reserva internacional.
- Adicionado campo adjusted no array de passenger acima do name.
- Adicionado nova mensagem de erro para transferencia de sessão.
- Adicionado campo promotionCode no método FromAttach.
- Adicionado tipo de documento Mercosul nos métodos de criação de reserva.
- Adicionado campo notifyContacts nos métodos de checkout Order V1 e Order.Management V2.

### Modificado
- Foi modificado o método que aplica a DU, para considerar a nova operação para DUI aplicando no máximo 7% do valor para cada passageiro.
- Foi modificado o método de busca de reserva, para validar se a reserva está em reacomodação.
- Foi modificado o método de criação de reserva, será obrigatório a inserção do documento somente se for selecionado o Type ou a moeda da agência for BRL.
- Foi modificado o método de checkout de grupos, para permitir o pagamento parcial e sem limite de quantidade de pagamento.
- Foi modificado os métodos de checkout, para permitir o checkout de reservas em bébito, desde que seja feito o pagamento mínimo.

## [1.11.0] - 21/10/2024

### Modificado
- Aumento no timeout das Apis.
- Limpeza do state após a divisão da reserva.
- Validação de caracteres especiais para os campos "first", "middle" e "last" na criação e modificação da reserva.

## [1.10.0] - 13/08/2024

### Adicionado
- Adicionado métodos para consulta e checkout de reservas de grupos.
- Adicionado novas mensagens de erro para cartões bloqueados.

### Modificado
- Ajuste na ordenação do AirSearch para voos com escala e conexão.
- Permissão para acesso a funcionalidade de relatórios aos agentes do perfil FinancialAgent.

[Link para as versões anteriores](/docs/pt-br/change-log/readme.history.md)

## [1.9.0] - 16/07/2024

### Adicionado
- Fluxo de remoção do promocode TAIC10 caso o pagamento com o cartão Tudo Azul deja declinado.
- Método para adicionar promocode em reservas em hold já criadas.

### Modificado
- Permissão para acesso aos métodos de relatórios aos agentes do perfil WebServiceAgent.
- Disponibilização da informação da data de importação ao consultar reacomodação.
- Indicação de que a reserva encontra-se em quarentena de pagamento nos métodos de consulta.
- Indicação do valor da multa de reembolso (RefundFeeAmount) a ser aplicada no método Calculate v2.

## [1.8.0] - 28/06/2024

### Adicionado
- Informação de localizadores de reservas CodeShare

### Modificado
- Ajustes e restrições na disponibilização de bagagens e serviços em trechos CodeShare
- Impedir menor desacompanhado em reservas CodeShare
- Bloquear emissão de reservas CodeShare com trechos com data de partida a menos de 24 horas

## [1.7.0] - 17/06/2024

### Adicionado
- Nova opção de reembolso do pagamento ao realizar o _checkout_ da reserva
- Disponibilizar informações de crédito disponível para uma organização sem a necessidade de consultar uma reserva anteriormente
- Adicionadas tarifas "No Show" no método de consulta de _fares_
- Retorno da informação do tipo de cabine ao realizar o AirSerch, Quote e na consulta de reservas

### Modificado
- Ajuste no desconto do cartão Tudo Azul, agora o desconto é aplicado apenas para pagamentos integrais das reservas
- Retornar identificação do cartão consultado no método de pagamento e de consulta de parcelamento
- Retorno de informações da data de vencimento e o nome do titular do cartão no objeto de pagamentos ao consultar reservas 

### Corrigido
- Erro ao informar um documento do tipo passaporte para infant na criação de reservas

## [1.6.1] - 16/05/2024

### Adicionado
- Novo método para consulta de lowfares

## [1.6.0] - 25/04/2024

### Adicionado
- Novo método para consulta de localizadores filho
- Exibir descontos promocionais aplicados nos objetos de charges

### Corrigido
- Paginações dos sumários de reacomodações
- Ajuste no mapeamento dos telefones das agências no contato da reserva gerada

## [1.5.0] - 27/02/2024

### Adicionado
- Shopping
    - Correção do campo "productClass" no método Offer Quote
- Payments
    - Remoção do GovId como campo obrigatório nos pagamentos com cartão na moeda BRL
    - Ajuste na regra de juros
- Reaccommodations
    - Novas filas de mudanças mapeadas
- Keep Alive
    - Novas mensagens de erro
    - Cálculo do tempo de keep alive dinâmico de acordo com o iddleTimeout da Navitaire

## [1.4.0] - 31/01/2024

### Adicionado
- Pagamentos com Juros
- Melhorias de fluxos
    - Divisão
        - Hold
        - Cancelamento
    - Desconto Itaucard 
        - Incluindo desconto sobre taxa combustível
    - Performance do fluxo de autenticação
    - Categorização TudoAzul
        - Correção de nomes com namematch
    - Tratativa de mensagens de erros
        - Tarifa esgotada
        - Account de Agencia bloqueada
    - Corereção de Calculo de Hold
    - Ajuste Regex de Senhas
    - Assentos Economy Prime
    - Documentações das APIs

## [1.3.0] - 04/01/2024

### Adicionado

- Disponibilização das funcionalidades de reacomodação

## [1.2.0] - 26/12/2023

### Adicionado

- Disponibilização das funcionalidades de relatórios
	- Relatório de pagamentos
	- Relatório de vendas
	- Relatório de segmentos

## [1.1.0] - 16/11/2023

### Adicionado

- Disponibilização das funcionalidades de gestão de passageiros
	- Adição de infant em reservas já criadas
	- Categorização de Tudo Azul em reservas já criadas	

- Disponibilização das funcionalidades de venda assíncrona de ancillaries

- Melhorias gerais no mapa de assentos
	- Retorno do SkySofa
	- Informação de saída de emergência

- Melhorias gerais nos fluxos de change e cancel
	- Bloquear busca do state com calculate pendente
	- Bloquear ajuste manual de DU com calculate pendente
	- Bloquear divisão de reservas com alteração de trechos
	
- Melhorias no gerenciamento de agentes
	- Busca de usuários
	- Informações extras no retorno da autenticação

## [1.0.1] - 28/09/2023

### Modificado

- Melhorias gerais na API de Loyalty
	- Nova API Comarch

## [1.0.0] - 01/08/2023

### Adicionado

- Disponibilização da versão inicial do barramento em produção

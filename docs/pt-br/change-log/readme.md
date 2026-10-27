# Changelog

## [1.26.0] - 11/11/2026

### Adicionado
- Adicionado o método _GET InstallmentsCalculate_ (V1) na **Sales.B2B.Order.Payments.Api**, permitindo simular as condições de parcelamento sem a necessidade de uma reserva previamente criada (Order em State), utilizando apenas os dados informados na requisição (valor, taxas e, opcionalmente, BIN do cartão e mercado doméstico/internacional). Quando o BIN é informado, é retornado o parcelamento correspondente ao cartão; quando BIN e mercado não são informados, são retornadas as quatro opções de parcelamento (Azul e Regular, doméstico e internacional). Os valores retornados representam uma estimativa prévia e podem sofrer alterações após a criação e validação da reserva; para os valores definitivos, deve ser utilizado o método _GET Installments_, que permanece disponível sem alterações. Para moedas diferentes de BRL, não são apresentadas opções de parcelamento.

  **Artefatos afetados:**
  - API: `Sales.B2B.Order.Payments.Api`
    - Método: `GET /api/v1/order/payments/installmentscalculate`

- Adicionado método para alteração dos dados do passageiro Infant na **Sales.B2B.Order.Passengers.Api**, estendendo ao Infant as alterações já permitidas para passageiros adultos e crianças. A alteração contempla nacionalidade, gênero, data de nascimento e documentos de viagem do Infant.

  **Artefatos afetados:**
  - API: `Sales.B2B.Order.Passengers.Api`
    - Método: `PATCH /api/v1/order/{recordLocator}/passengers/{Key}/infant`

- Adicionado o critério de pesquisa _OrganizationGroup_ na busca de reservas da **Sales.B2B.Order.Management.Api**, permitindo pesquisar reservas considerando um grupo organizacional. Também foi corrigido o envio das informações de organização e agente nas consultas à Navitaire, garantindo que a pesquisa seja executada no contexto da organização consultada, e removida a obrigatoriedade do campo _FirstName_. Os critérios de pesquisa já existentes permanecem inalterados.

  **Artefatos afetados:**
  - API: `Sales.B2B.Order.Management.Api`
    - Método: `GET /api/v1/orders/searchBy/:type`

### Modificado
- Corrigida a consulta de créditos organizacionais na **Sales.B2B.Order.Payments.Api**, que era interrompida quando a reserva possuía um tipo de documento não mapeado pelo Barramento B2B. Essas reservas passam a ser processadas normalmente, seguindo o mesmo comportamento já adotado na **Sales.B2B.Order.Management.Api**; documentos já mapeados continuam sendo processados sem alteração.

  **Artefatos afetados:**
  - API: `Sales.B2B.Order.Payments.Api`
    - Método: `GET /api/v1/order/payments/credits/:type`

- Corrigida a divergência nas informações de reacomodação retornadas pelos métodos _Get Summary_ e _Get Summary Details_ na **Sales.B2B.Order.Reaccommodation.Api**, garantindo que os totalizadores sejam consistentes com os detalhes e que os segmentos efetivamente alterados sejam retornados como reacomodados.

  **Artefatos afetados:**
  - API: `Sales.B2B.Order.Reaccommodation.Api`
    - Método: `GET /api/v1/orders/reaccommodations/summary`
    - Método: `GET /api/v1/orders/reaccommodations/summary/Details`

- Incluído o UserAgent da requisição no comentário registrado automaticamente na criação de reservas pela **Sales.B2B.Order.Api**, permitindo identificar o canal, aplicação ou integração responsável pela criação da reserva. Quando o UserAgent não for enviado, o comentário registra "Não informado", sem impacto na criação da reserva.

  **Artefatos afetados:**
  - API: `Sales.B2B.Order.Api`

- Atualizada a documentação do campo _MethodCode_ na **Sales.B2B.Order.Payments.Api** e do atributo _methodCode_ na **Sales.B2B.Order.Management.Api**, detalhando o significado de cada código de forma de pagamento: AG (Faturado), CF (Crédito de Reserva), AX (American Express), VI (Visa), MC (MasterCard), DI (Diners Club), HP (Hipercard) e EL (Elo). Alteração apenas documental, sem impacto funcional.

  **Artefatos afetados:**
  - API: `Sales.B2B.Order.Payments.Api`
  - API: `Sales.B2B.Order.Management.Api`

[Link para as versões anteriores](/docs/pt-br/change-log/readme.history.md)

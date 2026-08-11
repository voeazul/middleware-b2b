# Changelog

## [1.23.0] - 11/08/2026
 
### Adicionado
- Adicionado o metodo _PATCH Passenger_ para permitir ajuste de dados de passageiro, garantindo o mecanismo para atualização dos documentos do viajante na **Sales.B2B.Order.Passengers.Api**.
- Adicionado o metodo _POST Contact_ para permitir o cadastro e regularização das informações obrigatórias do contato quando a reserva não possuir um contato do tipo _Customer_ na **Order.Management.Api**.

### Modificado
- Alteração e bloqueio para pagamento de reserva sem travelDocuments conforme nacionalidade do viajante.
- Alteração no fluxo de criação de reservas, incluindo novo campo "GOVID" e validação de nacionalidade na **Order.Api**. 
  Caso o govId não seja informado, será retornado um warning, sem impactar a criação da reserva. A notificação permanecerá ativa até a aplicação do bloqueio definitivo, após o prazo estabelecido pela área de negócios da Azul.
- Alteração no fluxo de alteração de contato de uma reserva, incluindo novo campo "GOVID" e validação de nacionalidade na **Order.Management.Api**.
 
[Link para as versões anteriores](/docs/pt-br/change-log/readme.history.md)
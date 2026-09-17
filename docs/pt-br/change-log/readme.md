# Changelog

## [1.25.0] - 30/09/2026

### Adicionado
- Adicionado novo tipo de período personalizado (intervalo de datas) na extração do relatório de Pagamentos (Payment Report) na **Sales.B2B.Reports.Api**, permitindo consultas além das opções já existentes de dia, semana e mês.
- Disponibilizada nova versão (V2) dos métodos de cadastro e atualização do contato de IROP na **Sales.B2B.Order.Api**, **Order.Management.Api** e **Organizations.Api**.

### Modificado
- Ajustado o relatório de Reacomodação (Reaccommodation Report) na **Sales.B2B.Reports.Api** para não considerar mais reservas de GDS e de Grupos, retornando apenas reservas do contexto B2B.
- Corrigido o retorno dos valores monetários do relatório de Vendas (Sales Report) na **Sales.B2B.Reports.Api**, que estavam sendo exibidos sem a casa decimal correta; incluídos os campos de código e nome da organização e reorganizada a ordem de exibição dos campos.
- Corrigida a busca do relatório de Segmentos (Segment Report) na **Sales.B2B.Reports.Api** para considerar todos os agentes da agência solicitante, e não apenas o agente que gerou a solicitação; incluído o campo de data de criação da reserva e reorganizada a ordem de exibição dos campos.
- Alterada a permissão de consulta de organizações na **Sales.B2B.Organizations.Api**, permitindo que integrações internas consultem os dados de uma organização sem a exigência de vínculo com um grupo comercial.
- Corrigido o retorno da verificação de alteração de nome de passageiro na **Sales.B2B.Order.Passengers.Api**, passando a indicar corretamente quais passageiros já tiveram o nome alterado em reservas com múltiplos viajantes.
- Excluídas da busca de reservas (SearchBy) da **Sales.B2B.Order.Management.Api** as reservas criadas pelo Portal Grupos, mantendo no resultado apenas reservas do contexto B2B.
- Tornado obrigatório o preenchimento do contato de IROP (IropContact) na **Sales.B2B.Order.Api**, com o telefone passando a ser informado em três campos separados (DDI, DDD e número).
- Adicionada validação de passageiro indisciplinado na **Sales.B2B.Order.Api** e **Sales.B2B.Order.Management.Api**, impedindo a confirmação via checkout de reservas que contenham esse tipo de passageiro. Para passageiros de nacionalidade **BR**, será obrigatório informar o documento do tipo **CPF**. A validação é independente dos bloqueios existentes para o BPE e será aplicada exclusivamente a voos 100% domésticos. Voos internacionais ou itinerários com conexão internacional não estarão sujeitos a essa validação.
 
[Link para as versões anteriores](/docs/pt-br/change-log/readme.history.md)
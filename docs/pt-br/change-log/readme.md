# Changelog

## [1.17.0] - 06/08/2025

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

[Link para as versões anteriores](/docs/pt-br/change-log/readme.history.md)
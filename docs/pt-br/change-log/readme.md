# Changelog

## [1.12.0] - 24/09/2024

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

[Link para as versões anteriores](/docs/pt-br/change-log/readme.history.md)
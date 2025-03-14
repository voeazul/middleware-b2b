# Changelog Completo

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

# Changelog Completo

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

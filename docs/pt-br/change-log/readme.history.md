# Changelog Completo

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

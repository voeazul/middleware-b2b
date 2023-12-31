# Documentação das APIs e Fluxo de Reserva

Bem-vindo à documentação centralizada das APIs do barramento e ao guia de fluxo de reserva! Aqui você encontrará informações sobre as APIs disponíveis e como realizar fluxos de reserva, alteração e outros principais.

## Sumário das APIs

Aqui está a lista das APIs disponíveis e uma breve descrição das APIs disponíveis:

| API   | Descrição                                         |
|-------|---------------------------------------------------|
| [Authentication](https://apim-stg-us-general.developer.azure-api.net/api-details#api=Sales.B2B.Authentication.Api) | O serviço de Authentication é responsável por autenticar o usuário sistêmico do Middleware B2B. A obtenção do token através do serviço de Authentication é obrigatória no início de cada sessão do Middleware B2B. |
| [User](https://apim-stg-us-general.developer.azure-api.net/api-details#api=Sales.B2B.User.Api) | O serviço de User é responsável por gerenciar as informações do agente de viagens logado no Middleware B2B. |
| [Shopping](https://apim-stg-us-general.developer.azure-api.net/api-details#api=Sales.B2B.Shopping.Api) | O serviço de Shopping é responsável por disponibilizar métodos de pesquisa de ofertas de voos através do Middleware B2B e fornecer toda a informação relativa às ofertas disponíveis. |
| [Organization](https://apim-stg-us-general.developer.azure-api.net/api-details#api=Sales.B2B.Organizations.Api) | O serviço de Organizations é responsável por fornecer informações relevantes às agências (organizações) que utilizam o Middleware B2B. |
| [Order](https://apim-stg-us-general.developer.azure-api.net/api-details#api=Sales.B2B.Order.Api) | O serviço de Order disponibiliza os métodos responsáveis ​​pela criação, consulta e gerenciamento de reservas realizadas através do Middleware B2B. |
| [Order Management](https://apim-stg-us-general.developer.azure-api.net/api-details#api=Sales.B2B.Order.Management.Api) | O serviço OrderManagement é responsável por fornecer métodos via Middleware B2B para gerenciar recursos de reservas. |
| [Order Seats](https://apim-stg-us-general.developer.azure-api.net/api-details#api=Sales.B2B.Order.Seats.Api) | O serviço OrderSeats é responsável por fornecer métodos via Middleware B2B para gerenciar recursos de mapas de assentos. |
| [Order Services](https://apim-stg-us-general.developer.azure-api.net/api-details#api=Sales.B2B.Order.Services.Api) | Este serviço oferece métodos que atendem solicitações de serviços especiais, malas e assistências. |
| [Order Payments](https://apim-stg-us-general.developer.azure-api.net/api-details#api=Sales.B2B.Order.Payments.Api) | O serviço OrderPayments é responsável por adicionar, consultar e gerir todos os pagamentos relativos a reservas efetuadas através do Middleware B2B. |
| [Resources](https://apim-stg-us-general.developer.azure-api.net/api-details#api=Sales.B2B.Resources.Api) | O serviço de Resources é responsável por disponibilizar os diversos tipos de recursos que serão utilizados no Middleware B2B. |
| [Reports](https://apim-stg-us-general.developer.azure-api.net/api-details#api=Sales.B2B.Reports.Api) | O serviço Reports é responsável por fornecer relatórios através do Middleware B2B. |

## Como Fazer um Fluxo de Reserva

Para obter informações detalhadas sobre os fluxos de reserva, quais APIs chamar para alteração, criação e manipulação da reserva, consulte alguns exemplos de fluxo do nosso postman na seção [Fluxos Básicos](/postman/middleware_b2b-release_1.2.5.postman_collection.json).

## Lista de Códigos de Erros da API

Se você encontrar algum erro ao utilizar as APIs, consulte a [Lista de Códigos de Erros da API](/docs/pt-br/apis-doc/errors-code.md) para obter informações sobre os códigos de erro, códigos de resposta HTTP e mensagens de erro correspondentes.

---

Explore os tópicos acima para obter mais informações sobre as APIs e os fluxos de reserva. Em caso de dúvidas ou sugestões, não hesite em entrar em contato conosco!

Happy coding! 😊

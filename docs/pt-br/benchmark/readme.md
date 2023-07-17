# Tempo de Resposta das APIs

Nesta seção, apresentamos o benchmark de tempo de resposta esperado e a variação limite para as principais APIs do barramento, tanto no ambiente de homologação quanto no ambiente de produção. Essas informações são úteis para entender o desempenho esperado das APIs e garantir uma melhor experiência para os usuários.

## Ambiente de Homologação

A tabela a seguir mostra o benchmark de tempo de resposta esperado e a variação limite para as principais APIs no ambiente de homologação:

| API                   | Tempo de Resposta Esperado (ms) | Variação Limite (ms) |
|-----------------------|--------------------------------|----------------------|
| `authentication/api/v1/token`      | 30                             | ±10                   |
| `user/api/v1/authenticate`      | 800                             | ±100                  |
| `shopping/api/v1/airsearch`      | 930                             | ±300                  |
| `order/api/v1/order`      | 300                            | ±100                   |
| `order/api/v1/checkout`      | 300                             | ±100                 |
| `order/payments/api/v1/payments`      | 800                             | ±200                   |

## Ambiente de Produção

A tabela a seguir mostra o benchmark de tempo de resposta esperado e a variação limite para as principais APIs no ambiente de produção:

| API                   | Tempo de Resposta Esperado (ms) | Variação Limite (ms) |
|-----------------------|--------------------------------|----------------------|
| `authentication/api/v1/token`      | 30                             | ±10                  |
| `user/api/v1/authenticate`      | 160                             | ±40                  |
| `shopping/api/v1/airsearch`      | 500                             | ±300                  |
| `order/api/v1/order`      | 300                            | ±100                   |
| `order/api/v1/checkout`      | 300                             | ±100                 |
| `order/payments/api/v1/payments`      | 500                            | ±100                   |

Essas informações são fornecidas como uma referência aproximada e podem variar dependendo de fatores como aumento de carga inesperado, conectividade de rede entre outras influencias externas. Mantemos uma monitoração regular no desempenho a fim de tomar ações quando necessário.
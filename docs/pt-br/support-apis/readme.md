# Suporte ao Versionamento de APIs

## Visão Geral
Nosso barramento oferece suporte ao versionamento para garantir a compatibilidade com versões anteriores e permitir a evolução da API de forma controlada. Nesta documentação, forneceremos informações sobre como lidamos com o versionamento das APIs, até quando mantemos suporte para versões anteriores e como notificamos os usuários sobre atualizações e mudanças.

## Versionamento de Rotas
Para garantir a estabilidade e a compatibilidade das APIs, seguimos um esquema de versionamento de rotas. Cada rota da API é versionada utilizando o número de versão como parte da URI.

- Exemplo de versão de rota: `/api/v1/endpoint`

O número de versão na rota indica a versão específica daquela rota. À medida que a API é atualizada e novas versões de rotas são introduzidas, o número de versão na rota pode ser incrementado.

## Mudanças no Número de Versão da Rota
O número de versão em uma rota pode mudar nas seguintes ocasiões:

1. **Alterações Incompatíveis**: Quando são feitas mudanças que não são compatíveis com a versão anterior da rota. Isso pode incluir alterações significativas na estrutura da resposta, nos parâmetros obrigatórios ou opcionais, ou na lógica subjacente. Essas mudanças podem afetar a integração da rota com a versão anterior e exigir atualizações no lado do cliente.

2. **Adição de Funcionalidades**: Quando são adicionadas novas funcionalidades à rota sem alterar a compatibilidade com a versão anterior. Isso geralmente inclui a introdução de novos parâmetros opcionais, respostas adicionais ou funcionalidades extras que não afetam a lógica existente da rota. Os clientes que desejarem usar essas novas funcionalidades podem atualizar para a versão mais recente da rota.

3. **Correções de Bugs**: Quando são realizadas correções de bugs na rota, sem alterar a funcionalidade principal ou a compatibilidade com a versão anterior. Essas correções são destinadas a resolver problemas específicos e não requerem alterações no lado do cliente.

## Suporte a Versões Anteriores
Garantimos suporte para versões anteriores por um período determinado, permitindo que os usuários façam a transição para as versões mais recentes. A duração do suporte para uma versão específica pode variar, mas em geral, seguimos a política de manter o suporte por __6 meses__:

## APIs Com Novas Versões
| API                   | Versão | Data Limite de Suporte |
|-----------------------|--------|-----------------------|
| `/api/v1/endpoint`    | 1.0    | 31 de Dezembro de 2023 |
| `/api/v2/endpoint`    | 2.0    | 31 de Dezembro de 2024 |
| `/api/v3/endpoint`    | 3.0    | 31 de Dezembro de 2025 |

Após a data limite de suporte para uma versão, recomendamos fortemente que os usuários migrem para a versão mais recente para continuar recebendo suporte e aproveitar as funcionalidades mais recentes.

## Notificações de Versões
Quando uma nova versão da API é lançada ou uma versão antiga atinge a data limite de suporte, notificaremos os usuários por e-mail e por nossa conta no Github. Por e-mail as notificações serão enviadas para o endereço de e-mail associado à chave de assinatura da API e para o contato principal da agência.

As notificações incluirão informações sobre a nova versão disponível, as mudanças e melhorias introduzidas, além da data limite de suporte para versões anteriores. Também forneceremos orientações e recursos adicionais para ajudar os usuários a migrar para a versão mais recente.

## Entre em Contato
Se você tiver dúvidas sobre o versionamento das APIs ou precisar de suporte adicional, entre em contato com nossa equipe de suporte técnico através dos seguintes canais:

- Github
- E-mail: support.b2b@voeazul.com.br

Estamos prontos para ajudá-lo com qualquer dúvida ou consulta relacionada às versões das APIs.
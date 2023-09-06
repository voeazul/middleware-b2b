# Modelo de Abertura de Issues

Para realização de abertura de issues, de modo a facilitar a análise do problema reportado e receber um feedback mais rapido e com maior assertividade, é impreescindivel que o template seja seguido.

Aqui você pode encontrar o [Template](./issue-template.md) para copiar e usa-ló na abertura da issue, e abaixo está o descritivo de cada ponto.

## Descrição do Problema

Descreva aqui de forma clara e concisa o problema encontrado no barramento.

## Etapas para Reproduzir

Liste aqui as etapas necessárias para reproduzir o problema. Inclua informações como URL da API, parâmetros utilizados, desde que os mesmos não contenham informações sensíveis, entre outras informações.

1. Execute um POST na API 'api/v1/b2b/auth'.
2. Execute um POST na API 'api/v1/b2b/rotaexemplo'.
3. Na chamada POST da API 'api/v1/b2b/rotaexemplo' use o seguinte payload:  
`{origin: "SDU", destination: "VCP", firstName: "*****"}`.
4. Após isso é retornado o erro "500 - Erro interno inesperado".

__Sempre se atente a remover qualquer informação que seja de cunho privado ou sensível.__  
Exemplo de informações que __não devem__ ser inclusas na issue sob nenhuma circunstancia:

- Chaves de Assinatura.
- Nomes e documentos pessoais.
- Dados de Cartões de Crédito.
- Qualquer informação que infrinja a LGPD.

__Obs.:__ Caso necessário alguma informação adicional, será solicitado na issue, caso a informação seja de cunho privado, será solicitado via e-mail ao autor da issue.

Exemplos com rotas e problemas comuns:

Exemplo 1:

1. Execute um POST na API 'api/v1/token'.
2. Execute um POST na API 'api/v1/authenticate'.
3. Na chamada POST da API 'api/v1/airSearch' use o seguinte payload:  
`{
    "passengers": [
        {
            "type": "ADT",
            "count": 1
        }
    ],
    "journeys": [
        {
            "origin": "POA",
            "destination": "VCP",
            "departure": "2023-09-20T00:00:00"
        }
    ],
    "criteria": {
        "promotionCode": "",
        "baggageAllowance": "All",
        "directFlightsOnly": false
    }
}`.
4. Após isso é retornado o erro "502 - Bad Gateway" de codigo interno "Navitaire.Request.Failed".

Exemplo 2:

1. Execute um POST na API 'api/v1/token'.
2. Execute um POST na API 'api/v1/authenticate'.
3. Execute um POST na API 'api/v1/airSearch' use o seguinte payload:  
`{
    "passengers": [
        {
            "type": "ADT",
            "count": 1
        }
    ],
    "journeys": [
        {
            "origin": "MVD",
            "destination": "BEL",
            "departure": "2023-09-30T00:00:00"
        }
    ],
    "criteria": {
        "promotionCode": "",
        "baggageAllowance": "All",
        "directFlightsOnly": false
    }
}`.
4. Na chamada POST da API 'api/v1/order' usando no payload com um adulto para um voo somente ida.
5. Após isso é retornado o erro "502 - Bad Gateway" de codigo interno "Integration.InvalidFare".

Exemplo 3:

1. Execute um POST na API 'api/v1/token'.
2. Execute um POST na API 'api/v1/authenticate'.
3. Execute um POST na API 'api/v1/airSearch' use o seguinte payload:  
`{
    "passengers": [
        {
            "type": "ADT",
            "count": 2
        }
    ],
    "journeys": [
        {
            "origin": "MVD",
            "destination": "SDU",
            "departure": "2023-09-21T00:00:00"
        },
                {
            "origin": "SDU",
            "destination": "MVD",
            "departure": "2023-09-29T00:00:00"
        }
    ],
    "criteria": {
        "promotionCode": "",
        "baggageAllowance": "All",
        "directFlightsOnly": false
    }
}`.
4. Execute um POST na API 'api/v1/order' usando no payload com dois adultos para um voo de ida e volta.
5. Execute um GET na API 'api/v1/order'.
6. Após isso é retornado o erro "502 - Bad Gateway" de codigo interno "RequestFailed.Unexpected".

## Ambiente

- Ambiente utilizado: Homologação ou Produção.
- Linguagem do Sistema de Origem: Python, PHP, C#, etc.

## Informações Adicionais

Adicione qualquer informação adicional que possa ser relevante para a compreensão do problema, como mensagens de erro, logs ou outros detalhes.

## Passos já tentados para solucionar o problema

Liste quaisquer passos que você já tentou para resolver o problema, se aplicável.

## Contexto Adicional

Forneça qualquer contexto adicional que você julgar relevante para o problema.

---

Agradecemos por reportar esse problema. Iremos analisá-lo e responderemos o mais breve possível. Se necessário, entraremos em contato para solicitar mais informações.

Obrigado pela sua colaboração!

Equipe de Suporte.
# Modelo de Abertura de Issues

Para realização de abertura de issues, de modo a facilitar a análise do problema reportado e receber um feedback mais rapido e com maior assertividade, é impreescindivel que o template seja seguido.

Aqui você pode encontrar o [Template](./issue-template.md) para copiar e usa-ló na abertura da issue, e abaixo está o descritivo de cada ponto.

## Descrição do Problema

Descreva aqui de forma clara e concisa o problema encontrado no barramento.

## Etapas para Reproduzir

Liste aqui as etapas necessárias para reproduzir o problema. Inclua informações como URL da API, parâmetros utilizados, desde que os mesmo não contenha informações sensiveis, entre outras informações.

1. Execute um POST na API 'api/v1/b2b/auth'.
2. Execute um POST na API 'api/v1/b2b/rotaexemplo'.
2. Na chamada POST da API 'api/v1/b2b/rotaexemplo' use o seguinte payload:  
`{origin: "SDU", destination: "VCP", firstName: "*****"}`.
3. Após isso é retornado o erro "500 - Erro interno inesperado".

__Sempre se atente a remover qualquer informação que seja de cunho privado ou sensivel.__  
Exemplo de informações que __não devem__ ser inclusas na issue sob nenhuma circunstancia:

- Chaves de Assinatura.
- Nomes e documentos pessoais.
- Dados de Cartões de Crédito.
- Qualquer informação que infrinja a LGPD.

__Obs.:__ Caso necessário alguma informação adicional, será solicitado na issue, caso a informação seja de cunho privado, será solicitado via e-mail ao autor da issue.

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
# Solicitação de Chave de Assinatura

O Barramento B2B tem uma camada de gerenciamento e segurança, chamada API Gateway, que é uma plataforma onde é possível gerenciar e proteger as APIs de forma escalável e eficiente. Para ter acesso as nossas APIs você precisa solicitar uma Chave de Assinatura.

## O que é uma Chave de Assinatura?

Uma Chave de Assinatura é um identificador exclusivo usado para autenticar suas solicitações às APIs. Para cada usuário ou aplicativo que consome nossas APIs recebe uma chave de acesso única, que deve ser utilizada para identificar e autorizar as chamadas.
Essa chave de assinatura deve ser solicitada no Portal do Desenvolvedor.

## Acesso ao Portal do Desenvolvedor

Nosso Portal do Desenvolvedor é uma plataforma dinâmica que oferece uma visão completa das APIs disponíveis para integração. Lá, você pode solicitar e gerenciar suas chaves de assinatura, além de encontrar documentações e utilizar um sandbox para testar as chamadas às APIs.

Estamos utilizando o Portal do Desenvolvedor fornecido pelo Azure API Management. Acesse as URLs abaixo para acessar o portal nos ambientes de Homologação e Produção.

[Portal Desenvolvedor Ambiente de Homologação](https://apim-stg-us-general.developer.azure-api.net/product#product=sales-b2b-agency)   
[Portal Desenvolvedor Ambiente de Produção](https://apim-prd-us-general.developer.azure-api.net/product#product=sales-b2b-agency)

## Como se cadastrar

Siga as etapas abaixo para se cadastrar no Portal do Desenvolvedor:

1. Acesse a URL do Portal do Desenvolvedor para o ambiente desejado.
2. Clique em "Sign up" na página inicial.
3. Preencha o formulário de registro com suas informações.
4. Após o registro, você receberá um e-mail de confirmação.
5. Siga as instruções no e-mail para confirmar sua conta.
6. Após a confirmação, você poderá fazer login no Portal do Desenvolvedor.

![Signup](/docs/assets/subkey-signup.png)

## Solicitando uma Chave de API

Siga as etapas abaixo para solicitar uma chave de assinatura:

1. Faça login no Portal do Desenvolvedor.
2. Navegue até a seção "Products".
3. Filtre pelo produto "__Sales B2B - Agency__", e após a exibição, clique em cima do mesmo.
![Passos 2 e 3](/docs/assets/subkey-search-product.png)
4. De um nome para sua chave de assinatura, por padrão, deixe o nome da sua chave com o nome da agência de forma que o responsável pela aprovação consiga identificar quem irá fazer uso. Exemplo:
    - azul-viagens-key
5. Clique em "Subscribe".
![Passos 4 e 5](/docs/assets/subkey-subscribe-product.png)
6. Após isso, é necessário enviar um e-mail para suporteb2b@voeazul.com.br, com um print evidenciando a URL do ambiente contendo o nome da chave, para que o acesso seja providenciado.
7. Após a execução do tópico anterior, é necessário aguardar a aprovação do time técnico Azul.
8. Após a aprovação, será enviado uma notificação no e-mail utilizado na criação da conta no portal do desenvolvedor.

## Visualizando uma Chave de Assinatura

Siga as etapas abaixo para visualizar uma chave de assinatura:

1. Faça login no Portal do Desenvolvedor.
2. Navegue até a seção "Profile".
3. Será listado todas suas solicitações de chaves e chave já aprovadas.
4. Se sua chave já estiver aprovada, será exibido a opção de "Show", caso não esteja exibindo essa opção, sua solicitação ainda não foi aprovada.
4. Em caso de aprovada, clique em "Show" e copie a chave exibida.
5. Após isso é só adicionar essa chave no header "Ocp-Apim-Subscription-Key" de todas as requisições para as APIs do barramento.

![Subscriptions](/docs/assets/subkey-show-key.png)

__Importante__: Essa chave é de uso individual da agência e não deve ser divulgada para pessoas não autorizadas.
Caso seja identificado algum comportamento incomum na utilização das APIs por meio da chave de assinatura, a mesma será revogada no ato, interrompendo todas as operações com o barramento e sendo necessário a geração e aprovação de uma nova chave.

## Atualizando uma Chave de Assinatura

O time de segurança da AZUL sugere que a cada seis meses a subscription key seja atualizada pelos parceiros para mitigar riscos de ataques e invasões, ao não trocar a chave regularmente, existe o risco de vazamento e acesso de pessoas não autorizadas. Caso sejam verificados comportamentos inesperados com as chaves em utilização elas serão bloqueadas pelo time de segurança da Azul, e os parceiros deverão executar o fluxo abaixo para voltar a ter acesso.

![Change Subscription Key](/docs/assets/subkey-change-subkey_PT.png)

Siga as etapas abaixo para regerar uma chave:

1. Faça login no Portal do Desenvolvedor.
2. Navegue até a seção "Profile".
3. Será listado todas suas solicitações as chaves de assinatura ativas.
4. Encontre a chave que deseja regerar.
5. Clique na opção "Regenerate" da linha da chave de assinatura que desejar regerar.
6. Após isso é só atualizar a chave nos lugares necessários e utilizar.

![Regenerate Subscription Key](/docs/assets/subkey-regenerate-key.png)

Agora você está pronto para aproveitar todos os benefícios das nossas APIs. Se tiver alguma dúvida ou precisar de suporte adicional, entre em contato conosco.
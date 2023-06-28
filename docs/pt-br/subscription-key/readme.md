# Solicitação de Chave de Assinatura

O barramento B2B tem uma camada de gerenciamento e segurança, chamada API Gateway, que é uma plataforma onde é possivel gerenciar e proteger as APIs de forma escalável e eficiente. Para ter acesso as nossas APIs você precisa solicitar uma Chave de Assinatura no Portal do Desenvolvedor.

## O que é uma Chave de Assinatura?

Uma Chave de Assinatura, é um identificador exclusivo usado para autenticar as solicitações feitas às APIs. Para cada usuário ou aplicativo que consome uma API de nossas APIs é atribuído a uma chave de acesso única, que é usada para identificar e autorizar as chamadas.
Essa chave de assinatura deve ser solicitada no Portal do Desenvolvedor.

## Acesso ao Portal do Desenvolvedor

O Portal do Desenvolvedor que estamos utilizando atualmente é o portal do Azure API Management, pode ser acessado através da URLs abaixo.

[Portal Desenvolvedor ambiente de Homologação](https://apim-stg-us-general.developer.azure-api.net)   
[Portal Desenvolvedor ambiente de Produção](https://apim-stg-us-general.developer.azure-api.net)

## Como se cadastrar

1. Acesse a URL o Portal do Desenvolvedor do ambiente desejado.
2. Clique em "Sign up" na página inicial.
3. Preencha o formulário de registro com suas informações.
4. Após o registro, você receberá um e-mail de confirmação.
5. Siga as instruções no e-mail para confirmar sua conta.
6. Após a confirmação, você poderá fazer login no Portal do Desenvolvedor.

![Signup](/docs/assets/subkey-signup.png)

## Solicitando uma Chave de API

1. Faça login no Portal do Desenvolvedor.
2. Navegue até a seção "Products".
3. Selecione a API para a qual deseja solicitar uma chave.
4. Filtre pelo produto "Sales B2B - Agency", e após a exibição do mesmo, clique em cima do mesmo.
5. De um nome para sua subscription, por padrão, deixe o nome da sua subscription com o nome da agência que irá fazer uso da subscription. Exemplo:
    - azul-viagens
6. Clique em "Subscribe".
7. Após isso, é necessário aguardar a aprovação do time Comercial da Azul.

## Visualizando uma Chave de Assinatura

1. Faça login no Portal do Desenvolvedor.
2. Navegue até a seção "Profile".
3. Será listado todas sua solicitações de chaves e chave já aprovadas.
4. Se sua chave já estiver aprovada, será exibido a opção de "Show", caso não esteja exibindo essa opção, sua solicitação ainda não foi aprovada.
4. Em caso de aprovada, clique em "Show" e copie a chave exibida.
5. Após isso é só adicionar essa chave no header "Ocp-Apim-Subscription-Key" de todas requisições para as APIs do barramento.

![Subscriptions](/docs/assets/subkey-show-key.png)

__Importante__: Essa chave é de uso individual da agência e não deve ser divulgada para pessoas não autorizadas.
Caso seja identificado algum comportamento incomum na utilização das APIs por meio da chave de assinatura, a mesma será revogada no ato, interropendo todas as operações com o barramento e sendo necessário a geração e aprovação de uma nova chave.

## Atualizando uma Chave de Assinatura

Em caso de chaves que foram vazadas a pessoas sem autorização, o criador da chave de assinatura poderá regerar a mesma no portal do desenvolvedor, considerando que ao regerar uma chave, a antiga é invalidada imediatamente e perde o acesso as APIs do barramento.

Regerando uma chave:

1. Faça login no Portal do Desenvolvedor.
2. Navegue até a seção "Profile".
3. Será listado todas sua solicitações as chaves de assinatura ativas.
4. Encontre a chave que deseja regerar.
5. Clique na opção "Regenerate" da linha da chave de assinatura que desejar regerar.
6. Após isso é só atualizar a chave nos lugares necessários e utilizar.

![Regenerate Subscription Key](/docs/assets/subkey-regenerate-key.png)
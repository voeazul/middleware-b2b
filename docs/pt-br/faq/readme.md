# Perguntas Frequentes (FAQ)

Aqui estão algumas perguntas frequentes sobre o uso do Barramento B2B:

## 1. Como posso começar a vender passagens da Azul?

Para começar a se integrar com nosso barramento e disponibilizar nossos voos em sua agência, entre em contato com nosso departamento comercial para cadastrar sua agencia de turismo

## 2. Como posso obter acesso às APIs do Barramento?

Para obter acesso às APIs do barramento, antes você deve seguir a orientação descrita no tópico anterior, e após isso, basta você seguir os passos descritos no documento [Como Solicitar uma Chave de Assinatura](/docs/pt-br/subscription-key/readme.md).

## 3. Como posso como realizar uma venda de passagens aéreas?

Para realizar uma venda de passagens aéreas, você deve utilizar a API de Order. Para informações mais detalhadas de como fazer um fluxo de venda, confira a documentação [Fluxos Básicos](/docs/pt-br/postman/README.md).

## 4. Posso cancelar uma reserva de passagem aérea?

Sim, é possível cancelar uma reserva.
Para realizar um cancelamento de passagens aéreas, você deve utilizar a API de Order Management. Para informações mais detalhadas de como fazer um fluxo de cancelamento, confira a documentação [Fluxos Básicos](/docs/pt-br/postman/README.md).

## 5. Como posso adicionar serviços adicionais à reserva de um passageiro?

Para realizar uma inclusão de serviços adicionais você precisa utilizar a API de Order Services, confira a documentação [Fluxos Básicos](/docs/pt-br/postman/README.md).

## 6. Como posso obter informações sobre voos disponíveis?

Você pode obter detalhes de um voo utilizando a API de Shopping, confira a documentação [Fluxos Básicos](/docs/pt-br/postman/README.md).

## 7. Como realizar a autenticação no barramento?

Você pode realizar a autenticação primeiramente obtendo o token na API de Authentication após a obtenção do token utilizar o mesmo na autenticação através da API de User.

## 8. Como alterar o ponto de venda com meu agente?

Você pode alterar o ponto de venda do usuário logado através da API de User.

## 9. Como marcar um assento à reserva de um passageiro?

Para realizar uma inclusão de assentos você precisa utilizar a API de Order Seats, confira a documentação [Fluxos Básicos](/docs/pt-br/postman/README.md).

## 10. Como adicionar bagagens à reserva de um passageiro?

Para realizar uma inclusão de bagagens você precisa utilizar a API de Order Services, confira a documentação [Fluxos Básicos](/docs/pt-br/postman/README.md).

## 11. Posso adicionar trechos em uma reserva?

Sim, é possível adicionar trechos uma reserva.
Para realizar a adição de trechos, você deve utilizar a API de Order Management. Para informações mais detalhadas de como fazer um fluxo de adição de trechos, confira a documentação [Fluxos Básicos](/docs/pt-br/postman/README.md).

## 12. Posso cancelar trechos em uma reserva?

Sim, é possível cancelar trechos uma reserva.
Para realizar cancelamento de trechos, você deve utilizar a API de Order Management. Para informações mais detalhadas de como fazer um fluxo de cancelamento de trechos, confira a documentação [Fluxos Básicos](/docs/pt-br/postman/README.md).

## 13. O que significam os códigos: AG, CF, AX, VI, MC, DI, HP, EL e TP, descritos no methodCode do swagger no endpoint do método POST Order/payments v1 ?

Os significados são: 
- AG = Conta de crédito direto com a Azul
- CS = Credit Shell, quando o cliente inputa crédito em sua reserva para usar posteriormente
- CF = Credit file, quando o cliente consume o  crédito existente no Credit Shell
- AX = American Express
- VI = VIsa
- MC = MasterCard
- DI = DinnersClub
- HP = HiperCard
- EL = ELO
- TP = UATP

## 14. Para que serve o serviço de Authentication/Token e qual seu tempo de duração por sessão?

O serviço de Authentication é responsável por autenticar e identificar o usuário sistêmico do Barramento B2B.  
A obtenção do token através do serviço Authentication é obrigatória no início de cada sessão do barramento B2B, e um token gerado para um agente de viagens deve ser utilizado até o final daquela sessão deste mesmo agente. 
O token irá expirar após 15 minutos de inatividade. Após este tempo, será necessário solicitar um novo token, caso contrário os métodos chamados passarão a retornar o status HTTP 401: Unauthorized.

## 15. Qual o processo de validação e Go Live?
 
O processo de validação e go live está detalhado no link [Processo para uso do barramento em produção](/docs/pt-br/processo-inicio-producao/readme.md).

## 16. O que devo fazer quando recebo o erro: HTTP 409: Conflict, "message": "An agent is already authenticated."

Nesta situação deverá ser enviado no header a variável: User_Agent com o nome: salesb2b/"Nome_da_Agência", sendo o nome da agência o nome da sua empresa para maiores detalhes acessar o link [Validação de UsersAgent](/README.pt.md).


## 17. O que devo fazer quando recebo o erro: HTTP 409: Conflict, "message": "An agent is already authenticated."

Nesta situação deverá ser enviado no header a variável: User_Agent com o nome: salesb2b/"Nome_da_Agencia"

## 18. Como encerrar a utilização de um token em uso?
Resposta: Basta executar um Delete token na api authentication. 


## 19. Como alterar o usuário utilizando o mesmo token? Devemos usar /api/v1/organizations/:organizationCode/users/:userKey/password/reset? 
Resposta: Basta executar um Delete logout na API de users.


## 20. Quais são as diferenças entre Primary Key e Secondary Key (estamos usando apenas a Primary Key no Postman) 
Resposta: Não existe diferença entre a funcionalidade da primary e secondary key, ambas são criadas apenas por uma questão de segurança, e caso seja necessário o bloqueio de uma a outra possa ser utiliza automaticamente. Inclusive, o time de segurança sugere a atualização semestral das subscripitions Keys utilizadas.


## 21. Existe um método de rotas disponíveis? Devo considerar o método stations para esta consulta?
Resposta: Atualmente as informações devem ser consultadas através da API /api/v1/stations, futuramente será desenvolvido um método de rotas.


---

Esperamos que essas perguntas frequentes tenham ajudado a esclarecer algumas dúvidas comuns sobre o uso do barramento para integração com a Navitaire. Se você tiver outras perguntas ou precisar de mais informações, não hesite em entrar em contato com a nossa equipe de suporte.

Happy coding! 😊✈️

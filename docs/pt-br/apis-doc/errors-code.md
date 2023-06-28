# Códigos de Erro e Mensagens

Nosso barramento tem diversas regras e tratativas para garantir a integridade do fluxo. Abaixo estão mapeados todos possiveis códigos de erro, códigos de resposta HTTP, e suas respectivas mensagens de erro:

## Erros Gerais

| Código HTTP       | Código Interno | Mensagem de Erro                               |
| ----------------- | -------------- | ----------------------------------------------
| 401 Não Autorizado  | Não aplicavel         | Usuário não está autenticado para acessar o recurso                        
| 403 Não Permitido  | Não aplicavel         | Usuário autenticado, mas sem permissões suficientes para acessar o recurso 
| 404 Not Found     | Não aplicavel         | Recurso não encontrado                         |
| 500 Internal Server Error | Não aplicavel    | Erro interno do servidor                       |

## Erros Negociais

| Código HTTP       | Código Interno | Mensagem de Erro                               |
| ----------------- | -------------- | ----------------------------------------------
| 400 Bad Request   | UserCannotBeUnlocked      | Somente usuários podem desbloquear um Agent           |
| 409 Conflict   | InvalidGetBooking       | Chamada valida apenas para reserva sem PNR           |
| 403 NotAllowed   | AgentWithoutAccess       | Agent informado não possui acesso nessa reserva          |
| 404 NotFound   | UserNotFound       | Usuário informado não existe           |

---

Essa tabela apresenta os erros negociais encontrados no barramento, juntamente com os códigos HTTP correspondentes, códigos internos e mensagens de erro associadas.
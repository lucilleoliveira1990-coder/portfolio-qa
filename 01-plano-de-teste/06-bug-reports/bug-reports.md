BUG-001 — Login com senha inválida

Título: Login permitido com senha inválida

ID: BUG-LOGIN-001

Funcionalidade: Login

Ambiente: Windows + Google Chrome

Severidade: Alta

Prioridade: Alta

Status: Aberto

Pré-condição

Usuário deve possuir acesso à página de Login.

Passos para reprodução

1. Acessar a aplicação.
2. Acessar a área de Login.
3. Informar os dados necessários para reproduzir o problema.
4. Clicar em Login.

Resultado esperado: O sistema deve rejeitar a autenticação, impedir o acesso e apresentar uma mensagem informando que as credenciais são inválidas.

Resultado obtido: O sistema permitiu o acesso ao site mesmo após informar uma senha inválida.


Evidência<img width="646" height="329" alt="Sem título1" src="https://github.com/user-attachments/assets/a30aeec3-7f48-4c7c-ae5c-9d99f1f89ef8" />


Impacto: O comportamento permite que um usuário seja autenticado mesmo utilizando uma senha incorreta, comprometendo a segurança e a confiabilidade do processo de autenticação.


Observação: O comportamento deve ser analisado para verificar se a autenticação está validando corretamente a senha informada.

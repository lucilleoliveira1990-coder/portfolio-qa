## Casos de teste
 
## CT001 — Login com credenciais válidas

Objetivo: Validar Login utilizando credenciais válidas.

Pré-condição: Usuário cadastrado.

Passos:
1. Acessar a tela de Login.
2. Informar e-mail válido.
3. Informar senha válida.
4. Clicar em "Entrar".
 
Resultado esperado: O sistema deve autenticar o usuário e direcioná-lo para a área autenticada.

Resultado obtido: Login realizado com sucesso. O usuário foi autenticado e redirecionado para a área restrita da aplicação.

Status: Passou.


## CT002 — Login com senha inválida

Objetivo: Verificar se o sistema impede acesso com senha incorreta.

Pré-condição: Usuário cadastrado.

Passos:
1. Acessar a tela de Login.
2. Informar e-mail válido.
3. Informar senha incorreta.
4. Clicar em "Entrar".

Resultado esperado: O sistema deve impedir o acesso e apresentar mensagem informando que as credenciais são inválidas.

Resultado obtido: O sistema permitiu o acesso mesmo após informar uma senha inválida. O usuário foi autenticado e redirecionado para a área restrita da aplicação.

Status: Falhou.

Observação: O comportamento obtido não corresponde ao resultado esperado, pois o sistema deveria bloquear o acesso quando a senha informada fosse inválida.


## CT003 — Login com e-mail inválido

Objetivo: Verificar se o sistema impede Login com e-mail inválido.

Passos:
1. Acessar a tela de Login.
2. Informar e-mail inválido.
3. Informar senha.
4. Clicar em "Entrar".

Resultado esperado: O sistema deve impedir o acesso e apresentar mensagem de validação.

Resultado obtido: O sistema permitiu o acesso mesmo após informar um e-mail inválido. O usuário foi autenticado e redirecionado para a área restrita da aplicação.

Status: Falhou.

Observação: O sistema deveria impedir o login e exibir uma mensagem informando que o e-mail ou as credenciais são inválidos.


## CT004 — E-mail vazio

Passos:
1. Acessar a tela de Login.
2. Não preencher o campo e-mail.
3. Informar uma senha.
4. Clicar em "Entrar".

Resultado esperado: O sistema deve informar que o campo e-mail é obrigatório.

Resultado Obtido: O sistema não permitiu o login e exibiu uma mensagem informando o campo de e-mail inválido.

Status: Passou.


## CT005 — Senha vazia

Passos:
1. Acessar a tela de Login.
2. Informar e-mail válido.
3. Não preencher a senha.
4. Clicar em "Entrar".

Resultado esperado: O sistema deve informar que o campo senha é obrigatório.

Resultado Obtido: O sistema não permitiu o login e exibiu uma mensagem informando o campo de senha inválida.

Status: Passou.


## CT006 — E-mail e senha vazios

Passos:
1. Acessar a tela de Login.
2. Não preencher nenhum campo.
3. Clicar em "Entrar".

Resultado esperado: O sistema deve apresentar as validações correspondentes aos campos obrigatórios.

Resultado Obtido: O sistema não permitiu o login e exibiu mensagens informando os campos de e-mail inválido e senha em branco.

Status: Passou.


## CT007 — E-mail não cadastrado

Passos:
1. Informar um e-mail que não está cadastrado.
2. Informar uma senha.
3. Clicar em "Entrar".

Resultado esperado: O sistema deve impedir o acesso e apresentar uma mensagem adequada.

Resultado obtido: O sistema permitiu o login mesmo utilizando um e-mail que não está cadastrado na aplicação.

Status: Falhou.

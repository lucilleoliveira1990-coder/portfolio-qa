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


## CT008 — E-mail em formato inválido

Dados: lucille2206@gmail.com

Passos:

1. Informar o e-mail inválido.
2. Informar uma senha.
3. Clicar em Login.

Resultado esperado: O sistema deve rejeitar o formato inválido.

Resultado obtido: O sistema permitiu o envio do formulário mesmo com o e-mail em formato inválido.

Status: Falhou.


## CT009 — E-mail com letras maiúsculas

Passos:

1. Informar um e-mail válido utilizando letras maiúsculas.
2. Informar a senha correspondente.
3. Clicar em Login.

Resultado esperado: O sistema deve tratar o e-mail conforme a regra de autenticação definida.

Resultado obtido: O sistema aceitou o e-mail com letra maiúscula e realizou o login com sucesso.

Status: Passou.


## CT010 — Campos obrigatórios

Objetivo: Verificar se os campos obrigatórios são devidamente identificados.

Passos:

1. Acessar a tela de Login.
2. Deixar os campos vazios.
3. Tentar realizar o login.

Resultado esperado: O sistema deve informar os campos obrigatórios que precisam ser preenchidos.

Resultado obtido: O sistema impediu o login e solicitou o preenchimento dos campos obrigatórios.

Status: Passou.


## CT011 — Mensagem de erro

Passos:

1. Informar credenciais inválidas.
2. Clicar em Login.

Resultado esperado: O sistema deve apresentar mensagem clara informando que não foi possível realizar a autenticação.

Resultado obtido: O sistema apresentou uma mensagem de erro, porém o acesso ao site foi realizado normalmente.

Status: Falhou.


## CT012 — Botão Login

Passos:

1. Acessar a página de Login.
2. Verificar o botão Login.
3. Clicar no botão.

Resultado esperado: O botão deve responder à ação do usuário e iniciar o processo de autenticação/validação.

Resultado obtido: Ao clicar no botão "Entrar", o sistema respondeu à ação do usuário e iniciou o processo de validação das credenciais informadas.

Status: Passou.


## CT013 — Acesso após login

Passos:

1. Informar credenciais válidas.
2. Clicar em Login.
3. Observar a página apresentada após autenticação.

Resultado esperado: O usuário deve ser direcionado para a área correspondente após o login.

Resultado obtido: Após informar credenciais válidas e clicar no botão "Entrar", o sistema autenticou o usuário e permitiu o acesso à área autenticada da aplicação.

Status: Passou.

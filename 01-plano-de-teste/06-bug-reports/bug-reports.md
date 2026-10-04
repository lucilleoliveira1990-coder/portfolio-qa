## BUG-001 — Login com senha inválida

Título: Login permitido com senha inválida

ID: BUG-LOGIN-001

Funcionalidade: Login

Ambiente: Windows + Google Chrome

Severidade: Alta

Prioridade: Alta

Status: Aberto

Pré-condição: Usuário deve possuir acesso à página de Login.

Passos para reprodução

1. Acessar a aplicação.
2. Acessar a área de Login.
3. Informar os dados necessários para reproduzir o problema.
4. Clicar em Login.

Resultado esperado: O sistema deve rejeitar a autenticação, impedir o acesso e apresentar uma mensagem informando que as credenciais são inválidas.

Resultado obtido: O sistema permitiu o acesso ao site mesmo após informar uma senha inválida.

Evidência

<img width="645" height="343" alt="Sem título1" src="https://github.com/user-attachments/assets/7e5bdd78-7909-461f-8b7b-d9ca86cb5ea1" />

<img width="574" height="371" alt="Sem título2" src="https://github.com/user-attachments/assets/65e3f0a4-7f40-46fc-9232-942216268a19" />


Impacto: O comportamento permite que um usuário seja autenticado mesmo utilizando uma senha incorreta, comprometendo a segurança e a confiabilidade do processo de autenticação.


Observação: O comportamento deve ser analisado para verificar se a autenticação está validando corretamente a senha informada.


## BUG-002 — Login com e-mail inválido

Título: Login permitido com e-mail inválido

ID: BUG-LOGIN-002

Funcionalidade: Login

Ambiente: Windows + Google Chrome

Severidade: Alta

Prioridade: Alta

Tipo de teste: Teste funcional

Status: Aberto

Pré-condição: Usuário deve possuir acesso à página de Login.

Passos para reprodução

1. Acessar a página de login.
2. Informar um e-mail em formato inválido.
3. Informar uma senha.
4. Clicar no botão Login.

Resultado esperado: O sistema deve validar o formato do e-mail e impedir o login quando o endereço informado for inválido.

Resultado obtido: O sistema permitiu o acesso ao site mesmo com o e-mail informado em formato inválido.

Evidência

<img width="664" height="351" alt="Sem título3" src="https://github.com/user-attachments/assets/8ad2e18c-a541-42be-87e7-256b807e1761" />

<img width="608" height="382" alt="Sem título4" src="https://github.com/user-attachments/assets/b27ae173-e2d3-4cea-9374-0ed609ff6bf7" />



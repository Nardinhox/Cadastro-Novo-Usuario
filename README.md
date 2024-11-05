**Projeto de Testes Automatizados**: Cadastro de Novo Usuário
Este projeto utiliza o Cypress para automatizar testes de cadastro e login de novo usuário no site Demoblaze. O projeto é ideal para demonstração de automação de testes e inclui uma validação completa do fluxo de cadastro e login de um usuário recém-cadastrado.

**Pré-requisitos**
Certifique-se de ter as seguintes ferramentas instaladas para executar o teste.
1. Node.js e npm instalados na máquina.
2. Cypress instalado como dependência de desenvolvimento.

**Configuração do Ambiente**
1. Clone o repositório para a sua máquina
Execute o comando "git clone https://github.com/Nardinhox/projeto-cadastro-novo-usuario.git" no terminal, depois navegue até ele executando o comando
"cd projeto-cadastro-novo-usuario".

2. Instalar Node.js
Verifique se o Node.js está instalado executando "node -v" no terminal. Se não estiver instalado, siga as instruções no site oficial do Node.js (https://nodejs.org/pt).

3. Instalar Cypress
Execute o comando "npm install cypress --save-dev" no terminal para instalar o Cypress como uma dependência de desenvolvimento.

4. Configurar o Projeto
Certifique-se de que o projeto contenha um arquivo "package.json". Se não tiver, crie um executando "npm init -y" no terminal.

5. Instale as dependências do projeto:
Execute o comando "npm install" no terminal.

**Estrutura do Projeto**
├── cypress/
│   ├── e2e/
│   │   └── Teste_Cadastro.cy.js          # Testes de cadastro e login de usuário
│   ├── support/                          # Funções de suporte e comandos customizados
│   └── cypress.config.js                 # Configurações do Cypress
├── node_modules/                         # Dependências do projeto
├── package.json                          # Arquivo de configuração de dependências e scripts
└── README.md                             # Documentação do projeto

**Testes Implementados**
O projeto contém dois testes principais:
1. Cadastro de Novo Usuário
    Acessa o site do Demoblaze.
    Abre o modal de "Sign up" e insere um nome de usuário único e uma senha.
    Clica em "Sign up" e valida que o cadastro foi realizado com sucesso capturando o alerta exibido.

2. Validação de Login com o Usuário Cadastrado
    Acessa o site do Demoblaze.
    Abre o modal de "Log in" e insere as mesmas credenciais usadas no cadastro.
    Clica em "Log in" e valida que o login foi bem-sucedido verificando a presença do nome de usuário na página.

**Executando o Teste**
Existem duas formas principais de executar os testes:
1. Abrindo a Interface Gráfica do Cypress
    Execute o comando "npx cypress open" no terminal.           # Isso abrirá a interface do Cypress, onde você pode selecionar e rodar os testes.

2. Executando no Modo Headless
    Execute o comando "npx cypress run" no terminal.            # Para rodar todos os testes diretamente no terminal.

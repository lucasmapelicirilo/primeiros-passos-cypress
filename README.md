# Testes Automatizados com Cypress

Repositório destinado aos meus estudos e à prática de **Qualidade de Software (QA)**, com foco em testes automatizados End-to-End (E2E) utilizando Cypress e JavaScript.

## Estrutura do projeto

Os testes automatizados estão organizados na pasta `Cypress/e2e/`:

```text
Cypress/
└── e2e/
    ├── loginspec.cy.js
    └── testlogin.cy.js
```

O repositório também contém outras pastas e arquivos de configuração utilizados no desenvolvimento e na execução dos testes.

## Cenários automatizados

### `loginspec.cy.js`

Testes relacionados ao fluxo básico de autenticação:

- Login com sucesso.
- Login com falha.

### `testlogin.cy.js`

Testes de diferentes combinações de credenciais e do fluxo de autenticação:

- Login com sucesso (usuário e senha corretos).
- Usuário correto e senha incorreta.
- Senha correta e usuário incorreto.
- Login e logout.
- Usuário correto e campo de senha vazio.
- Senha correta e campo de usuário vazio.

## Tecnologias utilizadas

- JavaScript
- Cypress
- Node.js

## Como executar os testes

1. Clone o repositório:

   ```bash
   git clone URL_DO_REPOSITORIO
   ```

2. Acesse a pasta do projeto:

   ```bash
   cd NOME_DO_PROJETO
   ```

3. Instale as dependências:

   ```bash
   npm install
   ```

4. Abra a interface do Cypress:

   ```bash
   npx cypress open
   ```

   Ou execute os testes em modo headless:

   ```bash
   npx cypress run
   ```

> **Observação:** os comandos pressupõem que o projeto tenha um `package.json` e o Cypress instalado como dependência. Execute-os na pasta que contém o `package.json`.

## Objetivo

Praticar a criação e a execução de testes automatizados, desenvolver lógica de programação com JavaScript e ampliar meus conhecimentos em testes de software e QA.

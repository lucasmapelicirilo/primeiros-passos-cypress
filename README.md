
# Primeiros Passos com Cypress

Repositório dedicado aos meus estudos e à prática de **Quality Assurance (QA)**, com foco em testes automatizados End-to-End (E2E), utilizando Cypress e JavaScript.

O projeto utiliza a plataforma OrangeHRM como ambiente de prática para desenvolver habilidades em automação de testes, validação de funcionalidades e interação com elementos da interface.

## Estrutura do projeto

```text
primeiros-passos-cypress/
├── cypress/
│   ├── e2e/
│   │   ├── user.spec.cy.js
│   │   └── testlogin.cy.js
│   ├── fixtures/
│   │   └── users/
│   │       └── userData.json
│   └── support/
├── cypress.config.js
├── package.json
├── package-lock.json
└── README.md
```

## Cenários automatizados

### 1. user.spec.cy.js

Testes relacionados à autenticação e atualização de informações do usuário.

**User Info Update - Success**
- Acesso à página de login do OrangeHRM.
- Autenticação com credenciais válidas.
- Validação do redirecionamento para o Dashboard.
- Acesso à seção My Info.
- Atualização do primeiro nome e sobrenome.
- Preenchimento de campos adicionais:
  - Employee ID
  - Other ID
  - Driver's License
- Atualização de data.
- Envio do formulário.
- Validação da mensagem de atualização realizada com sucesso.

**Login - Fail**
- Tentativa de autenticação com credenciais inválidas.
- Validação da exibição do alerta de credenciais incorretas.

### 2. testlogin.cy.js

Cenários de validação do fluxo de autenticação:

- Login com sucesso.
- Usuário correto e senha incorreta.
- Senha correta e usuário incorreto.
- Login e logout.
- Usuário correto e campo de senha vazio.
- Senha correta e campo de usuário vazio.

## Recursos de automação utilizados

- **Seletores CSS:** identificação de elementos da interface.
- **Fixture:** armazenamento e reutilização de dados de teste em arquivo JSON.
- **Assertions:** validação de resultados esperados.
- **Comandos Cypress:** `cy.visit()`, `cy.get()`, `cy.type()`, `cy.click()`, `cy.clear()` e `cy.location()`.
- **Organização de seletores:** utilização de um objeto `selectorsList` para centralizar os seletores utilizados nos testes.

## Tecnologias utilizadas

- JavaScript
- Cypress
- Node.js
- JSON

## Como executar o projeto

Clone o repositório:

```bash
git clone https://github.com/lucasmapelicirilo/primeiros-passos-cypress.git
```

Acesse a pasta do projeto:

```bash
cd primeiros-passos-cypress
```

Instale as dependências:

```bash
npm install
```

Abra a interface do Cypress:

```bash
npx cypress open
```

Para executar os testes pelo terminal:

```bash
npx cypress run
```

## Objetivo

Desenvolver conhecimentos práticos em automação de testes, JavaScript e fundamentos de QA, aplicando conceitos de organização de testes, reutilização de dados, identificação de elementos e validação de funcionalidades em aplicações web.

# 🌐 Cypress — Automação de Testes E2E

## 📘 O que é o Cypress?

O **Cypress** é um framework de automação de testes end-to-end moderno, desenvolvido especialmente para aplicações web. Ele roda diretamente no navegador e oferece uma experiência de desenvolvimento rica, com recarregamento automático, execução visual dos testes e excelente integração com CI/CD.

> Ideal para testes de interface (UI), validação de APIs e testes de comportamento do usuário.

---

## 🔗 Documentação Oficial

📚 **[Why Cypress? - Documentação Oficial](https://docs.cypress.io/guides/overview/why-cypress)**  
> A explicação da proposta do Cypress, com exemplos de uso, vantagens e diferenciais.

---

## 🎥 Aulas e Vídeos no YouTube

Para quem prefere aprender na prática com vídeos, aqui estão alguns canais com playlists e tutoriais completos:

### 📺 Canal **QAutomatizado**
🔗 [Playlist Cypress para Iniciantes](https://youtu.be/HW8DZD2o68w)  
> Série completa com automação desde o zero, explicando passo a passo como instalar, configurar e automatizar testes com Cypress.

---

### 📺 Canal **Agilizei**
🔗 [Introdução ao Cypress](https://youtu.be/wIjtX0CPaw0)  
> Vídeo explicando os conceitos iniciais, comandos básicos e execução dos primeiros testes.

---

### 📺 Canal **QA Hacks e Dicas**
🔗 [Playlist de Cypress](https://www.youtube.com/watch?v=XZamVtEwZ_Y&list=PLBzB7PpRjH0oLLflTjpYnj3Dhyw_KFeXR)  
> Diversas aulas com foco prático em automação, uso de comandos personalizados e dicas para o dia a dia com Cypress.

---

### 📺 Canal **QA Papito**
🔗 [Testes Automatizados com Cypress](https://www.youtube.com/watch?v=FI65wNBKQkE)  
> Tutorial introdutório e direto ao ponto para começar a automatizar com Cypress em poucos minutos.

---

### 📺 Canal **Talking About Testing**
🔗 [Canal no YouTube](https://www.youtube.com/@TalkingAboutTesting)  
> Conteúdo aprofundado sobre Cypress, testes de software e qualidade de código, com vídeos atualizados, boas práticas e integrações com CI/CD.

---

### 📺 Canal **QAzando**
🔗 [Testes Automatizados com Cypress na prática](https://www.youtube.com/watch?v=3BtGP-DOYqo)  
> Aula prática sobre como configurar o ambiente, escrever testes e interpretar os resultados no Cypress.

---

## 🚀 Criação de um Projeto com Cypress

### Pré-requisitos
- Node.js instalado
- IDE de preferência (ex: Visual Studio Code)

---

### 1. Inicialização do Projeto

No terminal, dentro da pasta desejada:

```bash
npm init

# ou

npm init -y
```

Esse comando cria o `package.json`:

```json
{
  "name": "seu-barriga-cypress",
  "version": "1.0.0",
  "main": "index.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "keywords": [],
  "author": "",
  "license": "ISC",
  "description": ""
}
```

---

### 2. Instalação do Cypress

```bash
npm install cypress@13.13.3 -D
```

> Instala o Cypress como dependência de desenvolvimento

![instalacao_cypress](https://github.com/user-attachments/assets/6d36a1d7-670d-412e-9700-715df465664e)

---

### 3. Inicialização do Cypress

```bash
npx cypress open
```

> Pode solicitar permissões do firewall, especialmente no Windows.

![permissao_execucao_firewall_windows](https://github.com/user-attachments/assets/d732dc0a-1c7b-4ed6-bad8-9d1de66afd5a)

---

## ⚙️ Configuração do Cypress

### 1. Tela de Apresentação

![apresentacao_cypress](https://github.com/user-attachments/assets/58190e25-d17d-4b55-9de7-3c3d6efe5157)

---

### 2. Tela de Boas-Vindas

![tela_boas_vindas_cypres](https://github.com/user-attachments/assets/4c39203b-e61b-48a4-91a1-346c4be75f0f)

* Escolha entre **E2E** e **Component**
* Neste guia, focaremos em **E2E**

---

### 3. Estrutura Padrão

![estrutura_padrao_cypress](https://github.com/user-attachments/assets/e99a8bdf-2b09-4d1e-b43f-e59dbde81e7f)

---

### 4. Seleção de Navegador

![selecao_browser](https://github.com/user-attachments/assets/c41c9a6b-d190-4f50-a909-4b5ad63af469)

---

### 5. Criar um Novo Arquivo de Teste

![criar_novo_spec_de_teste](https://github.com/user-attachments/assets/0afc14be-6b68-47fb-85a1-f9410fb648ac)

---

### 6. Renomear o `cypress\e2e\spec.cy.js` o para ``cypress\e2e\register.cy.js``

![renomear_spec_teste](https://github.com/user-attachments/assets/8f054740-33db-4790-b605-48f91616b704)

---

### 7. Estrutura Básica do Arquivo

![estrutura_basica](https://github.com/user-attachments/assets/3c2cfa96-db15-4bdf-b9fa-a69341e241f1)

---

### 8. Primeira Execução

![primeira_execucao](https://github.com/user-attachments/assets/33a4ef06-3cc3-48ea-be2b-b629358a24ea)

---

### 9. Estrutura Final de Pastas

Após as configurações iniciais, essa será a estrutura esperada:

```text
cypress/
│
├── e2e/
│   └── register.cy.js          # Arquivo de teste E2E
│
├── fixtures/
│   └── example.json            # Massa de dados de exemplo
│
├── support/
│   ├── commands.js             # Comandos customizados
│   └── e2e.js                  # Arquivo de setup de testes
│
node_modules/                   # Pacotes instalados
cypress.config.js               # Arquivo de configuração do Cypress
package.json                    # Gerenciador de dependências
package-lock.json               # Versões exatas das dependências
```

![estrutura_de_pastas](https://github.com/user-attachments/assets/f89e289b-5a3c-49f4-9c82-3a09b448e819)

---


## ✅ Criação dos Testes

### 1. Teste Simples de Cadastro

Nesta primeira etapa, vamos criar um teste básico de cadastro no site **[SeuBarriga](https://seubarriga.wcaquino.me/login)**, sem usar hooks nem comandos personalizados.

```javascript
describe('Registrar', () => {
  it('deve criar uma conta com sucesso', () => {
    cy.visit('/')

    cy.contains('a', 'Novo usuário?').should('be.visible').click()

    cy.get('input[name="nome"]').should('be.visible').type('QA Cristiano')
    cy.get('input[name="email"]').should('be.visible').type('teste-qa@teste.com')
    cy.get('input[name="senha"]').should('be.visible').type('abc@123')

    cy.contains('input', 'Cadastrar').should('be.visible').click()

    cy.get('.alert-success').should('be.visible')
  })
})
```

![cadastro_com_sucesso](https://github.com/user-attachments/assets/c5a2ceea-64d2-4efc-9fd6-400d64d3fd99)

---

### 2. Teste Simples de Login

Agora, criamos um teste de login usando o mesmo padrão:

```javascript
  it('Deve realizar o login com o usuário cadastrado', () => {
    cy.visit('/')

    cy.get('.active > a').should('be.visible')

    cy.get('input[name="email"]').should('be.visible').type('teste-qa-16@teste.com')
    cy.get('input[name="senha"]').should('be.visible').type('abc@123')
    cy.contains('button', 'Entrar').should('be.visible').click()

    cy.get('.alert').should('be.visible')
  });
})
```

![login](https://github.com/user-attachments/assets/a35b2a8c-7c17-4947-af69-e582e4afa35d)

---

### 3. Introdução de Hooks

Perceba que chamamos `cy.visit('/')` em ambos os testes. Para evitar repetição, configuramos a URL base em `cypress.config.js` e usamos hooks:

```javascript
// cypress.config.js
const { defineConfig } = require("cypress");

module.exports = defineConfig({
  e2e: {
    baseUrl: "https://seubarriga.wcaquino.me/login",
    setupNodeEvents(on, config) {
       // implement node event listeners here
    },
  },
});
```

**Hooks** são funções executadas antes ou depois dos testes.  

- `before()` executa **uma vez** antes de todos os testes da spec.  
- `beforeEach()` executa **antes de cada** teste.

Exemplo com `beforeEach()`:

```javascript
describe('Registrar', () => {
  beforeEach(() => {
    // Executado antes de cada it()
    cy.visit('/')
  })

  it('deve criar uma conta com sucesso', () => {

    cy.contains('a', 'Novo usuário?').should('be.visible').click()

    cy.get('input[name="nome"]').should('be.visible').type('QA Cristiano')

    cy.get('input[name="email"]').should('be.visible').type('teste-qa-16@teste.com')

    cy.get('input[name="senha"]').should('be.visible').type('abc@123')

    cy.contains('input', 'Cadastrar').should('be.visible').click()

    cy.get('.alert')
      .should('be.visible')
  })

  it('Deve realizar o login com o usuário cadastrado', () => {

    cy.get('.active > a').should('be.visible')

    cy.get('input[name="email"]').should('be.visible').type('teste-qa-16@teste.com')

    cy.get('input[name="senha"]').should('be.visible').type('abc@123')

    cy.contains('button', 'Entrar').should('be.visible').click()

    cy.get('.alert')
      .should('be.visible')
  });
})
```

> Os hooks tornam o spec mais limpo e garantem que cada teste comece no ponto esperado.

---

### 4. Comandos Personalizados (Custom Commands)

Para reduzir ainda mais a repetição, criamos **Custom Commands** em `cypress/support/commands.js`:

```javascript
// cypress/support/commands.js

Cypress.Commands.add('registoComSucesso', (nome, email, senha) => {
  cy.contains('a', 'Novo usuário?').click()
  cy.get('input[name="nome"]').type(nome)
  cy.get('input[name="email"]').type(email)
  cy.get('input[name="senha"]').type(senha)
  cy.contains('input', 'Cadastrar').click()
})

Cypress.Commands.add('loginComSucesso', (email, senha) => {
  cy.get('input[name="email"]').type(email)
  cy.get('input[name="senha"]').type(senha)
  cy.contains('button', 'Entrar').click()
})

Cypress.Commands.add('mensagemSucesso', () => {
  cy.get('.alert').should('be.visible')
})
```

E importamos em `cypress/support/e2e.js`:

```javascript
import './commands'
```

---

### 5. Testes Refatorados por Partes

**Parte 1: Hooks**

```javascript
describe('Registrar', () => {
  beforeEach(() => {
    cy.visit('/')
  })
  it('deve criar uma conta com sucesso', () => {
    /* código de cadastro */
  })
  it('Deve realizar o login com o usuário cadastrado', () => {
    /* código de login */
  })
})
```

**Parte 2: Hooks + Custom Commands**

```javascript
describe('Registrar', () => {
  beforeEach(() => {
    cy.visit('/')
  })
  it('deve criar uma conta com sucesso', () => {
    cy.registoComSucesso('QA Cristiano', 'teste-qa@teste.com', 'abc@123')
    cy.mensagemSucesso()
  })
  it('Deve realizar o login com o usuário cadastrado', () => {
    cy.loginComSucesso('teste-qa@teste.com', 'abc@123')
    cy.mensagemSucesso()
  })
})
```

---

### 🪝 Hooks no Cypress

Os **Hooks** no Cypress são funções especiais que permitem executar trechos de código em momentos específicos do ciclo de vida dos testes. Eles ajudam a manter seu código organizado e evitar duplicação.

#### Principais Hooks

- **`before(fn)`**  
  Executa uma única vez **antes** de todos os testes do escopo atual (a suite `describe`).

- **`beforeEach(fn)`**  
  Executa **antes de cada** teste (cada `it`) na suite.

- **`after(fn)`**  
  Executa uma única vez **após** todos os testes do escopo.

- **`afterEach(fn)`**  
  Executa **após cada** teste na suite.

---

#### Exemplo Prático

```javascript
describe('Fluxo de Usuário - Hooks', () => {

  before(() => {
    cy.log('Iniciando testes do fluxo de usuário')
  })

  beforeEach(() => {
    cy.visit('/')
  })

  it('deve criar uma conta com sucesso', () => {
    cy.contains('a', 'Novo usuário?').click()
    cy.get('input[name="nome"]').type('QA Cristiano')
    cy.get('input[name="email"]').type('teste-qa@teste.com')
    cy.get('input[name="senha"]').type('abc@123')
    cy.contains('input', 'Cadastrar').click()
    cy.get('.alert-success').should('be.visible')
  })

  it('deve fazer login com sucesso', () => {
    cy.get('input[name="email"]').type('teste-qa@teste.com')
    cy.get('input[name="senha"]').type('abc@123')
    cy.contains('button', 'Entrar').click()
    cy.get('.alert').should('be.visible')
  })

})
```

---

### 🧰 Recursos Complementares

- :bookmark: [Documentação Cypress](https://docs.cypress.io)
- :open_book: [Frameworks de Teste](./frameworks.md)



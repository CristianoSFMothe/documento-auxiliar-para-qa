# 🧱 Frameworks de Automação de Testes

## 📌 O que é um Framework?

Um **framework** é uma estrutura base composta por ferramentas, bibliotecas e boas práticas que facilita o desenvolvimento de aplicações ou a automação de processos — como é o caso da automação de testes.

No contexto de **Qualidade de Software**, um framework de testes serve para padronizar, organizar e agilizar o processo de escrita, execução e manutenção de testes automatizados.

> Ele oferece componentes reutilizáveis, integração com ferramentas de relatório, suporte a diferentes tipos de teste (UI, API, mobile, etc.) e muito mais.

---

## 💡 Por que utilizar um Framework?

- 🔄 **Reutilização de código**
- 🧹 **Organização da estrutura de testes**
- 🚀 **Agilidade na criação e manutenção**
- 🔗 **Integração com pipelines de CI/CD**
- 📊 **Geração de relatórios de execução**
- 🧪 **Suporte a diferentes níveis de teste**

---

## 🌐 Principais Frameworks de Automação

Divididos por categoria, aqui estão os frameworks mais utilizados no mercado:

### 🔹 **Web**

| Framework           | Linguagem         | Observações                                                           |
| ------------------- | ----------------- | --------------------------------------------------------------------- |
| **Cypress**         | JavaScript        | Foco em testes E2E rápidos, ótima documentação e fácil de configurar. |
| **Playwright**      | JS/TS, Python, C# | Suporte a múltiplos navegadores e múltiplas linguagens.               |
| **Selenium**        | Várias            | Robusto e consolidado no mercado, mas com curva de aprendizado maior. |
| **TestCafe**        | JavaScript        | Não exige WebDriver, execução em paralelo com facilidade.             |
| **Robot Framework** | Python            | Framework genérico com suporte a testes Web, fácil de ler e escrever. |

---

### 🔹 **API**

| Framework            | Linguagem          | Observações                                                                       |
| -------------------- | ------------------ | --------------------------------------------------------------------------------- |
| **Rest Assured**     | Java               | Muito utilizado para testes de API REST em Java.                                  |
| **Supertest**        | JavaScript         | Fácil integração com frameworks Node.js, como Express.                            |
| **Postman + Newman** | Nenhuma específica | Postman para testes manuais/automatizados, Newman para execução via CLI.          |
| **Karate**           | DSL + Java         | Escrita simples, com suporte a API e testes Web.                                  |
| **Cypress**          | JavaScript         | Apesar do foco em Web, também realiza testes de API com facilidade.               |
| **Robot Framework**  | Python + DSL       | Com bibliotecas específicas, realiza testes de API com boa legibilidade.          |
| **JMeter**           | Java               | Focado em testes de carga e performance, mas também usado para testes funcionais. |
| **k6**               | JavaScript-like    | Leve, rápido e ótimo para testes de performance em APIs.                          |

---

### 🔹 **Mobile**

| Framework    | Linguagem   | Observações                                                                |
| ------------ | ----------- | -------------------------------------------------------------------------- |
| **Appium**   | Várias      | Open source, suporta Android e iOS, utiliza WebDriver.                     |
| **Detox**    | JavaScript  | Foco em apps React Native, ótima performance em testes E2E.                |
| **Espresso** | Java/Kotlin | Nativo para Android, mantido pelo Google.                                  |
| **XCUITest** | Swift       | Nativo para iOS, mantido pela Apple.                                       |
| **Maestro**  | DSL         | Foco em testes funcionais e E2E, execução rápida e simples em Android/iOS. |

---

### 🔹 **Desktop**

| Framework        | Linguagem | Observações                                                           |
| ---------------- | --------- | --------------------------------------------------------------------- |
| **WinAppDriver** | C#, Java  | Automação para apps Windows, baseado no WebDriver.                    |
| **Winium**       | C#        | Similar ao Selenium, voltado para aplicações Windows.                 |
| **SikuliX**      | Várias    | Usa reconhecimento de imagem para automatizar qualquer coisa na tela. |

---

## ⚖️ Vantagens e Desvantagens dos Frameworks

| Framework           | Vantagens                                              | Desvantagens                                                  |
| ------------------- | ------------------------------------------------------ | ------------------------------------------------------------- |
| **Cypress**         | Rápido, moderno, fácil de configurar                   | Suporte limitado a múltiplos navegadores                      |
| **Selenium**        | Amplo suporte de linguagem e navegador                 | Pode ser mais lento e complexo de manter                      |
| **Rest Assured**    | Poderoso para testes REST, integração com Java         | Exige conhecimento em Java                                    |
| **Appium**          | Multiplataforma, gratuito                              | Mais difícil de configurar e manter                           |
| **Playwright**      | Testes paralelos, múltiplas linguagens                 | Ainda ganhando adoção em larga escala                         |
| **Robot Framework** | Fácil de aprender, legível, suporte a Web, API, Mobile | Pode ser limitado para testes muito complexos ou customizados |
| **JMeter**          | Excelente para performance, comunidade forte           | Interface menos amigável, curva de aprendizado inicial        |
| **k6**              | Scripts simples, ótimo para CI/CD, muito rápido        | Foco principal é em testes de carga (não funcionais)          |

---

## 🔗 Recursos Complementares

- :open_book: [Documentação da Qualidade](../Documentacao_da_qualidade/README.md)
- :open_book: [Trilhas de Estudos QA](../Trilhas_de_estudos_QA/README.md)

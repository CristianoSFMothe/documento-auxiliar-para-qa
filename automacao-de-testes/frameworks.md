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
  "name": "bugbank",
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

- Escolha entre **E2E** e **Component**
- Neste guia, focaremos em **E2E**

---

### 3. Estrutura Padrão

![estrutura_padrao_cypress](https://github.com/user-attachments/assets/e99a8bdf-2b09-4d1e-b43f-e59dbde81e7f)

---

### 4. Seleção de Navegador

![selecao_browser](https://github.com/user-attachments/assets/262b23f1-3479-4918-8297-16ef59e144ad)

---

### 5. Criar um Novo Arquivo de Teste

![criar_novo_spec_de_teste](https://github.com/user-attachments/assets/d940de72-2498-41bb-93f6-dd21f4192704)

---

### 6. Nomeando o Arquivo `register.cy.js`

![nomear_spec_teste](https://github.com/user-attachments/assets/0beec3df-3da3-42b8-a13b-aeb4436503d2)

---

### 7. Estrutura Básica do Arquivo

![estrutura_basica](https://github.com/user-attachments/assets/de4696d9-85b8-45e3-b857-0b36920431e5)

---

### 8. Primeira Execução

![primeira_execucao](https://github.com/user-attachments/assets/6661fd09-8caf-41d7-9678-3f54e29a24d7)

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

## 🧰 Recursos Complementares

- :bookmark: [Documentação Cypress](https://docs.cypress.io)
- :open_book: [Frameworks de Teste](./frameworks.md)

---

📌 **Este projeto está em construção. Novas seções e exemplos serão adicionados em breve.**

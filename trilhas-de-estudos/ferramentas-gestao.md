## 🧪 Ferramentas de Gestão de Testes

Este documento apresenta uma visão geral das principais ferramentas utilizadas por times de QA para organizar, documentar e acompanhar suas atividades de testes — desde a criação de casos até a execução e análise de resultados.

---

### 📌 **<a href="https://trello.com/" _target="_blank">Trello</a>**

> **Tipo:** Kanban / Gestão visual  
> **Plataforma:** Nuvem (Web, Mobile)  
> **Indicado para:** Pequenos times e projetos enxutos

<br />

O **Trello** é uma ferramenta visual baseada em quadros, listas e cartões. Embora não seja específica para testes de software, é bastante usada por QAs para organizar ciclos de testes, backlog de casos e bugs.

**Recursos úteis para QA:**

- Organização de testes em **listas** e **cartões** com etiquetas e prioridades;
- Criação de **checklists** para validar passos de um caso de teste;
- Atribuição de responsáveis e datas de entrega;
- Integração com ferramentas como Slack, GitHub, Google Drive.

🔸 Simples e prático, mas não possui funcionalidades nativas para testes automatizados ou rastreabilidade.

---

### 🐞 **<a href="https://www.atlassian.com/software/jira" _target="_blank">Jira</a>**

> **Tipo:** Gestão Ágil de Projetos  
> **Plataforma:** Nuvem e Self-hosted  
> **Indicado para:** Times ágeis e grandes organizações

<br />

O **Jira** é amplamente utilizado no desenvolvimento ágil e pode ser transformado em uma plataforma poderosa de QA quando combinado com plugins como **<a href="https://www.getxray.app/" _target="_blank">Xray</a>** ou **<a href="https://www.smartbear.com/product/zephyr/overview/" _target="_blank">Zephyr</a>**.

**Funcionalidades destacadas:**

- **Criação e execução de casos de teste** (com plugins);
- Rastreabilidade entre **requisitos**, **testes**, **bugs** e **deploys**;
- Integração com ferramentas de CI/CD e controle de versão (GitHub, GitLab, Jenkins, etc);
- **Dashboards personalizáveis** para acompanhamento de qualidade.

🔸 Muito completo, mas pode exigir tempo de configuração e custos mais elevados.

---

### 📋 **<a href="https://qase.io/" _target="_blank">Qase.io</a>**

> **Tipo:** Plataforma moderna de Test Management  
> **Plataforma:** Nuvem  
> **Indicado para:** Times que usam testes manuais e automatizados

O **Qase** é uma ferramenta moderna, focada exclusivamente na gestão de testes. Possui uma interface intuitiva e recursos nativos para execução manual e integração com pipelines automatizados.

**Destaques:**

- Criação de suites e casos de teste com versionamento;
- Execução manual ou via **integração com CI/CD**;
- Importação de resultados de testes automatizados (via API ou CLI);
- Relatórios e gráficos de execução em tempo real;
- Integrações com GitHub, Slack, Jira, TestRail, entre outros.

🔸 Ótima escolha para quem busca organização + automação sem complicação.

---

### 🧷 **<a href="https://testlink.org/" _target="_blank">TestLink</a>**

> **Tipo:** Ferramenta open-source de Test Management  
> **Plataforma:** Self-hosted  
> **Indicado para:** Projetos com baixo orçamento e necessidade de personalização

O **TestLink** é uma solução gratuita e de código aberto para gestão de testes. Apesar da interface mais datada, ainda é bastante utilizada por times que precisam de controle detalhado sobre testes e não podem investir em ferramentas pagas.

**Funcionalidades:**

- Gerenciamento de **requisitos**, **casos de teste**, **planos de teste** e **execuções**;
- Integração com **Jenkins**, **Bugzilla**, **Jira**, entre outros;
- Possibilidade de personalização do código-fonte;
- Relatórios exportáveis e histórico de execuções.

🔸 Exige instalação, configuração e manutenção do servidor. Ideal para ambientes internos ou times técnicos.

---

### 📈 Comparativo Rápido

| Ferramenta    | Testes Automatizados | Integração com CI/CD | Nuvem / Local | Facilidade de Uso |
| ------------- | -------------------- | -------------------- | ------------- | ----------------- |
| Trello        | ❌                   | ❌                   | Nuvem         | ⭐⭐⭐⭐☆         |
| Jira + plugin | ✅                   | ✅                   | Nuvem / Local | ⭐⭐⭐☆☆          |
| Qase          | ✅                   | ✅                   | Nuvem         | ⭐⭐⭐⭐☆         |
| TestLink      | ✅ (com configs)     | ✅ (com configs)     | Local         | ⭐⭐☆☆☆           |

---

:open_book: **[Material de Estudo](./ferramentas-de-estudo.md)**

:open_book: **[Ferramentas Testes de API](./ferramentas-teste-api.md)**

:open_book: **[Canais YouTube Ferramenta de Gestão](./canais-youtube-gestao.md)**

:open_book: **[Linguagem Programação](./linguagem-programacao.md)**

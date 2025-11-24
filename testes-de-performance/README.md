## 🧪 Testes de Performance

Os **testes de performance** têm como objetivo avaliar o **comportamento de um sistema sob determinadas condições de carga, uso intensivo ou limite**. Esses testes verificam se o sistema atende aos requisitos de desempenho, como **tempo de resposta, throughput, uso de recursos** e **estabilidade**.

### 📌 Objetivos dos testes de performance:

- Avaliar a **velocidade** com que o sistema responde às requisições.
- Medir o **tempo de carregamento** e **resposta** de APIs e páginas web.
- Verificar o **consumo de CPU, memória e rede** sob diferentes cargas.
- Detectar **gargalos de performance** em diferentes camadas da aplicação.
- Garantir que o sistema seja **escalável** e estável sob crescimento de usuários.

---

### 🔧 Tipos de Testes de Performance:

| Tipo de Teste                 | Descrição                                                                    |
| ----------------------------- | ---------------------------------------------------------------------------- |
| **Teste de Carga**            | Avalia o desempenho sob uma carga esperada de usuários ou requisições.       |
| **Teste de Estresse**         | Verifica a estabilidade do sistema em cenários extremos de carga.            |
| **Teste de Pico (Spike)**     | Analisa a reação do sistema a aumentos repentinos e curtos de carga.         |
| **Teste de Endurance (Soak)** | Verifica o comportamento do sistema durante longos períodos de uso contínuo. |
| **Teste de Escalabilidade**   | Avalia a capacidade do sistema de aumentar desempenho com mais recursos.     |

---

## 🔍 Principais Ferramentas e Frameworks de Teste de Performance

### 1. **Apache JMeter**

- Open source e muito utilizado para testar aplicações web, APIs REST e SOAP.
- Suporta múltiplos protocolos: HTTP, FTP, JDBC, JMS, etc.
- Interface gráfica e possibilidade de execução em linha de comando.
- Suporta testes distribuídos.

👉 Site: **<a href="https://jmeter.apache.org" _target="_blank">Apache JMeter Oficial</a>**

---

### 2. **K6 (by Grafana)**

- Ferramenta moderna e baseada em código JavaScript para testes de carga e performance.
- Foco em testes de APIs e microsserviços.
- Permite fácil integração com CI/CD.
- Excelente suporte a relatórios e visualização no Grafana Cloud.

```js
import http from "k6/http";
import { check } from "k6";

export default function () {
  const res = http.get("https://api.exemplo.com");
  check(res, {
    "status é 200": (r) => r.status === 200,
  });
}
```

👉 Site: \*\*<a href="https://k6.io" _target="_blank">k6</a>

---

### 3. **Locust**

- Ferramenta baseada em Python para testes de carga.
- Permite definir comportamentos de usuários com scripts.
- Interface web para monitoramento em tempo real.
- Boa escolha para times Pythonistas.

👉 Site: **<a href="https://locust.io" _target="_blank">Locust</a>**

---

### 4. **Artillery**

- Framework leve baseado em Node.js para testes de performance de APIs e aplicações web.
- Permite escrita de cenários em YAML ou JS.
- Ótimo para testes rápidos e integração com CI.

```yaml
config:
  target: "https://api.exemplo.com"
  phases:
    - duration: 60
      arrivalRate: 10
scenarios:
  - flow:
      - get:
          url: "/users"
```

👉 Site: **<a href="https://www.artillery.io" _target="_blank">Artillery</a>**

---

### 5. **Gatling**

- Ferramenta baseada em Scala, com foco em desempenho e alta escalabilidade.
- Muito usada em ambientes corporativos e integrações com Jenkins.
- Interface visual (Gatling FrontLine) disponível como produto comercial.

👉 Site: **<a href="https://gatling.io" _target="_blank">Gatling</a>**

---

## 📈 Considerações Finais

Testes de performance são essenciais para garantir a **resiliência e escalabilidade** de aplicações modernas, principalmente em arquiteturas distribuídas, como microsserviços e aplicações em nuvem. A escolha da ferramenta dependerá da **linguagem usada, infraestrutura, tipo de aplicação** e **integrações com o pipeline de CI/CD**.

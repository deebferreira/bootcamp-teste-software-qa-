# ⚙️ Frameworks Ágeis: Scrum e Kanban

Neste tópico são apresentados os principais frameworks utilizados em metodologias ágeis: **Scrum e Kanban**.

Serão abordados seus conceitos, práticas e ferramentas, como **sprints, backlog, estimativas, cerimônias e métricas**, além do funcionamento do fluxo contínuo no Kanban.

O objetivo é entender como esses frameworks organizam o trabalho das equipes e como contribuem para entregas mais rápidas, eficientes e com maior qualidade.

---

# 🌀 Scrum

Scrum é um framework ágil baseado em **iterações chamadas Sprints**.

---

## 📅 Sprint

Período de tempo (1 a 4 semanas) onde um conjunto de funcionalidades é desenvolvido e entregue.

👉 Exemplo:
- Sprint de 2 semanas focada em:
  - Implementar login
  - Criar tela de cadastro
  - Validar autenticação

---

## 📋 Backlog

Lista priorizada de tarefas, histórias e funcionalidades.

- **Product Backlog** → tudo que precisa ser desenvolvido  
- **Sprint Backlog** → itens selecionados para a sprint atual  

👉 Exemplo:

**Product Backlog:**
- Criar login  
- Criar cadastro  
- Recuperação de senha  

**Sprint Backlog (Sprint atual):**
- Criar login  
- Validar login com dados válidos e inválidos  

---

## 🧠 Planning Poker

Técnica usada para estimar esforço das tarefas em grupo.

👉 Exemplo:
- Desenvolvedor A: 3 pontos  
- QA: 5 pontos  
- Desenvolvedor B: 3 pontos  

Após discussão, equipe define: **3 pontos**

---

## 📊 Story Points

Unidade usada para medir esforço considerando:

- Complexidade  
- Tempo  
- Risco  

👉 Exemplo:
- Login simples → 2 pontos  
- Cadastro com validações → 5 pontos  
- Integração com API externa → 8 pontos  

---

## 📉 Burndown Chart

Gráfico que mostra quanto trabalho ainda falta na sprint.

👉 Exemplo:

- Dia 1: 20 pontos restantes  
- Dia 5: 10 pontos restantes  
- Dia 10: 0 pontos (sprint concluída)

Se o gráfico não estiver descendo como esperado → atraso na sprint

---

## 📈 Velocity Chart

Mostra a quantidade de trabalho entregue por sprint.

👉 Exemplo:

- Sprint 1: 20 pontos  
- Sprint 2: 25 pontos  
- Sprint 3: 22 pontos  

👉 Média: ~22 pontos por sprint (capacidade da equipe)

---

## 🔄 Cerimônias Scrum

### 🗓 Daily  
Reunião diária rápida para alinhamento.

👉 Exemplo:
- QA: "Testei login, encontrei 2 bugs"  
- Dev: "Corrigindo bug do cadastro"  

---

### 🔍 Sprint Review  
Demonstração do que foi desenvolvido.

👉 Exemplo:
- Apresentar login funcionando para o PO  
- Validar fluxo completo com stakeholder  

---

### 🔁 Sprint Retrospective  
Reunião para melhoria contínua.

👉 Exemplo:
- Problema: muitos bugs em produção  
- Ação: adicionar mais testes de regressão  

---

# 🧩 Kanban

Kanban é uma metodologia baseada em fluxo contínuo de trabalho.

---

## 📌 Características

- Sem sprints fixas  
- Trabalho contínuo  
- Uso de quadro visual  
- Limite de WIP  

👉 Exemplo de quadro Kanban:

- To Do → In Progress → Testing → Done


---

## 🚧 Limite de WIP

Define quantas tarefas podem estar em andamento ao mesmo tempo.

👉 Exemplo:

- "In Progress" permite no máximo 3 tarefas  
- Se já tiver 3 tarefas → ninguém pode iniciar uma nova  

👉 Benefício:
- Evita sobrecarga  
- Melhora foco da equipe  

---

# ⚖️ Scrum vs Kanban

| Característica | Scrum | Kanban |
|--------------|------|--------|
| Estrutura | Sprints | Fluxo contínuo |
| Planejamento | Fixo por sprint | Contínuo |
| Mudanças | Limitadas durante sprint | A qualquer momento |
| WIP | Não obrigatório | Obrigatório |
| Métricas | Velocity | Lead time / Cycle time |
| Reuniões | Definidas | Opcional |

---

# 🎯 Conclusão

As metodologias ágeis permitem entregar software com mais qualidade, rapidez e flexibilidade.

Elas promovem:

- Colaboração  
- Adaptação  
- Entregas contínuas  
- Foco no usuário  

Para QA, isso significa atuar de forma ativa em todo o ciclo de desenvolvimento, garantindo qualidade desde o início.

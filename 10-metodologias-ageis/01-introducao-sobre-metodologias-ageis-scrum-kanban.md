# 🚀 Metodologias Ágeis

As metodologias ágeis são abordagens de desenvolvimento de software que priorizam **flexibilidade, colaboração e entrega contínua de valor** ao cliente.

Elas surgiram como alternativa aos modelos tradicionais (como o modelo cascata), que eram mais rígidos e lentos para se adaptar a mudanças.

O principal marco das metodologias ágeis é o **Manifesto Ágil**, criado em 2001.

---

# ⚖️ Ágil vs Modelo Tradicional (Clássico)

| Característica | Modelo Tradicional (Cascata) | Metodologia Ágil |
|--------------|-----------------------------|------------------|
| Planejamento | Extenso e fixo | Adaptável e contínuo |
| Mudanças | Difíceis e custosas | Bem-vindas |
| Entregas | No final do projeto | Contínuas |
| Testes | Após desenvolvimento | Durante todo o processo |
| Comunicação | Formal e documental | Colaborativa |
| Foco | Processo | Valor entregue |

---

# 📜 Manifesto Ágil

## 💡 4 Valores do Manifesto Ágil

### 1️⃣ Indivíduos e interações mais que processos e ferramentas

Valoriza a comunicação entre pessoas acima de processos rígidos.

Na prática, isso significa que a colaboração entre QA, desenvolvedores e Product Owner é mais importante do que seguir processos engessados.

---

### 2️⃣ Software em funcionamento mais que documentação abrangente

O foco é entregar software que funcione, não apenas documentação.

Isso reforça que validar o sistema funcionando é mais importante do que apenas escrever casos de teste sem execução.

---

### 3️⃣ Colaboração com o cliente mais que negociação de contratos

O cliente participa ativamente do desenvolvimento.

Validações são feitas em conjunto com stakeholders, permitindo feedback constante e ajustes rápidos nas funcionalidades.

---

### 4️⃣ Responder a mudanças mais que seguir um plano  

Mudanças são bem-vindas, mesmo em fases avançadas.

Por isso, testes precisam se adaptar rapidamente a novos requisitos, e a regressão contínua se torna essencial.

---

# 🧠 12 Princípios Ágeis

## 1️⃣ Satisfação do cliente com entregas contínuas

Entregar valor constantemente é prioridade, com releases frequentes e validação contínua das funcionalidades.

---

## 2️⃣ Aceitar mudanças de requisitos

Mudanças fazem parte do processo e devem ser incorporadas rapidamente, exigindo atualização constante dos testes e, muitas vezes, apoio de automação.

---

## 3️⃣ Entregar software frequentemente

O sistema deve ser entregue em ciclos curtos, o que exige execução frequente de testes e atenção especial à regressão.

---

## 4️⃣ Colaboração diária entre equipes

A comunicação constante entre QA, desenvolvedores e PO facilita o entendimento dos requisitos e reduz erros.

---

## 5️⃣ Pessoas motivadas e confiáveis

Equipes capacitadas e com autonomia tendem a produzir melhores resultados, incluindo maior qualidade nos testes e investigações mais profundas.

---

## 6️⃣ Comunicação direta

A troca direta de informações reduz ruídos e acelera a resolução de problemas, como bugs e dúvidas sobre comportamento do sistema.

---

## 7️⃣ Software funcional como métrica principal

O progresso é medido pelo funcionamento do sistema, não apenas por tarefas concluídas ou documentação produzida.

---

## 8️⃣ Ritmo sustentável

Manter um ritmo constante evita sobrecarga e garante que os testes sejam bem planejados e executados sem acúmulo.

---

## 9️⃣ Excelência técnica

Boas práticas técnicas aumentam a qualidade e a agilidade, incluindo testes bem estruturados, reutilizáveis e automatizados.

---

## 🔟 Simplicidade

Fazer apenas o necessário evita complexidade desnecessária, inclusive na criação de casos de teste.

---

## 1️⃣1️⃣ Times auto-organizados

As equipes têm autonomia para decidir como trabalhar, incluindo estratégias de teste e melhorias no processo.

---

## 1️⃣2️⃣ Melhoria contínua

A equipe deve evoluir constantemente, ajustando processos, aprendendo com erros e aprimorando a qualidade do produto.

---

# 👥 Equipes Ágeis

Equipes ágeis são geralmente **multidisciplinares** e auto-organizadas.

## 🔹 Composição comum

- Product Owner (PO)  
- Scrum Master  
- Desenvolvedores  
- QA (Quality Assurance)  

---

## 🧪 O papel do QA na equipe ágil

O QA não é apenas um testador — ele participa de todo o processo.

### Responsabilidades:

- Participar do refinement e planejamento  
- Escrever cenários de teste  
- Executar testes manuais e automatizados  
- Reportar bugs  
- Validar critérios de aceitação  
- Trabalhar junto com devs e PO  
- Garantir qualidade contínua  

---

# 📦 Conceitos importantes

## 📌 MVP (Minimum Viable Product)

Produto mínimo com funcionalidades essenciais para entrega rápida e validação.

👉 Objetivo:
- Validar uma ideia com o menor esforço possível  
- Coletar feedback real dos usuários  

### Exemplo

Um sistema de reserva de voos completo teria:
- login
- busca de voos
- pagamento
- histórico de reservas

Um **MVP** poderia ser apenas:
- busca de voos
- seleção básica
- simulação de reserva (sem pagamento real)

---

## 📌 User Story

Descrição simples de uma funcionalidade do ponto de vista do usuário.

Formato comum:

- Como [tipo de usuário], quero [ação], para [benefício].

### Exemplo

- Como usuário, quero fazer login para acessar minha conta.


👉 Critérios de aceitação (exemplo):

- Deve permitir login com email e senha válidos  
- Deve exibir erro para credenciais inválidas  
- Deve redirecionar para a dashboard após login  

👉 Em testes:
- Cada user story gera cenários de teste  
- Base para criação de casos de teste  

---

## 📌 Épicos

Grandes funcionalidades que podem ser divididas em várias user stories.

### Exemplo

**Épico:** Sistema de autenticação

User Stories:
- Login com email e senha  
- Recuperação de senha  
- Login com redes sociais  

---

## 📌 Temas

Agrupamento de épicos relacionados.

### Exemplo

**Tema:** Autenticação e Segurança

Épicos:
- Login  
- Cadastro  
- Recuperação de senha  

---

# 🌀 Scrum

Scrum é um framework ágil baseado em **iterações chamadas Sprints**.

---

## 📅 Sprint

Período de tempo (geralmente 1 a 4 semanas) onde o trabalho é realizado.

👉 Exemplo:
- Sprint de 2 semanas com foco em "Login e Cadastro"

---

## 📋 Backlog

Lista priorizada de tarefas, histórias e funcionalidades.

### Tipos:

- Product Backlog → tudo que precisa ser feito  
- Sprint Backlog → itens selecionados para a sprint  

---

## 🧠 Planning Poker

Técnica usada para estimar tarefas com base em consenso da equipe.

👉 Exemplo:
- Cada membro escolhe um valor (1, 2, 3, 5, 8...)  
- Todos revelam ao mesmo tempo  
- Discussão até chegar em consenso  

---

## 📊 Story Points

Unidade de medida de esforço baseada em:

- Complexidade  
- Tempo  
- Risco  

👉 Exemplo:
- Login simples → 2 pontos  
- Integração com pagamento → 8 pontos  

---

## 📉 Burndown Chart

Gráfico que mostra quanto trabalho ainda falta na sprint.

👉 Uso:
- Acompanhar progresso diário  
- Identificar atrasos  

---

## 📈 Velocity Chart

Mostra quantos story points a equipe entrega por sprint.

👉 Uso:
- Prever capacidade futura  
- Planejar próximas sprints  

---

## 🔄 Cerimônias Scrum

### 🗓 Daily

Reunião diária rápida (15 min)

Cada membro responde:
- O que fiz ontem?
- O que farei hoje?
- Existe algum bloqueio?

---

### 🔍 Sprint Review

Apresentação do que foi entregue.

👉 Exemplo:
- Mostrar funcionalidade de login funcionando  

---

### 🔁 Sprint Retrospective

Reunião para melhoria contínua.

👉 Exemplo:
- O que funcionou bem?  
- O que pode melhorar?  

---

# 🧩 Kanban

Kanban é uma metodologia baseada em fluxo contínuo de trabalho.

---

## 📌 Características

- Sem sprints fixas  
- Trabalho contínuo  
- Uso de quadro visual  
- Limite de WIP (Work in Progress)  

---

## 🚧 Limite de WIP

Define quantas tarefas podem estar em andamento ao mesmo tempo.

### Exemplo

- Coluna "Em andamento" permite no máximo 3 tarefas  
- Se atingir o limite, ninguém pode puxar novas tarefas  

👉 Benefício:
- Evita sobrecarga  
- Melhora foco e produtividade  

---

# ⚖️ Scrum vs Kanban

| Característica | Scrum | Kanban |
|--------------|------|--------|
| Estrutura | Iterações (Sprints) | Fluxo contínuo |
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

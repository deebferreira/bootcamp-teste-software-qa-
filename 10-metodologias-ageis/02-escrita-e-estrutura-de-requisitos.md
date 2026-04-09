# ✍️ Escrita e Estrutura de Requisitos

Este tópico aborda como os requisitos são definidos e organizados dentro de um contexto ágil.

Aqui são apresentados conceitos fundamentais como **User Stories, INVEST e BDD**, que ajudam a garantir que os requisitos sejam claros, bem estruturados e testáveis.

Além disso, são exploradas as formas de organização desses requisitos, como **épicos e temas**, permitindo uma melhor gestão do backlog e facilitando o trabalho da equipe de desenvolvimento e QA.

---

## 👥 Equipes Ágeis

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

- Participar do refinamento e planejamento  
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

## 🧠 INVEST (Qualidade das User Stories)

A técnica **INVEST** garante que as histórias sejam bem escritas.

- **I — Independent (Independente)**  
Exemplo: Login pode ser testado sem depender do cadastro.

- **N — Negotiable (Negociável)**  
Exemplo: Forma de login pode mudar (email, Google, Facebook).

- **V — Valuable (Valiosa)**  
Exemplo: Login agrega valor ao usuário.

- **E — Estimable (Estimável)**  
Exemplo: Login é estimável, sistema completo não.

- **S — Small (Pequena)**  
Exemplo: Login cabe em uma sprint.

- **T — Testable (Testável)**  
Exemplo: Deve permitir login válido e erro para inválido.

---

## 🧪 BDD (Behavior Driven Development)

BDD descreve o comportamento do sistema de forma clara, usando linguagem próxima do negócio.

Formato padrão:

- Given (Dado)
- When (Quando)
- Then (Então)


### Exemplo

User Story:
- Como usuário, quero fazer login para acessar minha conta.

BDD:

- Given que o usuário está na tela de login
- When ele insere credenciais válidas
- Then o sistema deve autenticar o usuário

- Given que o usuário insere credenciais inválidas
- When ele tenta fazer login
- Then o sistema deve exibir erro

---

# 📚 Organização de Requisitos

## 📌 Épicos

Grandes funcionalidades divididas em várias histórias.

**Exemplo:** Sistema de autenticação

---

## 📌 Temas

Agrupamento de épicos relacionados.

**Exemplo:** Segurança e autenticação

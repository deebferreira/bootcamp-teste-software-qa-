# 🔄 Teste de Transição de Estado (State Transition Testing)

O **Teste de Transição de Estado** é uma técnica de teste de caixa preta utilizada quando o sistema possui **estados bem definidos** e o comportamento depende do **estado atual ou do histórico de ações**.

Diferente de outras técnicas que focam apenas nas entradas e saídas, aqui o foco está na **mudança de estado do sistema**.

---

## 🧠 Conceitos Fundamentais

### 🔹 Estado (State)

Um estado representa a condição atual do sistema em determinado momento.

Exemplos:
- Conta ativa
- Conta bloqueada
- Usuário logado
- Sessão expirada
- Pedido finalizado

---

### 🔹 Transição (Transition)

É a mudança de um estado para outro, causada por uma ação ou evento.

Exemplos:
- 3 tentativas de senha errada → Conta bloqueada
- Login correto → Usuário autenticado
- Cancelar pedido → Pedido cancelado

---

### 🔹 Estado Inicial

É o ponto de partida do sistema.

Exemplo:
- Tela de login
- Carrinho vazio
- Sistema desligado

---

### 🔹 Estado Final / Dead State

Um **estado morto** é aquele que não possui saída.

Exemplo:
- Cartão retido no caixa eletrônico
- Conta permanentemente bloqueada

---

## 🎯 Quando usar Teste de Transição de Estado?

Utilize essa técnica quando:

- O sistema possui limite de tentativas
- O comportamento depende do histórico
- Existem bloqueios automáticos
- Há fluxos sequenciais
- O sistema muda de comportamento após determinada ação

---

# 📌 Exemplo 1 — Login com Bloqueio

### Regra de negócio:

Após 3 tentativas incorretas de senha, a conta deve ser bloqueada.

---

### Estados:

1. Conta ativa
2. Conta bloqueada

---

### Transições:

- 1 senha errada → continua ativa
- 2 senhas erradas → continua ativa
- 3 senhas erradas → bloqueada
- Conta bloqueada → não permite login

---

### Casos de Teste Importantes:

- Errar 2 vezes → ainda deve permitir tentativa
- Errar 3 vezes → deve bloquear
- Errar 3 vezes e depois inserir senha correta → deve continuar bloqueada

👉 Aqui o histórico é essencial.

---

# 📌 Exemplo 2 — Carrinho de Compras

### Estados:

1. Carrinho vazio
2. Carrinho com itens
3. Pedido finalizado
4. Pedido cancelado

---

### Transições possíveis:

- Adicionar item → muda para "Carrinho com itens"
- Finalizar compra → muda para "Pedido finalizado"
- Cancelar pedido → muda para "Pedido cancelado"

---

### Testes importantes:

- Finalizar compra com carrinho vazio
- Cancelar pedido já finalizado
- Adicionar item após pedido cancelado

Algumas transições devem ser bloqueadas pelo sistema.

---

# 📌 Exemplo 3 — Caixa Eletrônico (ATM)

### Estados:

1. Inserir PIN
2. Segunda tentativa
3. Terceira tentativa
4. Cartão retido (Dead State)
5. Conta acessada

---

### Transições:

- PIN correto → acesso liberado
- PIN incorreto → próxima tentativa
- 3 tentativas incorretas → cartão retido

Após cartão retido, não há retorno.

---

# 📊 Tipos de Cobertura

### 1️⃣ Cobertura de Estados
Garantir que cada estado seja testado pelo menos uma vez.

### 2️⃣ Cobertura de Transições
Testar cada mudança possível entre estados.

### 3️⃣ Cobertura de Sequência
Testar caminhos completos (fluxos do início ao fim).

---

# 🔎 Diferença entre Tabela de Decisão e Transição de Estado

| Tabela de Decisão | Transição de Estado |
|------------------|--------------------|
| Foca em combinações de entrada | Foca em mudança de estado |
| Não depende do histórico | Depende do histórico |
| Baseada em lógica booleana | Baseada em fluxo sequencial |
| Ideal para regras complexas | Ideal para sistemas com estados |

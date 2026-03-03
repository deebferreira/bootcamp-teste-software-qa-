# 🔄 Teste de Pares (Pairwise Testing)

O **Teste de Pares (Pairwise Testing)**, também conhecido como **All-Pairs Testing**, é uma técnica de teste de caixa preta utilizada para reduzir o número de combinações de teste quando existem múltiplos parâmetros com vários valores possíveis.

A ideia principal é:

> Garantir que todas as combinações possíveis entre **pares de variáveis** sejam testadas pelo menos uma vez.

---

# 📌 Por que usar Teste de Pares?

Quando um sistema possui muitas variáveis, o número total de combinações cresce exponencialmente.

Exemplo:

Se temos 3 parâmetros com 3 valores cada:

- 3 × 3 × 3 = 27 combinações

Se tivermos 5 parâmetros com 4 valores cada:

- 4⁵ = 1024 combinações

Testar todas as combinações se torna inviável.

O Pairwise reduz drasticamente essa quantidade mantendo boa cobertura.

---

# 🧠 Conceito Principal

Estudos mostram que a maioria dos defeitos ocorre pela interação entre **dois fatores**, e não entre três ou mais ao mesmo tempo.

Por isso, ao garantir que todos os **pares possíveis de valores** sejam testados, conseguimos encontrar a maior parte dos defeitos com menos testes.

---

# 📊 Exemplo 1 – Filtros de Curso (Plataforma Educacional)

Imagine um sistema com os seguintes filtros:

- ⭐ Avaliação: 3.0+, 4.0+, 4.5+
- ⏳ Duração: 0–1h, 1–3h, 3–6h
- 🎓 Nível: iniciante, intermediário, expert

Total completo:

- 3 × 3 × 3 = 27 combinações


Com Pairwise, podemos reduzir para algo como:

| Avaliação | Duração | Nível |
|-----------|----------|--------|
| 3.0+      | 0–1h     | iniciante |
| 4.0+      | 1–3h     | expert |
| 4.5+      | 3–6h     | intermediário |
| 3.0+      | 1–3h     | expert |
| 4.0+      | 3–6h     | iniciante |
| 4.5+      | 0–1h     | expert |

Esses testes garantem que todas as combinações entre pares sejam cobertas.

---

# 📊 Exemplo 2 – Teste de Compatibilidade

Sistema web com:

- 🌐 Navegador: Chrome, Firefox, Edge
- 💻 Sistema Operacional: Windows, Mac
- 👤 Tipo de Usuário: Admin, Comum

Total completo:

- 3 × 2 × 2 = 12 combinações


Com Pairwise, é possível reduzir para aproximadamente 6–8 testes, mantendo cobertura entre todos os pares:

- Chrome + Windows
- Chrome + Mac
- Firefox + Windows
- Edge + Mac
- Admin + Chrome
- Comum + Firefox
- etc.

---

# 🛠 Como aplicar na prática

## 1️⃣ Identificar os fatores
Liste todas as variáveis que influenciam o comportamento do sistema.

## 2️⃣ Listar os valores possíveis
Defina claramente todos os valores válidos para cada fator.

## 3️⃣ Gerar combinações pairwise
Você pode usar ferramentas como:

- Microsoft PICT
- Pairwise Pict Online
- Ferramentas de automação combinatória

Essas ferramentas geram automaticamente o conjunto mínimo de testes.

---

# 📌 Quando usar Teste de Pares?

Use quando:

- Existem muitos parâmetros combináveis
- Testar todas as combinações é inviável
- O sistema possui múltiplas configurações
- É necessário otimizar tempo e esforço de teste

Muito comum em:

- Testes de compatibilidade
- Filtros de busca
- Configurações de sistema
- Planos de assinatura
- Sistemas com múltiplas permissões

---

# 🔍 Comparação com outras técnicas

| Técnica | Foco |
|----------|-------|
| Partição de Equivalência | Grupos de valores |
| Análise de Valor Limite | Valores extremos |
| Tabela de Decisão | Regras de negócio |
| Transição de Estado | Mudança de status |
| Pairwise | Combinação entre variáveis |

---

# 🎯 Vantagens

- Reduz drasticamente o número de testes
- Mantém boa cobertura
- Muito eficiente em cenários combinatórios
- Amplamente utilizado em grandes empresas

---

# ⚠️ Limitações

- Não cobre combinações de três ou mais fatores simultaneamente
- Pode não encontrar defeitos causados por interações muito complexas
- Não substitui outras técnicas (deve ser usado em conjunto)

---

# 🧩 Conclusão

O Teste de Pares é uma técnica poderosa para lidar com múltiplas combinações de variáveis de forma eficiente.

Ele permite reduzir esforço de teste sem perder qualidade, sendo amplamente utilizado em projetos reais, especialmente em testes de configuração e compatibilidade.


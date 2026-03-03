# 🧠 Teste com Tabela de Decisão (Decision Table Testing)

O **Teste com Tabela de Decisão** é uma técnica de teste de caixa preta utilizada quando o sistema possui **múltiplas condições** que influenciam diretamente o resultado.

Essa técnica ajuda a mapear todas as combinações possíveis de entradas (condições) e seus respectivos resultados (ações).

---

## 📌 Conceito

Uma tabela de decisão é composta por:

- **Condições (Inputs)** → regras ou perguntas (ex: verdadeiro/falso)
- **Ações (Outputs)** → resultado esperado
- **Regras** → combinações possíveis entre condições

---

## 🧮 Quantidade de combinações

A quantidade de cenários possíveis é calculada por:

- 2^n

Onde:
- `n` = número de condições (perguntas)

### Exemplos:

- 2 condições → `2² = 4 cenários`
- 3 condições → `2³ = 8 cenários`
- 4 condições → `2⁴ = 16 cenários`

👉 Quanto mais condições, mais combinações!

---

## 📊 Exemplo clássico:

### 🎯 Regra de negócio:
Para ganhar desconto:
- Deve gastar mais de **$100**
- Deve ter **assinatura Gold**

---

## 🧾 Tabela de decisão

| Regra | Compra > 100 | Assinatura Gold | Resultado |
|------|-------------|----------------|----------|
| 1    | Sim         | Sim            | Desconto ✅ |
| 2    | Sim         | Não            | Sem desconto ❌ |
| 3    | Não         | Sim            | Sem desconto ❌ |
| 4    | Não         | Não            | Sem desconto ❌ |

---

## 🧪 Casos de teste gerados

1. Compra = 150 / Gold = Sim → Deve aplicar desconto  
2. Compra = 150 / Gold = Não → Não deve aplicar desconto  
3. Compra = 50 / Gold = Sim → Não deve aplicar desconto  
4. Compra = 50 / Gold = Não → Não deve aplicar desconto  

---

## 🎯 Quando usar essa técnica?

Use Tabela de Decisão quando:

- Existem **múltiplas regras de negócio**
- O comportamento depende de **combinações de condições**
- Existem muitas variações de entrada
- Você quer evitar esquecer cenários

---

## ⚠️ Vantagens

- Garante **cobertura completa**
- Evita cenários esquecidos
- Organiza regras complexas
- Muito útil para sistemas com lógica de negócio forte

---

## 🚨 Pontos de atenção

- Pode crescer rapidamente (muitas combinações)
- Nem todas as combinações são válidas (podem ser descartadas)
- Pode ser necessário simplificar

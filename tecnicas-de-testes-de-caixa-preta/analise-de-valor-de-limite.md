## Análise de Valor de Limite (Boundary Value Analysis - BVA)

A **Análise de Valor de Limite (BVA)** é uma técnica de teste de **caixa preta** que foca nos **valores extremos (limites)** de uma entrada.

Essa técnica parte do princípio de que a maioria dos defeitos ocorre **nos limites dos dados**, e não nos valores intermediários.

---

## 🎯 Objetivo

- Identificar falhas nos limites de entrada  
- Garantir que o sistema trata corretamente valores extremos  
- Complementar a Partição de Equivalência  

---

## 🧠 Conceito-chave

> Os erros geralmente ocorrem nos limites. Por isso, devemos testar valores próximos ao mínimo e ao máximo permitido.

---

## 📊 Como aplicar BVA

Dado um intervalo de valores, devemos testar:

- Valor abaixo do mínimo (mínimo - 1)  
- Valor mínimo  
- Valor acima do mínimo (mínimo + 1)  
- Valor abaixo do máximo (máximo - 1)  
- Valor máximo  
- Valor acima do máximo (máximo + 1)  

---

## 📊 Exemplo 1: Idade (Regra simples)

### Regra:
- Idade mínima: 13 anos  
- Idade máxima: 100 anos  

---

### Casos de teste (BVA):

- 12 → inválido ❌ (abaixo do mínimo)
- 13 → válido ✅ (mínimo)
- 14 → válido ✅ (acima do mínimo)

- 99 → válido ✅ (abaixo do máximo)
- 100 → válido ✅ (máximo)
- 101 → inválido ❌ (acima do máximo)


---

## 📅 Exemplo 2: Idade baseada em Data de Nascimento

Na prática, muitos sistemas não pedem a idade diretamente, mas sim a **data de nascimento**.

### Cenário:
- Data atual: Janeiro de 2026  
- Idade mínima: 13 anos  

---

### Casos de teste:

- Jan/2013 → válido ✅ (usuário tem 13 anos)

- Fev/2013 → inválido ❌ (usuário ainda não completou 13 anos)

- Jan/2012 → válido ✅ (acima do limite mínimo)


---

### 🧠 Explicação

O sistema calcula a idade com base em:

- idade = data atual - data de nascimento


Por isso, pequenas diferenças de data podem mudar completamente o resultado.

---

## 🔐 Exemplo 3: Senha

### Regra:
- Mínimo de 6 caracteres  

---

### Casos de teste (BVA):

- 5 caracteres → inválido ❌
- 6 caracteres → válido ✅
- 7 caracteres → válido ✅


---

## 🧠 Por que BVA é importante?

- Detecta erros em validações de entrada  
- Evita falhas em cálculos (ex: idade, datas)  
- Garante comportamento correto nos limites  

---

## 🔄 Relação com Partição de Equivalência

| Técnica | Foco |
|--------|------|
| Partição de Equivalência | Grupos de dados |
| BVA | Limites dos dados |

---

### 💡 Exemplo combinado:

- Partição válida: idade entre 13 e 100  
- BVA: testa 12, 13, 14, 99, 100, 101  

---

## 📌 Quando usar BVA

Utilize essa técnica em:

- Validação de idade  
- Campos com limite mínimo/máximo  
- Senhas  
- Campos numéricos (preço, quantidade)  
- Datas  
- Tamanho de texto  

---

## ⚠️ Erro comum

Testar apenas valores válidos:

- Idade = 25 ✅

❌ Isso não testa os limites.

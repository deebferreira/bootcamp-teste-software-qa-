## Partição de Equivalência (Equivalence Partitioning)

A **Partição de Equivalência** é uma técnica de teste de **caixa preta** utilizada para reduzir a quantidade de casos de teste sem perder cobertura.

A ideia principal é dividir os dados de entrada em **grupos (partições)** onde todos os valores dentro de um mesmo grupo se comportam da mesma forma.

Em vez de testar todos os valores possíveis, testamos apenas **um valor representativo de cada partição**.

---

## 🎯 Objetivo

- Reduzir o número de testes  
- Aumentar a eficiência da validação  
- Garantir cobertura funcional adequada  

---

## 🧠 Conceito-chave

> Se um valor de uma partição funciona (ou falha), todos os outros valores daquela partição terão o mesmo comportamento.

---

## 📊 Exemplo 1: Idade (Cadastro)

### Regra:
- Idade mínima: 13 anos  
- Idade máxima: 120 anos  

### Partições:

- ❌ Idade menor que 13  
- ✅ Idade entre 13 e 120  
- ❌ Idade maior que 120  

### Casos de teste:

- Idade = 10 → inválido ❌
- Idade = 25 → válido ✅
- Idade = 130 → inválido ❌

---

## 🔐 Exemplo 2: Senha

### Regra:
- Mínimo de 6 caracteres  
- Deve conter letras e números  

### Partições:

- ❌ Senha com menos de 6 caracteres  
- ❌ Senha sem números  
- ❌ Senha sem letras  
- ✅ Senha válida (atende todos os critérios)  

### Casos de teste:

- "A2#" → inválido (curta) ❌
- "abcdef" → inválido (sem número) ❌
- "123456" → inválido (sem letra) ❌
- "abc123" → válido ✅

---

## 🔎 Exemplo 3: Busca (Funcionalidade de Pesquisa)

### Regra:
Sistema deve retornar resultados relevantes para a busca

### Partições:

- ✅ Texto correto  
- ✅ Texto parcial  
- ✅ Texto com erro de digitação  
- ❌ Campo vazio  
- ❌ Apenas espaços  
- ❌ Caracteres inválidos  

### Casos de teste:

- "selenium" → válido ✅
- "selen" → válido ✅
- "seleniun" → válido ✅

- "" → inválido ❌
- " " → inválido ❌
- "@#$%" → inválido ❌

---

## 📌 Quando usar Partição de Equivalência

Essa técnica é muito utilizada em **testes funcionais**, principalmente quando:

### ✔ Validação de campos de entrada
- Idade  
- Senha  
- E-mail  
- Telefone  

### ✔ Regras de negócio com intervalos
- Faixa etária  
- Limite de valores (ex: preço, quantidade)  

### ✔ Formatos de dados
- E-mails válidos e inválidos  
- Números de telefone  
- Strings  

### ✔ Funcionalidades de busca
- Busca por texto  
- Busca parcial  
- Tratamento de erros de digitação  

---

## ⚠️ Observação Importante

A Partição de Equivalência **não testa os limites exatos dos valores**.

Para isso, utilizamos outra técnica.

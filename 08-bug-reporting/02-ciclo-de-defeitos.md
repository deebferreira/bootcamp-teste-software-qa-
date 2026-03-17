# 🐞 Ciclo de Defeitos (Bug Life Cycle)

O **Ciclo de Defeitos** representa o caminho que um bug percorre desde a sua identificação até a sua resolução final.

Esse processo envolve diferentes membros da equipe, como:

- QA (testadores)
- Desenvolvedores
- Gerentes de projeto

O objetivo é garantir que todos os defeitos sejam **registrados, analisados, corrigidos e validados corretamente**.

---

# 🔄 Fluxo do Ciclo de Defeitos

```
New → Assigned → Open → Fixed → Retest → Verified
                     ↘ Reopened (se falhar)
```

---

# 📊 Etapas do Ciclo de Defeitos

## 🆕 New (Novo)

O bug foi identificado e registrado pelo QA.

- Ainda não foi analisado
- Aguarda triagem

---

## 📌 Assigned (Atribuído)

O bug é atribuído a um desenvolvedor responsável pela correção.

---

## 🔓 Open (Aberto)

O desenvolvedor começa a analisar o problema.

- Investigação do defeito
- Identificação da causa raiz

---

## ❌ Possíveis classificações do bug

Durante a análise, o bug pode seguir outros caminhos:

- **Duplicate** → Já existe outro bug registrado com o mesmo problema  
- **Rejected** → O bug não é válido  
- **Deferred** → Correção adiada para outra versão  
- **Not a Bug** → Comportamento esperado do sistema  

---

## 🔧 Fixed (Corrigido)

O desenvolvedor implementou a correção do defeito.

- O código foi ajustado
- A solução foi aplicada

---

## ⏳ Pending Retest (Aguardando Reteste)

O bug está pronto para ser validado novamente pelo QA.

---

## 🔁 Retest (Reteste)

O QA executa novamente os testes para verificar se o problema foi corrigido.

---

## 🔄 Reopened (Reaberto)

Se o bug ainda existir ou não tiver sido corrigido corretamente:

- Ele é reaberto
- Retorna para o desenvolvedor

---

## ✅ Verified (Verificado)

O QA confirma que o bug foi corrigido com sucesso.

- O comportamento está correto
- O defeito não ocorre mais

---

# 📌 Importância do Ciclo de Defeitos

O ciclo de defeitos é essencial porque:

- Garante rastreabilidade dos bugs  
- Evita que defeitos sejam esquecidos  
- Organiza o fluxo de trabalho  
- Melhora a comunicação entre QA e desenvolvedores  
- Aumenta a qualidade do software  

---

# 🎯 Conclusão

O **Bug Life Cycle** é uma parte fundamental do processo de testes.

Seguir esse fluxo corretamente garante que os defeitos sejam tratados de forma estruturada, contribuindo para um produto mais estável e confiável.

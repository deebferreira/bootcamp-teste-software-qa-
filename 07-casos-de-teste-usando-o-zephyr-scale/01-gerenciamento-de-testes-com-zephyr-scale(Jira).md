# 🧪 Gerenciamento de Testes com Zephyr Scale (Jira)

O **Zephyr Scale** é uma ferramenta de **gerenciamento de testes (Test Management)** integrada ao **Jira**.  
Ele permite que equipes de QA criem, organizem, executem e monitorem testes diretamente dentro do ambiente do Jira.

Com o Zephyr Scale é possível:

- Criar **casos de teste**
- Organizar testes em **pastas**
- Criar **ciclos de teste**
- Executar testes e registrar **PASS / FAIL**
- Criar testes utilizando **BDD**
- Utilizar **datasets**
- Gerar **relatórios de execução**
- Integrar testes com **histórias e tarefas do Jira**

Essa integração permite que todo o fluxo de desenvolvimento e testes fique **centralizado em uma única plataforma**.

---

# 📦 Como adicionar o Zephyr Scale ao Jira

Para utilizar o Zephyr Scale é necessário instalar o plugin no Jira.

### 1️⃣ Acessar o Atlassian Marketplace

No Jira, navegue até:

```
Settings → Apps → Find new apps
```

ou acesse diretamente o **Atlassian Marketplace**.

---

### 2️⃣ Buscar pelo plugin

Pesquise por:

```
Zephyr Scale Test Management for Jira
```

---

### 3️⃣ Instalar o plugin

Clique em:

```
Install
```

Após a instalação, uma nova aba chamada **Zephyr** será adicionada ao seu projeto no Jira.

---

### 4️⃣ Acessar o Zephyr no projeto

Dentro do projeto Jira, você verá novas seções:

```
Zephyr
├── Casos de Teste
├── Ciclos de Teste
├── Planos de Teste
└── Relatórios
```

Essas áreas são utilizadas para organizar e executar os testes.

---

# 🧾 Como criar um Caso de Teste no Zephyr

Para criar um caso de teste:

### 1️⃣ Acessar

```
Zephyr → Casos de Teste
```

---

### 2️⃣ Criar novo teste

Clique em:

```
Novo caso de teste
```

---

### 3️⃣ Preencher os campos principais

**Name**

Título do teste.

Exemplo:

- Validar login com e-mail e senha válidos.

---

**Objective**

Objetivo do teste.

Exemplo:

- Garantir que o usuário consiga acessar o sistema utilizando credenciais válidas.

---

**Precondition**

Condições necessárias antes da execução do teste.

Exemplo:

- O usuário deve possuir uma conta registrada no sistema.

---

### 4️⃣ Adicionar Test Script (passos do teste)

Exemplo:

| Step | Action | Expected Result |
|-----|------|------|
|1|Acessar a página de login|Página de login é exibida|
|2|Inserir e-mail válido|Campo aceita valor|
|3|Inserir senha válida|Campo aceita valor|
|4|Clicar em login|Usuário é autenticado|

---

# 🔁 Como criar um Ciclo de Teste

O **Test Cycle** é utilizado para **executar um conjunto de testes**.

Exemplo: testes de uma sprint ou release.

### Criar ciclo de teste

```
Zephyr → Ciclos de Teste
```

Clique em:

```
Criar Ciclo de Teste
```

---

### Preencher informações

**Name**

Login Tests – Sprint 1

**Objective**

- Executar testes relacionados à funcionalidade de login.

---

### Adicionar casos de teste ao ciclo

Clique em:

```
Add Test Case
```

Selecione os testes que deseja executar.

---

### Executar testes

Durante a execução você poderá marcar o resultado do teste como:

```
PASS
FAIL
BLOCKED
```

Também é possível registrar o **resultado real do teste**.

---

# 🧩 BDD no Zephyr (Behavior Driven Development)

BDD é uma abordagem de testes baseada em **comportamento do sistema**.

Em vez de descrever apenas passos técnicos, o teste é escrito em uma linguagem mais próxima do negócio.

O formato mais comum utiliza **Gherkin**.

Estrutura:

```
Given
When
Then
```

---

### Exemplo de BDD

```
Feature: Login do usuário

Scenario: Login com credenciais válidas

Given que o usuário possui uma conta registrada
When ele insere um e-mail válido
And insere uma senha válida
And clica no botão de login
Then o sistema autentica o usuário com sucesso
```

---

### Vantagens do BDD

- Facilita a comunicação entre **QA, desenvolvedores e stakeholders**
- Testes ficam mais **legíveis**
- Permite integração com ferramentas de automação

---

# 📊 Datasets no Zephyr

Datasets permitem reutilizar **dados de teste** dentro de vários casos de teste.

Isso evita repetir informações manualmente.

Exemplo de dataset:

| email | senha |
|------|------|
|user1@email.com|Senha123|
|user2@email.com|Senha456|

---

### Utilização em um teste

Em vez de escrever valores fixos como:

```
Inserir email user@email.com
```

Você pode utilizar variáveis:

```
Inserir email {email}
Inserir senha {senha}
```

Assim o teste pode ser executado com **diferentes combinações de dados**.

---

# ⚡ Criando Casos de Teste em Massa

O Zephyr permite criar vários testes rapidamente através de **importação**.

### Importação via CSV ou Excel

É possível importar planilhas contendo campos como:

```
Name
Objective
Steps
Expected Result
Priority
```

---

### Benefícios

- Criar **dezenas ou centenas de testes rapidamente**
- Migrar testes de ferramentas antigas
- Importar testes criados em planilhas

---

# 🤖 Criando Test Scripts com IA (Reflect)

Ferramentas de IA podem auxiliar na geração automática de **test scripts**.

Essas ferramentas analisam:

- requisitos
- histórias de usuário
- descrições de funcionalidades

e sugerem passos de teste automaticamente.

Exemplo:

História de usuário:

- Como usuário, quero fazer login para acessar minha conta.

A ferramenta pode sugerir passos como:

```
1. Acessar página de login
2. Inserir e-mail válido
3. Inserir senha válida
4. Clicar em login
5. Verificar redirecionamento para dashboard
```

Essa abordagem ajuda a acelerar a criação de testes, mas **os testes ainda devem ser revisados pelo QA**.

---

# 📈 Gerando Relatórios no Zephyr

O Zephyr oferece relatórios para acompanhar a qualidade e progresso dos testes.

Para acessar:

```
Zephyr → Relatórios
```

---

### Tipos de relatórios disponíveis

**Test Execution Report**

Mostra resultados como:

```
PASS
FAIL
BLOCKED
NOT EXECUTED
```

---

**Traceability Report**

Relaciona:

```
Requisitos → Casos de Teste → Execução
```

---

**Test Progress**

Permite acompanhar o progresso da execução de testes.

Exemplo:

```
Total tests: 50
Executed: 40
Passed: 35
Failed: 5
```

---

# 📌 Conclusão

O Zephyr Scale transforma o Jira em uma ferramenta completa de **gerenciamento de testes**, permitindo:

- Criar e organizar **casos de teste**
- Executar testes em **ciclos**
- Trabalhar com **BDD**
- Utilizar **datasets**
- Criar testes de forma mais rápida com auxílio de **IA**
- Gerar **relatórios de qualidade**

Essa integração facilita a colaboração entre **QA, desenvolvedores e gestores**, garantindo maior controle sobre a qualidade do software.

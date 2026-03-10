# 🧪 Como Escrever Casos de Teste

Um **caso de teste (Test Case)** é um conjunto de condições e passos utilizados para verificar se uma funcionalidade do sistema está funcionando conforme o esperado.

Os casos de teste são utilizados para garantir que os testes sejam **reproduzíveis, padronizados e documentados**, permitindo que qualquer membro da equipe execute o mesmo teste e obtenha resultados consistentes.

Um caso de teste normalmente inclui os seguintes elementos:

---

# 1️⃣ Título do Caso de Teste

O título descreve **de forma clara e objetiva o que está sendo testado**.

Boas práticas:

- Deve ser curto e direto
- Deve representar o objetivo do teste
- Não deve haver **dois casos de teste com o mesmo título**

### Exemplo

> Verificar login com e-mail e senha válidos

ou

> Validar cadastro de usuário com número de telefone válido

---

# 2️⃣ Pré-condições

As **pré-condições** descrevem o estado necessário do sistema antes da execução do teste.

Elas garantem que o ambiente esteja preparado para executar o caso de teste.

### Exemplo

- Usuário já registrado no sistema
- Usuário possui credenciais válidas
- Aplicação está acessível

---

# 3️⃣ Etapas de Teste (Passos)

As **etapas de teste** descrevem passo a passo como executar o teste.

Boas práticas:

- Escrever passos claros e objetivos
- Cada passo deve representar uma única ação
- Evitar passos muito longos ou ambíguos

### Exemplo

1. Acessar a página de login  
2. Inserir um nome de usuário válido  
3. Inserir uma senha válida  
4. Clicar no botão **"Sign in"**

---

# 4️⃣ Resultado Esperado

O **resultado esperado** descreve o comportamento correto do sistema após a execução das etapas do teste.

Ele é utilizado para verificar se o sistema está funcionando corretamente.

### Exemplo

- Usuário é autenticado com sucesso
- Usuário é redirecionado para a página inicial
- Sistema envia OTP para confirmação de conta

---

# 5️⃣ Cenário de Teste Relacionado

Um caso de teste normalmente está associado a um **cenário de teste**, que representa uma funcionalidade ou fluxo geral do sistema.

Como visto no **Capítulo 4 – Criação de Cenários de Teste**, o cenário define **o que precisa ser testado**, enquanto o caso de teste descreve **como executar o teste**.

### Exemplo

> Cenário de teste: Login de usuário

ou

> Cenário de teste: Cadastro de usuário

---

# 6️⃣ Ambiente de Teste

O **ambiente de teste** descreve em quais condições o teste será executado.

Isso pode incluir:

- Sistema operacional
- Navegador
- Dispositivo
- Tipo de rede

### Exemplo

Desktop:

> Windows 11
> 
> Google Chrome
> 
> Rede Wi-Fi

Mobile:

> Samsung Galaxy Note 20
> 
> Android 13
> 
> Rede 4G

---

# 7️⃣ Resultado Atual (Resultado Real)

O **resultado atual** descreve o que realmente aconteceu após executar o teste.

Ele é registrado após a execução do caso de teste e comparado com o resultado esperado.

> Usuário é redirecionado para o feed de notícias

Resultado atual:

> Usuário foi redirecionado corretamente para o feed de notícias

---

# 8️⃣ Status do Caso de Teste

O status indica o estado atual do caso de teste após sua execução.

Os status mais comuns são:

| Status | Significado |
|------|------|
| **New** | Caso de teste criado, ainda não executado |
| **Ready for Test** | Caso de teste pronto para execução |
| **Pass** | Teste executado com sucesso e resultado esperado alcançado |
| **Fail** | Teste executado, mas resultado diferente do esperado |
| **Blocked** | Teste não pode ser executado devido a dependência ou problema no sistema |
| **Skipped** | Teste não foi executado (por decisão do time ou mudança de escopo) |

---

# 📊 Estrutura Simplificada de um Caso de Teste

Um caso de teste normalmente segue a seguinte estrutura:

| Campo | Descrição |
|------|------|
| ID | Identificador único do teste |
| Título | Descrição do objetivo do teste |
| Pré-condição | Condições necessárias antes do teste |
| Passos | Etapas de execução |
| Resultado esperado | Comportamento esperado do sistema |
| Ambiente | Ambiente onde o teste será executado |
| Resultado atual | Resultado obtido após execução |
| Status | Estado atual do teste |

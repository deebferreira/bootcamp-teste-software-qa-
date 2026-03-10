# 🧪 Casos de Teste vs Cenários de Teste

No **Capítulo 4 – Criação de Cenários de Teste**, vimos como os **cenários de teste** ajudam a identificar o que deve ser validado em uma funcionalidade.

Nesta seção vamos aprofundar a diferença entre:

- **Cenários de Teste (Test Scenarios)**
- **Casos de Teste (Test Cases)**

Embora estejam relacionados, eles possuem **níveis de detalhe diferentes** no planejamento e execução dos testes.

---

# 📌 Cenários de Teste (Test Scenarios)

Como visto anteriormente no **Capítulo 4**, um **cenário de teste** representa uma situação ou funcionalidade que precisa ser validada no sistema.

Eles são descritos em **alto nível**, sem detalhar os passos de execução.

### Exemplo

Funcionalidade: **Cadastro de usuário**

Cenários possíveis:

- Registrar-se com número de telefone válido
- Registrar-se com e-mail válido
- Registrar-se com nome e sobrenome válidos
- Registrar-se com diferentes formatos de telefone
- Registrar-se com idade válida
- Registrar-se selecionando um gênero

Cada cenário representa **uma situação que deve ser testada**, mas ainda não define exatamente como o teste será executado.

---

# 📌 Casos de Teste (Test Cases)

Um **caso de teste** é a descrição detalhada de **como executar o teste**.

Ele define passo a passo como validar um cenário.

Normalmente inclui:

- Identificador do teste (ID)
- Pré-condições
- Passos de execução
- Dados de entrada
- Resultado esperado
- Prioridade
- Status do teste

O objetivo é garantir que o teste seja **reproduzível e padronizado**.

---

## 📊 Exemplo de Caso de Teste

**Cenário:** Registrar-se com número de telefone válido

**Pré-condição**

> O usuário deve possuir um número de telefone ou e-mail válido.

**Passos**

1. Navegar até a página de cadastro  
2. Inserir um primeiro nome válido  
3. Inserir um sobrenome válido  
4. Inserir um número de telefone válido  
5. Inserir uma senha válida  
6. Inserir uma data de nascimento válida  
7. Selecionar um gênero  
8. Clicar em **"Sign up"**

**Resultado esperado**

- Registro realizado com sucesso
- Usuário redirecionado para o feed de notícias
- Envio de OTP para confirmação

---

# 🔎 Diferença entre Cenário e Caso de Teste

| Cenário de Teste | Caso de Teste |
|---|---|
| Alto nível | Detalhado |
| Define **o que testar** | Define **como testar** |
| Baseado na funcionalidade | Baseado em passos |
| Menos detalhado | Estruturado e executável |

---

# 📌 Testes de Alto Nível vs Baixo Nível

Esses conceitos também se relacionam com **níveis de detalhamento dos testes**.

## 🔹 Testes de Alto Nível (High-Level Tests)

Descrevem **funcionalidades ou fluxos gerais do sistema**, sem detalhar execução.

Geralmente correspondem aos **cenários de teste**.

**Exemplo**

> Validar cadastro de usuário com dados válidos

---

## 🔹 Testes de Baixo Nível (Low-Level Tests)

São testes detalhados que especificam **passos, dados e resultados esperados**.

Correspondem aos **casos de teste**.

**Exemplo**

1. Acessar página de cadastro  
2. Inserir nome válido  
3. Inserir telefone válido  
4. Inserir senha válida  
5. Clicar em **Sign up**

**Resultado esperado**

> Usuário registrado com sucesso.


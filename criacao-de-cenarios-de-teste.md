## Criação de Cenários de Teste

Um **cenário de teste** representa uma funcionalidade ou comportamento do sistema que pode ser validado. Ele também pode ser chamado de **condição de teste** ou **possibilidade de teste**.

Ao criar cenários de teste, o profissional de QA deve se colocar no lugar do **usuário final**, buscando identificar possíveis falhas e comportamentos inesperados no sistema.

---

## Como Criar Cenários de Teste

### 1. Estudar os documentos do projeto

O primeiro passo é analisar toda a documentação disponível, como:

- Requisitos de negócio  
- Especificação de requisitos funcionais  
- Histórias de usuário  
- Documentos técnicos  

Essa análise permite compreender o comportamento esperado do sistema.

---

### 2. Isolar cada requisito

Separe o sistema em funcionalidades individuais.

**Exemplos:**
- Login  
- Cadastro  
- Carrinho de compras  

Em seguida, identifique:

- Possíveis ações do usuário  
- Fluxos principais e alternativos  
- Possíveis falhas técnicas  
- Riscos associados  

Também é importante considerar **questões de segurança**, como:
- Entrada de dados inválidos  
- Tentativas de acesso indevido  
- Falhas de validação  

---

### 3. Escrever os cenários de teste

Para cada funcionalidade, crie cenários que cubram diferentes comportamentos do usuário.

- Não há um número fixo de cenários  
- O ideal é cobrir todos os fluxos relevantes  

**Exemplo:**
- Usuário realiza login com dados válidos  
- Usuário tenta login com senha incorreta  
- Usuário deixa campos obrigatórios em branco  

---

### 4. Criar rastreabilidade

Estabeleça uma relação entre **cenários de teste e requisitos**.

Isso é chamado de **rastreabilidade bidirecional**, permitindo responder:

- Qual requisito está sendo testado?
- Quais cenários são impactados se um requisito mudar?

Essa prática é essencial para manter a qualidade e facilitar manutenções futuras.

---

### 5. Revisar os cenários

Os cenários devem ser revisados por outros membros da equipe para garantir:

- Cobertura adequada  
- Clareza  
- Consistência  
- Validade  

A revisão ajuda a identificar falhas antes da execução dos testes.

---

### Observação Importante

Após a análise das funcionalidades, é necessário decidir **quais cenários serão executados**.

Essa decisão depende de fatores como:

- Tempo disponível  
- Prioridade das funcionalidades  
- Fase do projeto (início, desenvolvimento ou pré-lançamento)  

---

## Dicas e Boas Práticas

### 🔹 Pesquise cenários semelhantes

Se o sistema for comum (ex: e-commerce), você pode buscar referências:

> "cenários de teste para e-commerce"

Isso ajuda a ter ideias e garantir maior cobertura.

---

### 🔹 Utilize ferramentas de apoio

Ferramentas como o ChatGPT podem auxiliar na criação de cenários.

**Exemplo de prompt:**

> Tenho uma funcionalidade de login com os seguintes campos obrigatórios: nome, e-mail e telefone.  
> Você pode sugerir cenários de teste para essa funcionalidade?

---

### 🔹 Pense como usuário (e como atacante também 👀)

Além do uso normal, considere:

- Erros de preenchimento  
- Comportamentos inesperados  
- Tentativas maliciosas  

Isso aumenta significativamente a qualidade dos testes.

Cenários bem definidos permitem identificar falhas com mais eficiência, melhorar a cobertura dos testes e garantir que o sistema atenda às expectativas do usuário e do negócio.

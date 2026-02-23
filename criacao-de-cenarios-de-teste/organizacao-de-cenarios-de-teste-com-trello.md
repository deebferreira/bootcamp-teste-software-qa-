## Organização de Cenários de Teste com Trello

O Trello pode ser utilizado como uma ferramenta simples e visual para organizar cenários de teste.

Neste exemplo, foi criado um quadro contendo três listas principais:

- **Inscrever**
- **Fazer Login**
- **Pesquisar**

Dentro de cada lista, são adicionados cartões representando funcionalidades específicas, como por exemplo: *"Inscrever-se no Facebook"*.

---

## Estrutura dos Cartões

Dentro de cada cartão, é possível adicionar:

- Etiquetas  
- Datas  
- Checklists  
- Membros  

Neste caso, foram criados dois checklists principais:

### ✔️ Cenários Válidos
Representam testes realizados com **dados corretos**, simulando o uso esperado do sistema.

### ❌ Cenários Inválidos
Representam testes com **dados incorretos ou incompletos**, com o objetivo de validar o comportamento do sistema diante de erros.

---

## Execução dos Cenários

Dentro de cada checklist, são adicionados os cenários de teste (ex: cenário 1, 2, 3...).

À medida que os testes são executados:

- Cenários aprovados são marcados como concluídos  
- Após a finalização, o cartão pode ser movido para a lista **"Concluído"**

---

## Evidências de Teste

É possível anexar evidências diretamente nos cartões, como:

- Prints de execução  
- Resultados dos testes  
- Imagens de cenários válidos e inválidos  

Isso ajuda na rastreabilidade e documentação dos testes.

---

## Boas Práticas

### 🔹 Testar um erro por vez

Ao validar cenários inválidos, o ideal é:

- Alterar apenas **um campo por vez**
- Manter os demais campos válidos

Isso facilita a identificação exata da causa do erro.

---

### 🔹 Campos com comportamento padrão

Alguns campos podem possuir valores padrão (ex: data de nascimento ou gênero).

Nesses casos:

- É necessário validar se o sistema permite ou não valores vazios  
- Ou se exige interação do usuário  

---

### 🔹 Validação de mensagens de erro

Ao inserir dados inválidos, espera-se que o sistema:

- Destaque o campo com erro (ex: borda vermelha)  
- Exiba mensagens claras para o usuário  

---

### 🔹 Tratamento de dados de entrada

Exemplo importante:

- Ao colar um número de telefone, o sistema deve:
  - Remover espaços extras  
  - Tratar formatação automaticamente  

Isso garante melhor experiência do usuário e evita erros.

# 🐞 Como Escrever um Bug Report (Relatório de Defeitos)

Um **Bug Report** é um documento utilizado para registrar defeitos encontrados durante os testes de software.

O objetivo do relatório é fornecer informações claras e suficientes para que os desenvolvedores consigam **reproduzir o problema e corrigi-lo**.

Um bom relatório de bug deve ser **claro, objetivo e detalhado**, evitando ambiguidades.

---

# 📌 Estrutura de um Bug Report

## 1️⃣ Título do Bug

O título deve ser **curto, claro e descritivo**, permitindo entender rapidamente qual é o problema.

Evite títulos muito vagos.

❌ Exemplo ruim  
Erro no site

✔ Exemplo correto  
Usuário não consegue salvar imagem após aplicar filtro Creative Commons no Google Imagens

---

## 2️⃣ Etapas para Reproduzir (Steps to Reproduce)

As etapas devem explicar exatamente **como reproduzir o problema**.

Cada passo deve ser **claro e sequencial**.

### Exemplo

**Pré-condição**

Abrir o navegador e acessar https://www.google.com

**Passos**

1. Clicar na opção **Imagens**
2. Pesquisar por qualquer termo
3. Abrir **Ferramentas**
4. Filtrar por **Licenças Creative Commons**
5. Selecionar uma imagem
6. Clicar com o botão direito
7. Selecionar **Salvar imagem como**

---

## 3️⃣ Resultado Esperado

Descreve o comportamento correto do sistema.

### Exemplo

O usuário deve conseguir salvar a imagem normalmente em seu computador.

---

## 4️⃣ Resultado Atual (Resultado Real)

Descreve o que realmente aconteceu durante o teste.

### Exemplo

O sistema não permite salvar a imagem e nenhuma ação ocorre ao clicar em "Salvar imagem como".

ou

Uma mensagem de erro é exibida impedindo o download da imagem.

---

## 5️⃣ Ambiente de Teste

Informações sobre o ambiente em que o bug foi encontrado.

Isso ajuda os desenvolvedores a reproduzirem o problema.

### Exemplo

- Sistema Operacional: Windows 11  
- Navegador: Google Chrome 121  
- Dispositivo: Desktop  
- Rede: Wi-Fi  

---

## 6️⃣ Evidências (Screenshots ou Vídeos)

Sempre que possível, adicione evidências visuais.

Isso pode incluir:

- capturas de tela  
- gravações de vídeo  
- logs do sistema  

Essas evidências ajudam a demonstrar o problema com mais clareza.

---

## 7️⃣ Prioridade do Defeito

A prioridade define **o impacto do bug no sistema**.

### Exemplo de níveis de prioridade

| Prioridade | Descrição |
|------|------|
| Crítica | Impede o uso da funcionalidade principal do sistema |
| Alta | Afeta uma funcionalidade importante |
| Média | Problema moderado que não impede o uso do sistema |
| Baixa | Problema visual ou de baixo impacto |

---

# 🧩 Tipos de Defeitos

Os defeitos podem ser classificados de acordo com a sua natureza.

---

## 1️⃣ Defeito Funcional

Ocorre quando uma funcionalidade do sistema **não funciona como deveria**.

### Exemplo

Usuário não consegue realizar login mesmo inserindo credenciais válidas.

---

## 2️⃣ Defeito Visual

Relacionado à interface do usuário (UI).

### Exemplo

Botão de login está desalinhado ou sobreposto a outros elementos da tela.

---

## 3️⃣ Defeito de Conteúdo

Relacionado a erros de texto.

### Exemplo

Mensagem exibida com erro de ortografia: "Senah incorreta".

---

## 4️⃣ Defeito de Performance

Relacionado ao desempenho do sistema.

### Exemplo

Página de login demora mais de 10 segundos para carregar.

---


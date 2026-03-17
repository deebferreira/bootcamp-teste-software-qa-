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

# 🎯 Conclusão

Um bom Bug Report é essencial para garantir que os defeitos sejam compreendidos e corrigidos de forma eficiente.

Relatórios claros, objetivos e bem estruturados facilitam a comunicação entre QA e desenvolvedores, contribuindo diretamente para a qualidade do software.

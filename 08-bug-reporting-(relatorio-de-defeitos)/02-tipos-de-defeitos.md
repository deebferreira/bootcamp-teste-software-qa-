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

## 5️⃣ Defeito de Segurança

Relacionado a falhas que podem comprometer a **segurança do sistema ou dos dados do usuário**.

### Exemplo

- Senha exibida em texto puro  
- Falta de criptografia em dados sensíveis  
- Possibilidade de SQL Injection  

---

## 6️⃣ Defeito de Integração

Ocorre quando há falhas na comunicação entre sistemas, serviços ou APIs.

### Exemplo

- API não retorna resposta corretamente  
- Dados não são sincronizados entre sistemas  
- Integração com pagamento falha  

---

## 7️⃣ Defeito de Compatibilidade

Relacionado ao funcionamento do sistema em diferentes ambientes.

### Exemplo

- Funciona no Chrome, mas não funciona no Safari  
- Problemas em dispositivos móveis  
- Layout quebrado em resoluções diferentes  

---

## 8️⃣ Defeito de Acessibilidade

Relacionado à dificuldade de uso do sistema por pessoas com deficiência.

Pode afetar diferentes tipos de usuários:

### 🔹 Visual
Usuários com baixa visão ou cegueira.

**Exemplos**

- Imagens sem descrição (alt text)  
- Baixo contraste de cores  
- Textos muito pequenos ou ilegíveis  

---

### 🔹 Auditivo
Usuários com deficiência auditiva.

**Exemplos**

- Vídeos sem legendas  
- Alertas sonoros sem alternativa visual  
- Conteúdos de áudio sem transcrição  

---

### 🔹 Motor
Usuários com dificuldades motoras.

**Exemplos**

- Não é possível navegar usando teclado  
- Botões muito pequenos ou difíceis de clicar  
- Falta de suporte para navegação assistida  

---

### 🔹 Cognitivo
Usuários com dificuldades de compreensão.

**Exemplos**

- Interface confusa ou complexa  
- Falta de instruções claras  
- Fluxos com muitos passos sem orientação  

---

### 🔹 Fala
Usuários com dificuldades de fala ou interação por voz.

**Exemplos**

- Sistema exige comandos de voz sem alternativa  
- Reconhecimento de voz falha com frequência  
- Não há opção de entrada alternativa (texto ou toque)  

---

### Ferramenta para Teste de Acessibilidade

O axe DevTools é uma extensão de navegador utilizada para realizar testes de acessibilidade em aplicações web, 
identificando problemas que podem dificultar o uso por pessoas com deficiência. 
Integrado ao DevTools do navegador, ele analisa automaticamente a página com base nas diretrizes WCAG (Web Content Accessibility Guidelines) 
e apresenta erros, alertas e sugestões de melhoria. É uma ferramenta muito utilizada por QAs e desenvolvedores para garantir que o sistema seja mais inclusivo, 
ajudando a detectar problemas como falta de contraste, ausência de textos alternativos (alt text) e elementos não acessíveis via teclado.

> [https://www.deque.com/axe/](https://chromewebstore.google.com/detail/axe-devtools-web-accessib/lhdoppojpmngadmnindnejefpokejbdd?pli=1)

---

<img width="1915" height="910" alt="image" src="https://github.com/user-attachments/assets/645d2a6c-2671-420a-8415-552d292603fe" />

<img width="1917" height="1033" alt="image" src="https://github.com/user-attachments/assets/5c77f89e-194d-41e0-9552-35fabda53260" />

---

# 📌 Conclusão

Identificar corretamente o tipo de defeito ajuda a priorizar a correção e facilita a comunicação entre QA e desenvolvedores, contribuindo para a qualidade do software.

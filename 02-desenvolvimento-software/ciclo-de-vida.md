## Existem três categorias principais de modelos de desenvolvimento de software:
- **Sequencial**
- **Iterativo**
- **Incremental**

---

## Modelo Sequencial

No modelo sequencial, o software passa por uma sequência de etapas bem definidas.  
Após a conclusão de uma etapa, não há retorno para a fase anterior; inicia-se a próxima etapa.

### Etapas do modelo sequencial
1. Coleta de requisitos  
2. Design / Wireframes  
3. Implementação e desenvolvimento  
4. Testes  

---

## Modelo Cascata (Waterfall)

O **modelo cascata** é um modelo sequencial composto por seis fases principais:

1. Coleta de requisitos  
2. Design / Wireframes  
3. Implementação / Desenvolvimento  
4. Testes  
5. Controle de versões e implantação do produto no servidor  
6. Manutenção  

### Características
- O cliente não participa ativamente do processo após a definição dos requisitos.

### Vantagens
- Modelo simples e fácil de entender  
- Pode ser utilizado em projetos pequenos e por pequenas empresas  

### Desvantagens
- Alto custo para correção de falhas detectadas tardiamente  
- Pouca flexibilidade para mudanças  

### Diagrama do Modelo Cascata
<img width="500" height="384" alt="modelo-cascata" src="https://github.com/user-attachments/assets/8f9796c7-e5df-4f65-b781-d1b2517e7df8" />

---

## Modelo em V

O **modelo em V** é uma variação do modelo cascata e estabelece uma forte relação entre desenvolvimento e testes.

### Requisitos do Usuário
Respondem às seguintes perguntas:
- O que o sistema faz?
- Qual é o objetivo do sistema?
- Por que ele foi criado?

Nesta etapa é utilizado o **BRD (Business Requirements Document)** – Documento de Requisitos de Negócio.

### Especificações do Software
Definem como o sistema será desenvolvido.

Nesta etapa é utilizado o **SRS (Software Requirements Specification)** – Especificação de Requisitos de Software.

Essas etapas são amplamente utilizadas em:
- Testes de Aceitação  
- Testes de Sistema  

### Diagrama do Modelo em V
<img width="1180" height="695" alt="modelo-em-v" src="https://github.com/user-attachments/assets/410647d9-188c-420d-b217-da4716d8d190" />

---

## Processo de Design

Após a definição dos requisitos, o processo de design é dividido em duas etapas:

### Projeto Arquitetônico
Analisa o sistema de forma geral, identificando os componentes e suas interações.

### Projeto Detalhado
Define o design de componentes ou módulos específicos do sistema.

Durante essas etapas são realizados:
- Testes de Unidade  
- Testes de Integração

## Planejamento de Testes no Modelo em V

Diferentemente do modelo cascata, que é estritamente sequencial, no **modelo em V** é possível planejar as etapas de teste de duas maneiras:

- **Planejamento dos testes:**  
  É possível iniciar pelo **teste de aceitação** e avançar até o **teste de unidade**, focando no planejamento antecipado das atividades de teste.

- **Execução dos testes:**  
  Quando é necessário executar os testes à medida que o sistema é desenvolvido, inicia-se pelo **teste de unidade** e avança-se até o **teste de aceitação**, fornecendo feedback contínuo sobre a qualidade do sistema.

Esse modelo é considerado mais eficiente do que o modelo cascata no que diz respeito aos testes, pois eles são aplicados **desde o início do desenvolvimento**.  
Ainda assim, ele é classificado como um **modelo sequencial**, uma vez que o cliente não participa ativamente do processo.

---

## Desenvolvimento Ágil

No **desenvolvimento ágil**, o software é entregue de forma **incremental e iterativa**, com entregas frequentes ao cliente. Isso permite o recebimento de **feedback constante e antecipado**.

Além disso, são realizadas entregas iterativas para que o cliente já consiga utilizar o produto. Esse conceito é conhecido como **MVP (Minimum Viable Product)**, ou **Produto Mínimo Viável**, também chamado de **produto potencialmente lançável**.

---

## Diferenças entre os Modelos de Desenvolvimento

### Modelo Sequencial
A maioria dos requisitos é definida desde o início do projeto e permanece fixa, com pouca ou nenhuma possibilidade de alteração.  
O projeto costuma ser simples e possui pouca interação com o cliente durante o processo.

**Exemplos:**  
- Modelo Cascata  
- Modelo em V  

**Desvantagens:**
- Pouca flexibilidade  
- Erros são identificados tardiamente, geralmente na fase de testes  
- Não lida bem com mudanças de requisitos  

---

### Modelo Iterativo
O sistema é desenvolvido em **ciclos repetidos (iterações)**, permitindo um desenvolvimento evolutivo.  
Há **feedback constante do cliente** e possibilidade de ajustes frequentes ao longo do projeto.

**Exemplos:**  
- Prototipação  
- RUP  
- Scrum (parcialmente)  

**Desvantagens:**
- Pode gerar retrabalho  
- Exige maior comunicação entre as partes  
- Pode sair do escopo se não houver controle adequado  

---

### Modelo Incremental
Geralmente utilizado em conjunto com o modelo iterativo.  
O sistema é entregue **por partes (incrementos)**, sendo que cada incremento adiciona novas funcionalidades utilizáveis.

**Exemplos:**  
- Scrum  
- Agile  

**Vantagens:**
- Entregas frequentes de software funcional desde o início  
- O cliente percebe valor rapidamente  

**Quando usar:**
- Projetos grandes  
- Quando é importante entregar rapidamente  
- Ambientes competitivos  

**Desvantagens:**
- Requer bom planejamento  
- A integração entre incrementos pode ser complexa  

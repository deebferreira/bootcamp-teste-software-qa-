## O que é Teste de Software

O teste de software tem como objetivo garantir a qualidade do software e minimizar riscos para o usuário e o negócio em **sites**, **plataformas** e **aplicativos**.

Quando um software não é testado e apresenta muitos problemas, isso pode gerar grandes prejuízos de **tempo**, **dinheiro** e afetar negativamente a **reputação da empresa**.  
Além disso, softwares não testados podem causar **danos graves**, podendo, em casos extremos, resultar em **injúrias ou até mesmo morte**, especialmente em sistemas críticos.

Os testes garantem a **qualidade do produto** e ajudam a **reduzir riscos**.

---

## Objetivos do Teste de Software

1. **Avaliação do produto de trabalho**  
   Consiste na análise da documentação criada ao longo do desenvolvimento, como código, requisitos e testes, que compõem o produto final.

2. **Cumprimento dos requisitos**  
   Envolve atividades de verificação para garantir que todos os requisitos definidos foram atendidos.

3. **Aumento da confiança**  
   Cria confiança de que o software está pronto para ser lançado, com o menor número possível de defeitos.

4. **Encontrar defeitos e falhas**  
   Encontrar defeitos e falhas é um dos principais objetivos do teste de software. Durante a execução dos testes, o objetivo do testador é identificar comportamentos incorretos no sistema (falhas), que são causados por problemas internos no código, nos requisitos ou no          design (defeitos). Essa identificação permite que os problemas sejam registrados, analisados e corrigidos antes que o software seja entregue ao usuário final, reduzindo riscos e garantindo maior qualidade do produto.

5. **Evitar defeitos**  
   O objetivo é evitar que defeitos ocorram desde o início do desenvolvimento.  
   Isso é feito por meio da análise antecipada de:
   - Requisitos  
   - Design  
   - Arquitetura do sistema  

   Quanto mais cedo um problema é identificado, menor é o custo para corrigi-lo.

6. **Prover informações para os stakeholders**  
   Diversas partes interessadas (*stakeholders*) aguardam informações sobre a qualidade do produto que está sendo desenvolvido.

   Cabe ao testador:
   - Fornecer feedbacks claros sobre o estado do software  
   - Informar se o produto está ou não pronto para ser implantado  
   - Apoiar a tomada de decisão com base nos resultados dos testes  

7. **Redução de riscos**  
   A identificação antecipada de defeitos, especialmente nos requisitos e no design, contribui diretamente para a redução de riscos.

   Corrigir problemas com antecedência ajuda a:
   - Evitar falhas em produção  
   - Reduzir custos  
   - Minimizar impactos negativos para o negócio e para o usuário final  

8. **Conformidade com leis e regulamentos**  
   Os testes também têm como objetivo garantir que o software esteja em conformidade com:
   - Leis  
   - Normas  
   - Regulamentos  
   - Padrões exigidos no ambiente onde o sistema será implantado  

   Isso é especialmente importante em sistemas financeiros, de saúde e governamentais.

9. **Objetivos variáveis**  
   Os objetivos do teste de software podem variar de acordo com:
   - Quem está testando  
   - O tipo de sistema  
   - O contexto do projeto  
   - A fase do ciclo de vida do software  

   Por exemplo, os objetivos de teste no início do desenvolvimento podem ser diferentes daqueles no final do projeto.

---

## Diferença entre Defeito e Falha

- **Falha**  
  É o efeito visível de um defeito no software. O sistema se comporta de forma incorreta devido a um problema existente no código.

  **Exemplo:**  
  Um cliente compra cinco unidades e o sistema calcula:  
  `Preço total = R$ 50`  
  Quando o correto seria:  
  `Preço total = R$ 60`  

  O usuário visualiza o valor incorreto na tela.

- **Defeito (Bug)**  
  É um erro no código, requisito, lógica ou design. O defeito existe dentro do software, mesmo que ainda não tenha causado uma falha visível. Ele pode ou não se manifestar.

  **Exemplo:**
  ```python
  preco = quantidade * 10
  # O correto seria:
  preco = quantidade * 12

---

## Teste vs Depuração

O teste de software tem como objetivo identificar defeitos e falhas no sistema, garantindo a qualidade do produto.

Já a depuração (debugging) é a atividade responsável por identificar a causa do defeito e corrigi-lo.

Enquanto o teste é realizado principalmente por profissionais de QA, a depuração é uma atividade típica de desenvolvimento, sendo realizada principalmente por desenvolvedores.

Fluxo:

1. O testador encontra uma falha durante a execução dos testes  
2. Um defeito é registrado  
3. O desenvolvedor realiza a depuração  
4. O testador executa o reteste  
5. Em seguida, realiza o teste de regressão

---

## Tipos de Testes de Software

Os testes de software podem ser classificados de diferentes formas, dependendo do contexto e do objetivo. As principais classificações envolvem a forma de execução, o nível do teste e o objetivo que se deseja alcançar.

A seguir, estão os principais tipos de testes utilizados no dia a dia de um profissional de QA.

---

## 1. Testes quanto à execução

### Teste Estático

O teste estático é realizado sem a execução do sistema. Ele consiste na análise de artefatos como código-fonte, documentos de requisitos, diagramas e outros materiais produzidos durante o desenvolvimento.

Esse tipo de teste tem como principal objetivo identificar defeitos de forma antecipada, reduzindo custos e evitando problemas nas fases posteriores. Exemplos incluem revisão de código, revisão de requisitos e inspeções técnicas.

---

### Teste Dinâmico

O teste dinâmico envolve a execução do sistema ou de partes dele. Nesse tipo de teste, são fornecidos dados de entrada, o sistema é executado e, em seguida, os resultados obtidos são comparados com os resultados esperados.

Esse é o tipo de teste mais comum no dia a dia do QA, pois permite validar o comportamento real da aplicação. Exemplos incluem testes funcionais, testes de API e testes de interface.

---

## Diferenças entre Teste Dinâmico e Teste Estático

### Teste Estático
O teste estático é realizado de forma antecipada e proporciona **maior economia de tempo e dinheiro**.

Ele não envolve a execução do sistema e não possui entrada nem saída de dados.

**Exemplos de teste estático:**
- Revisão de requisitos  
- Revisão de histórias de usuário  
- Revisão de documentos como **SRS** e **BRD**  
- Testes de design no **Figma**  
- Revisão de wireframes  
- Revisão de código (**teste de caixa branca**)  

### Teste Dinâmico
O teste dinâmico requer algum tipo de processamento.  
Nesse tipo de teste, são fornecidos dados de entrada ao sistema, ele executa determinados processos e, em seguida, produz um resultado (saída).

## 2. Testes quanto à abordagem

### Teste de Caixa Preta (Black Box)

O teste de caixa preta avalia o sistema sem considerar sua estrutura interna ou implementação. O foco está apenas nas entradas e saídas, ou seja, no comportamento externo da aplicação.

Nesse tipo de teste, o QA valida se o sistema atende aos requisitos funcionais, sem a necessidade de conhecer o código. É muito utilizado em testes funcionais, testes de sistema e testes de aceitação.

---

### Teste de Caixa Branca (White Box)

O teste de caixa branca é baseado no conhecimento da estrutura interna do sistema, incluindo código, lógica e fluxos de execução.

Esse tipo de teste é geralmente realizado por desenvolvedores ou QAs com conhecimento técnico mais avançado. Ele permite validar caminhos do código, condições, loops e estruturas internas, garantindo maior cobertura e qualidade.

---

## 3. Testes quanto ao nível

### Teste Unitário

O teste unitário verifica pequenas partes do sistema, como funções, métodos ou componentes isolados. Ele é geralmente realizado por desenvolvedores durante a fase de desenvolvimento.

O objetivo é garantir que cada unidade do código funcione corretamente de forma independente. Esse tipo de teste facilita a identificação rápida de erros e contribui para a qualidade do código.

---

### Teste de Integração

O teste de integração tem como foco verificar a comunicação entre diferentes módulos ou sistemas. Ele garante que as partes do sistema funcionem corretamente quando integradas.

Esse tipo de teste é essencial para identificar falhas na troca de dados, como erros em APIs, problemas de comunicação entre serviços ou inconsistências entre módulos.

---

### Teste de Sistema

O teste de sistema valida o sistema completo, simulando o comportamento do usuário final em um ambiente o mais próximo possível do real.

Nesse tipo de teste, são avaliados fluxos completos, como cadastro, login, compras e outras funcionalidades principais. O objetivo é garantir que o sistema atenda aos requisitos especificados.

---

### Teste de Aceitação (UAT)

O teste de aceitação é realizado por usuários finais ou stakeholders, com o objetivo de validar se o sistema atende às necessidades do negócio.

Esse tipo de teste é a última etapa antes da entrega do sistema, sendo fundamental para garantir que o produto esteja pronto para uso em produção.

---

## 4. Testes quanto ao objetivo

### Teste Funcional

O teste funcional verifica se as funcionalidades do sistema estão funcionando conforme o esperado, com base nos requisitos definidos.

Esse tipo de teste foca no "o que" o sistema faz, validando regras de negócio, entradas e saídas de dados, e comportamentos esperados.

---

### Teste Não Funcional

O teste não funcional avalia aspectos relacionados ao desempenho e à qualidade do sistema, como performance, segurança, usabilidade e escalabilidade.

Diferente do teste funcional, aqui o foco está em "como" o sistema se comporta, garantindo uma boa experiência para o usuário e estabilidade da aplicação.

---

## 5. Testes importantes no dia a dia

### Teste de Regressão

O teste de regressão é realizado para garantir que **alterações feitas no sistema não afetaram funcionalidades que já estavam funcionando corretamente**.

Ou seja, mesmo partes do sistema que **não foram modificadas diretamente** devem ser testadas, pois podem ter sido impactadas indiretamente pelas correções.

---

### Reteste (Teste de Confirmação)

O reteste consiste em executar novamente um caso de teste que anteriormente falhou, após a correção do defeito.

O objetivo é confirmar que o problema foi realmente resolvido. Diferente do teste de regressão, o reteste foca especificamente no defeito corrigido.

Se o defeito não ocorrer mais, o problema é considerado **resolvido e encerrado**.

---

### Teste Exploratório

O teste exploratório é realizado sem um roteiro fixo, permitindo que o testador explore o sistema de forma livre, utilizando sua experiência e intuição.

Esse tipo de teste é muito útil para encontrar defeitos que não foram previstos em casos de teste formais, aumentando a cobertura e a qualidade da aplicação.

---

## Verificação e Validação

### Verificação (ponto de vista do desenvolvedor)
A verificação tem como objetivo garantir que **o que está descrito nos requisitos** foi corretamente implementado no sistema.

### Validação (ponto de vista do cliente)
A validação avalia o sistema sob a ótica do usuário final.  
Nesse caso, não se analisa apenas o requisito, mas se o software:
- Atende às necessidades do usuário  
- É útil  
- Proporciona uma boa experiência  
- Gera satisfação durante o uso

---

## Etapas do Processo de Teste

O processo de teste pode ser dividido nas seguintes etapas:

1. **Planejamento**
   - Definição de escopo, estratégia, recursos e cronograma

2. **Design (Projeto de Testes)**
   - Criação de casos de teste, cenários e dados de teste

3. **Execução**
   - Execução dos testes e registro dos resultados

4. **Análise de Resultados**
   - Verificação de falhas e registro de defeitos

5. **Encerramento**
   - Consolidação dos resultados e documentação final
  
<img width="1536" height="1024" alt="ChatGPT Image 22 de fev  de 2026, 11_26_39" src="https://github.com/user-attachments/assets/c0b614f9-b52a-478a-9562-e0d8151c3085" />

---

## Etapas do Processo de Teste (ISTQB)

### 1. Planejamento de Teste

Nesta etapa, analisamos o **plano do projeto** e o **cronograma**, e então criamos o documento chamado **Plano de Teste**.

Esse documento define:

- Equipe de testes
- Papéis e responsabilidades
- Abordagem de testes
- Ferramentas utilizadas
- Padrões e modelos

O plano de teste geralmente é elaborado pelo **Gerente de Testes** ou **Líder de Testes**.

---

### 2. Monitoramento e Controle

Nesta fase, acompanhamos o progresso dos testes comparando o que foi executado com o que foi planejado.

- **Monitoramento:** análise do andamento do projeto
- **Controle:** aplicação de ações corretivas caso algo esteja fora do planejado

Essa etapa também pode gerar um documento chamado **Relatório de Progresso de Teste**, que apresenta:

- O que já foi executado
- Status dos testes
- Possíveis riscos ou desvios

Responsáveis: **Gerente de Testes** e **Líder de Testes**.

---

### 3. Análise de Teste

É nesta etapa que o trabalho do testador começa de forma mais ativa.

Aqui definimos **o que será testado**, identificando as funcionalidades mais importantes do sistema.

Fontes utilizadas:

- Documento de requisitos
- Design do sistema
- Histórias de usuário

Exemplos de análise:

- Validar campo de e-mail vazio
- Validar senha incorreta
- Validar comportamento com dados inválidos

---

### 4. Design de Teste

Nesta etapa, detalhamos **como os testes serão realizados**.

- Criamos **cenários de teste**
- Desenvolvemos **casos de teste**
- Definimos dados de teste

Tudo isso é documentado para garantir padronização e rastreabilidade.

---

### 5. Implementação de Teste

Aqui preparamos o ambiente para execução dos testes.

Inclui:

- Preparação de dados de teste
- Configuração de ambiente
- Escolha de dispositivos ou ferramentas

Exemplo:
- Testar em dispositivo real ou emulador?
- Ambiente local, homologação ou produção?

Essa etapa garante que tudo esteja pronto para iniciar a execução.

---

### 6. Execução de Teste

Nesta fase, executamos os **casos de teste** e comparamos o resultado obtido com o resultado esperado.

- Se o resultado estiver correto → teste aprovado ✅
- Se houver divergência → teste falhou ❌

Quando ocorre falha:

1. É criado um **relatório de defeito (bug report)**
2. O desenvolvedor corrige o problema
3. O testador realiza o **reteste**
4. Em seguida, executa o **teste de regressão**

---

### 7. Encerramento de Teste

Etapa final do processo.

Atividades:

- Consolidação dos resultados
- Geração do **Relatório de Conclusão de Teste**
- Compartilhamento de documentos com outras equipes (ex: manutenção)

Objetivo:

- Avaliar se o software está pronto para entrega
- Registrar aprendizados e melhorias para projetos futuros





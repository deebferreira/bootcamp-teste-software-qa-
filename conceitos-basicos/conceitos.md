## O que é Teste de Software

O teste de software tem como objetivo evitar que usuários tenham experiências ruins em **sites**, **plataformas** e **aplicativos**.

Quando um software não é testado e apresenta muitos problemas, isso pode gerar grandes prejuízos de **tempo**, **dinheiro** e afetar negativamente a **reputação da empresa**.  
Além disso, softwares não testados podem causar **danos graves**, podendo, em casos extremos, resultar em **injúrias ou até mesmo morte**, especialmente em sistemas críticos.

Os testes garantem a **qualidade do produto** e ajudam a **reduzir riscos**.

---

## Diferenças entre Teste Dinâmico e Teste Estático

### Teste Dinâmico
O teste dinâmico requer algum tipo de processamento.  
Nesse tipo de teste, são fornecidos dados de entrada ao sistema, ele executa determinados processos e, em seguida, produz um resultado (saída).

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

## Objetivos do Teste de Software

1. **Avaliação do produto de trabalho**  
   Consiste na análise da documentação criada ao longo do desenvolvimento, como código, requisitos e testes, que compõem o produto final.

2. **Cumprimento dos requisitos**  
   Envolve atividades de verificação para garantir que todos os requisitos definidos foram atendidos.

3. **Aumento da confiança**  
   Cria confiança de que o software está pronto para ser lançado, com o menor número possível de defeitos.

4. **Encontrar defeitos e falhas**  

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



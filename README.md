
<h1 style="display: flex; align-items: center;">  Amazon Data Analysis </h1>

**Time responsável pelo projeto**: Maiully Mendoça e Eslaine Santos
##

<p align="center">
 
[Caso](#caso)  •  [Principais Hipóteses](#principais-hipóteses)  •  [Objetivo](#objetivo)  •  [Ferramentas](#ferramentas)   •  [Resultados e Discussão](#resultados-e-discussão)  •  [Conclusões](#conclusões)  •  [Recomendações](#recomendações)  •  [Venha nos conhecer!](#venha-nos-conhecer)

</p>

Este projeto foi desenvolvido para analisar as avaliações de produtos vendidos na Amazon, buscando entender como diferentes fatores influenciam a percepção dos clientes. O objetivo é fornecer insights acionáveis para melhorar estratégias de marketing, qualidade dos produtos e a experiência geral dos consumidores.


### Caso

Este projeto busca entender os fatores que influenciam as avaliações dos clientes nos produtos vendidos na Amazon. As empresas precisam compreender como variáveis como descontos, preços, número de avaliações e categorias de produtos afetam a percepção dos consumidores para otimizar suas estratégias de marketing, aprimorar a qualidade dos produtos e melhorar a experiência do cliente. 

Além disso, identificar padrões de sentimento nas avaliações dos clientes pode ajudar a detectar problemas específicos e oportunidades de melhoria.

### **Objetivo**

O objetivo deste projeto é analisar as avaliações de produtos da Amazon para entender melhor os fatores que influenciam a satisfação do cliente e fornecer insights valiosos para a tomada de decisões estratégicas. A análise abrange diversas questões, desde a relação entre descontos e avaliações até a identificação de padrões de sentimento nas avaliações dos clientes.

### **Perguntas de Pesquisa**

1. **Produtos com maior desconto tendem a receber melhores avaliações?**
2. **Produtos mais caros tendem a receber melhores avaliações?**
3. **Quanto maior o número de pessoas que avaliaram o produto, melhor será a classificação?**
4. **Quais categorias de produtos possuem melhores avaliações e mais compras?**
5. **Quais são as categorias mais bem avaliadas?**
6. **Qual o principal conteúdo das avaliações baixas e altas?**

### **Metodologia**

- **Tratamento e Limpeza dos Dados**
- **Análise Estatística**: Aplicação de testes de hipóteses, análise de correlação e regressão linear para identificar relações entre variáveis.
- **Natural Language Processing para Análise de Sentimentos das Avaliações**: Uso de técnicas de Processamento de Linguagem Natural (NLP) para analisar sentimentos expressos nas avaliações dos clientes, assim como a identificação de palavras (unigramas), assim como pares (bigramas) e trios (trigramas) de palavras frequentes em avaliações para entender melhor o contexto e as principais reclamações dos clientes.

### Ferramentas

- Google Colab (Python) - Tratamento, limpeza, análise e visualização
- Power Bi - Visualização

#### Tratamento do Dados e Análises

#### Visualização dos dados - Colab e PowerBi

### Apresentação do projeto


### Resultados e Discussão
A análise detalhada desse projeto com os gráficos e discussões pode ser vista em nossa página pública do [Notion], assim como no notebook do [Google Colab]. 

Mas aqui, vou fazer um resumo dos principais resultados encontrados:

- **Descontos e Avaliações**: Não há uma forte relação entre a porcentagem de desconto e a avaliação dos produtos. Embora tenha sido encontrada uma diferença significativa nas médias das avaliações entre produtos com altos e baixos descontos, produtos com baixos descontos tiveram, em média, avaliações ligeiramente melhores.
- **Preços e Avaliações**: Produtos mais caros não tendem a receber melhores avaliações. A análise de correlação e o teste de Mann-Whitney demonstraram uma fraca relação positiva e nenhuma diferença significativa entre os preços dos produtos que receberam avaliações altas e baixas.
- **Número de Avaliações e Qualidade**: Não há correlação entre o número de pessoas que avaliaram um produto e a qualidade da avaliação. A análise de correlação indicou uma fraca relação positiva, refutando a hipótese inicial.
- **Categorias de Produtos**: Entre as categorias com maior quantidade de compras, "Computers&Accessories" apresentou a maior mediana e a maior porcentagem de avaliações altas. "Office Products" também se destacou, mas com menos avaliações.
- **Análise de Sentimentos - NLP**:
    - **Análise de Sentimentos dos Títulos**: A maioria das avaliações dos títulos foram positivas (1432), em comparação com negativas (21) e neutras (6).
    - **Análise dos Unigramas Negativos - Títulos**:
        - **Qualidade do Produto**: Termos como "good", "quality", "bad", "poor" indicam preocupações com a durabilidade e desempenho dos produtos.
        - **Preço**: Termos como "price" e "money" sugerem insatisfação com o custo-benefício.
        - **Funcionalidade**: Termos como "working", "features", "battery", "damaged", "works" apontam problemas técnicos.
        - **Sentimento Negativo**: Termos como "negation" (no, not, never), "fool", "youworst" refletem frustração e insatisfação.
    - **Análise dos Bigramas Negativos - Títulos**: Principais bigramas incluem "good quality", "negation working", "negation smart", "smart one", "one features", "features make", "make fool", "fool youworst", "youworst watch", destacando reclamações sobre funcionalidade e qualidade.
    - **Análise dos Trigramas Negativos - Títulos**: Principais trigramas incluem "watch negation smart", "negation smart one", "smart one features", "one features make", "features make fool", "make fool youworst", "fool youworst watch", "youworst watch connecting", "watch connecting problem", "connecting problem phone", continuando a destacar problemas com smartwatches.
    - **Análise de Sentimentos do Conteúdo das Avaliações**: A maioria das avaliações de conteúdo foram positivas (1423), em comparação com negativas (27) e neutras (9).
    - **Análise dos Unigramas Negativos - Conteúdo das Avaliações**:
        - **Problemas de Funcionamento**: Termos como "negation", "product", "using", "working", "cable", "battery", "money" indicam problemas técnicos e questões financeiras.
        - **Qualidade do Produto e Experiência dos Usuários**: Termos como "product", "quality", "got", "good", "bit", "water", "days", "like" focam na qualidade e experiência do usuário.
        - **Desempenho**: Termos como "unit", "working", "item", "service" indicam discussões sobre desempenho.
        - **Qualidade do Produto**: Termos como "use", "poor", "quality", "charging", "cable", "handle" indicam questões de uso e qualidade, especialmente em relação ao carregamento e manuseio.
        - **Compra, Serviço e Instalação**: Termos como "buy", "bad", "service", "come", "install", "provider", "stand", "pay" destacam problemas de compra, serviço e instalação.
    - **Análise dos Bigramas Negativos - Conteúdo das Avaliações**: Principais bigramas incluem "negative come", "product come", "quality poor", "bad service", "installation guy", "good product", "google tv", "charging cable", "fast charging", indicando problemas de entrega, qualidade e serviço.
    - **Análise dos Trigramas - Conteúdo das Avaliações**: Principais trigramas incluem "câmera display poor", "display poor quality", "poor quality batery", "quality batery good", "batery good nothing", "good nothing badnice", "nothing badnice phone", "badnice phone reasonable", "phone reasonable pricegoodnicevalue", "reasonable pricegoodnicevalue moneytheek", reforçando reclamações sobre a qualidade dos produtos.

### **Considerações Finais**

- **Insights Gerais**: Descontos, preços e número de avaliações não são determinantes para melhores avaliações.
- **Análise de Sentimentos**: Identificação de problemas específicos pode orientar melhorias nos processos de entrega, qualidade do produto e serviços oferecidos.

### **Recomendações**

1. **Focar na Qualidade e no Serviço**: Melhorar a qualidade dos produtos e serviços, especialmente em áreas identificadas como problemáticas, como entrega e atendimento ao cliente.
2. **Monitorar Categorias de Destaque**: Continuar a investir e melhorar as categorias com maior mediana de avaliações, como "Computers & Accessories".
3. **Análise Contínua de Sentimentos**: Manter a análise de sentimentos atualizada para identificar e abordar rapidamente novas questões que possam surgir nas avaliações dos clientes.

### **Limitações dos Dados**

- **Representatividade e Qualidade da Amostra**: Alguns produtos e categorias possuem poucas avaliações, limitando a representatividade.
- **Generalização dos Resultados**: Resultados específicos ao contexto da Amazon podem não se aplicar a outras plataformas.
- **Fatores Externos**: Mudanças no mercado e influências externas não são completamente capturadas nos dados.

### **Ideias Futuras de Análise**

- **Análise Temporal**: Investigar tendências sazonais e o impacto de promoções ao longo do tempo.
- **Análise Demográfica**: Examinar padrões de avaliação de diferentes grupos demográficos.
- **Benchmarking com Concorrentes**: Comparar as avaliações com as de produtos concorrentes para identificar pontos fortes e áreas de melhoria.

## Venha nos conhecer!

Quer saber mais sobre as autoras desse projeto? Acesse o nosso LinkedIn:

https://www.linkedin.com/in/maiully-data-analyst/

https://www.linkedin.com/in/eslaine-santos-e-santos-46159a28/

Obrigada por sua atenção!

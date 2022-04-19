# Rossmann Sales Predict
A Rossmann opera mais de 3.000 drogarias em 7 países europeus. Atualmente, os gerentes de loja da Rossmann têm a tarefa de prever suas vendas diárias com até seis semanas de antecedência. Com milhares de gerentes individuais prevendo vendas com base em suas circunstâncias únicas, a precisão dos resultados pode ser bastante variada e isso dificulta a tomada de decisão. Para auxiliar na resolução da questão foi implementado um modelo de predição que permite interação com o time de negócios.

# Questão de Negócio 
Atender a requisição dos gerentes das lojas que precisam fazer uma previsão de vendas com 6 semanas de antecedência.  

# Entendimento do Negócio 
Após reuniões com pessoas da área descobriu-se que a requisição provém do CFO que está enfrentando o problema de determinar o orçamento para cada loja realizar sua reforma, sendo assim precisa aplicar o valor exato para este orçamento a partir da previsão de vendas das próximas 6 semanas de cada loja. Com o valor da receita das lojas será possível entender a quantia necessária para reforma de cada unidade.

# Hipóteses Importantes
As vendas da loja são influenciadas por muitos fatores, incluindo promoções, competição, feriados escolares e estaduais, sazonalidade e localidade. E a partir destes fatos foram levantadas algumas hipóteses importantes e representadas por meio de visualizações. 

 -
 -
-
-
-
-
-
-

# Etapas de Solução 
<b>1. Análise Descritiva dos Dados</b>

Iniciada descrição dos dados com o objetivo de obter um resumo abrangente sobre os dados para entender qual o problema será enfrentado com esses dados. 

<b>2. Engenharia de Atributos</b>

Neste passo foram criadas variáveis a partir das originais e em seguida aplicada filtragem das variáveis baseada no modelo de negócio que apresenta muitas restrições, pois alguns dados podem ser utilizados e outros não estão disponíveis. 

<b>3. Análise Exploratória de Dados</b>

Esta análise teve dois objetivos: entender o negócio do ponto de vista dos dados e encontrar quais variáveis são importantes para o aprendizado do modelo e para isso foram aplicadas análises univariada, bivariada e multivariada, que possibilitaram o levantamento de hipóteses. 

<b>4. Preparação dos Dados</b>

As variáveis foram transformadas por meio de encoding de categóricas para numéricas em dados cíclios e em seguida a foi modifica a variável resposta com a aplicação do log. 

<b>5. Seleção de Atributos</b>

Por meio do algoritmo Boruta que encontra todas as correlações e sugere variáveis que possam ser relevantes para o modelo, foi realizado um merge e o dataset ficou pronto para a execução da próxima etapa, machine learning. 

<b>6. Treinamento de Modelos de Machine Learning</b>

Foram implementados 5 algoritmos: Baseline, Linear Regression, Linear Regression Lasso, Random Forest Regressor e XGboost Regressor. Em seguido foi ranqueada a performance de cada um desses modelos de acordo com o menor erro ou maior performance, finalizando com a aplicação do cross-validation para medir a performance real. 

<b>7. Modelo de Negócios </b>

A performance do modelo de machine learning foi traduzida para o modelo de negócio com informações que podem impactar no retorno financeiro e custo de investimos.  

<b>8. Implantação do Modelo em Produção </b>

A implementação do modelo em produção visa tornar as predições mais acessíveis para qualquer responsável por acompanhar o desenvolvimento do negócio. 

<b>9. Bot no Telegram </b>


# Conclusão 


# Referências
Disponível em: https://www.kaggle.com/c/rossmann-store-sales


# Rossmann Sales Prediction

<div align="center">
<img src="https://github.com/valferreiraalv/rossmann_sales_prediction/blob/main/img/Rossmann2.png" width="1100px" />
</div>

# Rossmann Store

A Rossmann opera mais de 3.000 drogarias em 7 países europeus. Atualmente, os gerentes de loja da Rossmann têm a tarefa de prever suas vendas diárias com até seis semanas de antecedência. Com milhares de gerentes individuais prevendo vendas com base em suas circunstâncias únicas, a precisão dos resultados pode ser bastante variada e isso dificulta a tomada de decisão. Para auxiliar na resolução da questão foi implementado um modelo de predição que permite interação com o time de negócios.

# Questão de Negócio 
Atender a requisição dos gerentes das lojas que precisam fazer uma previsão de vendas com 6 semanas de antecedência.  

# Entendimento do Negócio 
Após reuniões com pessoas da área descobriu-se que a requisição provém do CFO que está enfrentando o problema de determinar o orçamento para cada loja realizar sua reforma, sendo assim precisa aplicar o valor exato para este orçamento a partir da previsão de vendas das próximas 6 semanas de cada loja. Com o valor da receita das lojas será possível entender a quantia necessária para reforma de cada unidade.

# Hipóteses Importantes
As vendas da loja são influenciadas por muitos fatores, incluindo promoções, competição, feriados escolares e estaduais, sazonalidade e localidade. E a partir destes fatos foram levantadas algumas hipóteses importantes e representadas por meio de visualizações. 

<b>H1.</b> Lojas com maior sortimentos deveriam vender mais.

<b>H2.</b> Lojas com competidores mais próximos deveriam vender menos.

<b>H3.</b> Lojas com competidores a mais tempo deveriam vender mais.

<b>H4.</b> Lojas com promoções ativas popr mais tempo deveriam vender mais.

<b>H5.</b> Lojas com mais dias de promoções consecutivas deveriam vender mais.

<b>H6.</b> Lojas deveriam vender mais ao longo dos anos.

<b>H7.</b> Lojas deveriam vender mais no segundo semestre do ano.

<b>H8.</b> Lojas deveriam vender mais no segundo semestre do ano.

<b>H9.</b> Lojas deveriam vender mais depois do dia 10 de cada mês.

<b>H10.</b> Lojas deveriam vender menos aos finais de semana.

<b>H11.</b> Lojas deveriam vender menos durante os feriados escolares.

# Etapas de Solução 

- [Notebook](https://github.com/valferreiraalv/rossmann_sales_prediction/blob/main/notebooks/m10_v01_store_sales_prediction.ipynb)

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
As etapas executadas nesta questão de negócio demonstram a importância de entender a origem da solicitação de previsão de vendas, quais as reais necessidades dos interessados para que o cientista de dados possa chegar ao resultado apresentado. 

Dentre essas etapas, a análise exploratória de dados foi fundamental para a elaboração de hipóteses que trouxeram insights relevantes para o planejamento de novas ações e aplicações dos modelos de machine learning. 

A implementação dos modelos de machine learning permitiram a construção de cenários que serviram de indicativos para a tomada de decisão pelo time de negócio, que por sua vez teve acesso às informações por meio do bot no Telegram. 



# Referências
Disponível em: https://www.kaggle.com/c/rossmann-store-sales

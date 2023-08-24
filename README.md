# Projeto Ciência de Dados - Previsão de Vendas

- Este é um projeto de ciência de dados focado na previsão de vendas com base nos gastos
   em anúncios nas três grandes redes utilizadas pela empresa Hashtag: TV, Jornal e Rádio.
   O objetivo principal é desenvolver modelos de machine learning capazes de prever as vendas futuras com base nos investimentos em publicidade nas diferentes mídias.

 - Passos do Projeto
    Carregando e Explorando os Dados:
    O projeto começa importando a biblioteca pandas e carregando o conjunto de dados a partir do arquivo "advertising.csv". O conteúdo do DataFrame é exibido para uma análise preliminar. Informações sobre o DataFrame, como tipos de dados e estatísticas básicas, também são exibidas para entender melhor os dados.

- Análise de Correlação:
    A correlação entre as variáveis é explorada para entender as relações entre os gastos em anúncios nas diferentes mídias (TV, Rádio e Jornal) e as vendas.
    A biblioteca seaborn e matplotlib são usadas para criar um mapa de calor que visualiza as correlações.

  Preparação dos Dados:
    As variáveis independentes (X) e a variável dependente (y) são definidas.
    Neste caso, as colunas 'TV', 'Radio' e 'Jornal' são escolhidas como características (X), enquanto 'Vendas' é a variável de destino (y).
     Além disso, os dados são divididos em conjuntos de treinamento e teste usando o train_test_split da biblioteca sklearn.model_selection.

- Modelagem:
   Dois modelos de regressão são implementados para prever as vendas:

- Regressão Linear: Um modelo de regressão linear é criado usando o LinearRegression da biblioteca sklearn.linear_model.
- Random Forest Regressor: Um modelo baseado em árvore de decisão é criado usando o RandomForestRegressor da biblioteca sklearn.ensemble.
 
- Avaliação do Desempenho:
    As previsões são feitas usando os modelos treinados e são avaliadas usando o coeficiente de determinação R² (R-squared). O R² mede a proporção da variabilidade na variável dependente que é explicada pelas variáveis independentes.


As previsões dos dois modelos são comparadas visualmente com os valores reais de vendas usando um gráfico de linhas. A biblioteca seaborn e matplotlib são utilizadas para criar o gráfico.

# Machine Learning - Classificadores: Prevendo o Churn de clientes.

[Dados](https://github.com/GBruneri/Gbruneri/tree/main/Churn_Clientes/Datasets)

[Data-prep](https://github.com/GBruneri/Gbruneri/blob/main/Churn_Clientes/Notebooks/data_prep.ipynb)

[EDA](https://github.com/GBruneri/Gbruneri/blob/main/Churn_Clientes/Notebooks/Churn_EDA.ipynb)

[Modelo](https://github.com/GBruneri/Gbruneri/blob/main/Churn_Clientes/Modelo/Churn_Modelos.ipynb)

## Introdução:
A previsão de churn, ou a taxa em que os clientes deixam de utilizar os serviços ou produtos de uma empresa, é um desafio crucial para muitas organizações em diversos setores. A capacidade de identificar os clientes propensos a abandonar uma empresa permite que as empresas tomem medidas proativas para retê-los, economizando recursos e preservando o crescimento dos negócios. Nesse contexto, o estudo e a prática de algoritmos de classificação são fundamentais. Esses algoritmos são ferramentas poderosas que permitem analisar dados históricos dos clientes, identificar padrões e criar modelos preditivos para antecipar o churn.

## Objetivo:
Desenvolver um algoritimo de classificação que seja capaz de identificar o churn de clientes futuros com base nos dados históricos. Análisar as métricas de performance e fornecer insights a empresa.

## Desenvolvimento:
As etapas de desenvolvimento seguiram o seguinte roteiro:

1) Coleta de Dados: Um extenso conjunto de dados com informações sobre os clientes, como tipo de plano, uso de serviços adicionais, histórico de pagamentos e demais características.

2) Análise de Dados: Análise exploratória dos dados visando a distribuição das variáveis e identificação ou padrões que possam estar relacionados ao Churn.

3) Pré-processamento de Dados: Limpeza e preparação dos dados, incluindo a codificação de variáveis categóricas, divisão dos dados em treino e teste e o tratamento de valores ausentes.

4) Modelagem: Treinamento de modelos de aprendizado de máquina, como K-Nearest Neighbors, Naive Bayes e Árvore de Decisão, para prever o Churn com base nas características dos clientes.

5) Avaliação: Avaliação das métricas como precisão, recall, F1-score e a curva ROC.

## Tecnologias Utilizadas
- Python
- Pandas
- Seaborn
- Matplotlib
- Numpy
- Scikitlearn
- Statsmodels

## Conclusão
Durante a modelagem, foram considerados três algoritmos distintos: o KNN, o Bernoulli Naive Bayes e a árvore de decisão, dos quais o KNN obteve a melhor performance ROC, com 87%. Durante o teste com 2 vetores de características aleatórios, o algoritmo foi capaz de classificar corretamente novas entradas.


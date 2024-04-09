# Projeto de Análise de Risco de Crédito
[Dados](https://github.com/GBruneri/Gbruneri/tree/main/Credit_Risk_ML/Datasets)

[Data Prep](https://github.com/GBruneri/Gbruneri/blob/main/Credit_Risk_ML/Notebooks/prep1.ipynb)

[EDA+Modelo](https://github.com/GBruneri/Gbruneri/blob/main/Credit_Risk_ML/Notebooks/EDA+Modelo.ipynb)

Bem-vindo ao projeto de Análise de Risco de Crédito! Neste projeto, foi explorado a detecção de fraudes em transações de crédito, um desafio comum enfrentado por instituições financeiras em todo o mundo. A fraude de risco de crédito ocorre quando indivíduos tentam obter crédito de forma desonesta, muitas vezes por meio de informações falsas ou enganosas.

## Organização dos arquivos
Todo material necessário se encontra na pasta "**datasets**". A Pasta "**notebooks**" engloba a preparação dos dados no arquivo prep1 e os procedimento de exploração e modelagem no arquivo **EDA+modelo**.

Os arquivos originais podem ser encontrados em : [Conjunto de dados de análise de risco de crédito](https://www.kaggle.com/datasets/praveengovi/credit-risk-classification-dataset)

## Objetivos

Este projeto teve como objetivo desenvolver modelos de aprendizado de máquina capazes de identificar e classificar potenciais casos de fraude de risco de crédito e avaliar duas técnicas de balanceamento de classes alvo. A primeira técnica foi o undersampling, no qual foram removidas aleatoriamente instâncias da classe majoritária, e a segunda técnica foi o oversampling, que consiste em criar exemplos sintéticos baseados nas instâncias dos k-vizinhos mais próximos, aumentando assim a classe minoritária.

## Abordagens Utilizadas
1. **Primeira Abordagem (Undersampling):**
   - Durante o pré-processamento dos dados, um modelo de Random Forest Classifier foi treinado para selecionar as melhores features.
   - Foi realizada a técnica de undersampling, ou seja, foi realizado uma remoção de instâncias para balancear as classes no conjunto de treinamento.
   - Após o pré-processamento dos dados, um modelo de Random Forest Classifier foi treinado para classificação, usando GridSearch para encontrar os melhores hiperparâmetros.
   - A avaliação do modelo incluiu métricas como acurácia, precisão, recall e F1-score, bem como a área sob a curva ROC (ROC-AUC) tanto para o conjunto de teste quanto o de validação.

3. **Segunda Abordagem (Oversampling):**
   - Durante o pré-processamento dos dados, um modelo de Random Forest Classifier foi treinado para selecionar as melhores features.
   - Nesta abordagem, foi aplicada a técnica de oversampling usando o método SMOTE, ou seja, criar exemplos sintéticos da classe minoritária, a fim de equilibrar o conjunto de dados. para balancear as classes no conjunto de treinamento.
   - Novamente foi utilizado GridSearchCV para ajustar os hiperparâmetros de um modelo de Random Forest Classifier.
   - A avaliação do modelo seguiu os mesmos procedimentos da primeira abordagem, com análise detalhada das métricas de desempenho no conjunto de teste e de validação.

## Análise das Métricas

Na análise das métricas de desempenho, destacou-se:
- **Acurácia (Accuracy):** a proporção de previsões corretas em relação ao total de previsões.
- **Precisão (Precision):** a proporção de verdadeiros positivos em relação ao total de positivos previstos pelo modelo.
- **Revocação (Recall):** a proporção de verdadeiros positivos em relação ao total de positivos reais na amostra.
- **F1-score:** a média harmônica entre precisão e recall, fornecendo uma métrica balanceada entre ambas.
- **Área sob a Curva ROC (ROC-AUC):** a capacidade do modelo de distinguir entre classes positivas e negativas.

## Resultados e Conclusões

Ambas as abordagens apresentaram resultados promissores na detecção de fraudes de risco de crédito. A comparação com a previsão com método simulado, ou seja, apenas um critério mostra que a aplicação do algoritimo realmente é necessária. A segunda abordagem, utilizando oversampling, demonstrou uma melhoria marginal nas métricas de precisão e F1-score em comparação com a primeira abordagem de undersampling, demonstrando quen neste cenário a técnica gera uma melhor performance com o ganho de amostragem. Não foi encontrado indicios de Data Leakage e o modelo parece não estar sofrendo de grande sobreajuste( overfitting).


# Projeto de Análise de Risco de Crédito

Bem-vindo ao projeto de Análise de Risco de Crédito! Neste projeto, exploramos a detecção de fraudes em transações de crédito, um desafio comum enfrentado por instituições financeiras em todo o mundo. A fraude de risco de crédito ocorre quando indivíduos tentam obter crédito de forma desonesta, muitas vezes por meio de informações falsas ou enganosas.

Este projeto tem como objetivo desenvolver modelos de aprendizado de máquina capazes de identificar e classificar potenciais casos de fraude de risco de crédito, ajudando assim as instituições financeiras a mitigar riscos e proteger seus ativos.

## Organização dos arquivos
Todo material necessário se encontra na pasta datasets. A Pasta notebooks engloba a preparação dos dados no arquivo prep1 e os procedimento de exploração e modelagem no arquivo EDA+modelo.

Os arquivos originais podem ser encontrados em : [Conjunto de dados de análise de risco de crédito](https://www.kaggle.com/datasets/praveengovi/credit-risk-classification-dataset)


Neste projeto, foram exploradas duas abordagens distintas:

## Abordagens Utilizadas
1. **Primeira Abordagem (Undersampling):**
   - Utilizamos a técnica de undersampling para balancear as classes no conjunto de treinamento.
   - Após o pré-processamento dos dados, um modelo de Random Forest Classifier foi treinado.
   - A avaliação do modelo incluiu métricas como acurácia, precisão, recall e F1-score, bem como a área sob a curva ROC (ROC-AUC).

2. **Segunda Abordagem (Oversampling):**
   - Nesta abordagem, aplicamos a técnica de oversampling usando o método SMOTE para balancear as classes no conjunto de treinamento.
   - Utilizamos GridSearchCV para ajustar os hiperparâmetros de um modelo de Random Forest Classifier.
   - A avaliação do modelo seguiu os mesmos procedimentos da primeira abordagem, com análise detalhada das métricas de desempenho.

## Análise das Métricas

Na análise das métricas de desempenho, focamos em:
- **Acurácia (Accuracy):** a proporção de previsões corretas em relação ao total de previsões.
- **Precisão (Precision):** a proporção de verdadeiros positivos em relação ao total de positivos previstos pelo modelo.
- **Revocação (Recall):** a proporção de verdadeiros positivos em relação ao total de positivos reais na amostra.
- **F1-score:** a média harmônica entre precisão e recall, fornecendo uma métrica balanceada entre ambas.
- **Área sob a Curva ROC (ROC-AUC):** a capacidade do modelo de distinguir entre classes positivas e negativas.

## Resultados e Conclusões

Ambas as abordagens apresentaram resultados promissores na detecção de fraudes de risco de crédito. A segunda abordagem, utilizando oversampling, demonstrou uma melhoria marginal nas métricas de precisão e F1-score em comparação com a primeira abordagem de undersampling.


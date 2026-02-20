# MODELO PREDITIVO TURNOVER DA BASE IBM HR

## 📌 Resumo Executivo

Projeto de modelagem preditiva para identificar colaboradores com maior risco de desligamento (turnover), permitindo ações preventivas da área de RH. A escolha do modelo considerou não apenas desempenho estatístico, mas principalmente impacto estratégico no negócio.

## 🎯 Problema de Negócio

O turnover representa a saída de colaboradores da empresa, gerando custos com recrutamento, treinamento e perda de conhecimento interno. Quando ocorre de forma inesperada, impacta a produtividade, o clima organizacional e os resultados financeiros. O principal desafio de negócio é antecipar esses desligamentos para permitir ações preventivas e reduzir perdas.

## 📊 Fonte dos Dados

IBM HR Analytics Employee Attrition & Performance
Dataset público para fins educacionais, disponibilizado pela IBM e amplamente utilizado em estudos de People Analytics.
Disponível no Kaggle.

## 🔎 Metodologia

Análise exploratória dos dados

Tratamento e preparação das variáveis

Divisão treino/teste (75% / 25%)

Teste de três modelos:

Regressão Logística

Random Forest

XGBoost

Avaliação com foco em:

Recall (principal métrica)

AUC

Matriz de confusão

Análise de overfitting

## 🛠 Skills e Ferramentas

Python

Pandas

Scikit-learn

XGBoost

Matplotlib

## 📈 Resultados e Recomendações

resultados ....

 <img src="https://github.com/Adriele-Cerqueira/PREVENDO-TURNOVER_IBM-HR/blob/main/Correlacao%20Vari%C3%A1veis.png" width="550">

Dataset desbalanceado (~16% de attrition).

Modelos mais complexos não trouxeram ganho estratégico relevante.

O modelo escolhido priorizou maior recall e menor número de falsos negativos.

 <img src="https://github.com/Adriele-Cerqueira/PREVENDO-TURNOVER_IBM-HR/blob/main/Curva%20ROC.png" width="550">
 
 <img src="https://github.com/Adriele-Cerqueira/PREVENDO-TURNOVER_IBM-HR/blob/main/Comparativo%20Modelos.png" width="550">


## 🚀 Próximos Passos

Avaliar novos modelos visando maior desempenho preditivo, ou seja, previsões mais precisas

Desenvolver dashboard para acompanhamento contínuo

Evoluir para análise baseada em impacto financeiro


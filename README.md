# MODELO PREDITIVO TURNOVER DA BASE IBM HR

## 📌 Resumo Executivo

Projeto de modelagem preditiva para identificar colaboradores com maior risco de desligamento (turnover), permitindo ações preventivas da área de RH. A escolha do modelo considerou não apenas desempenho estatístico, mas principalmente impacto estratégico no negócio.

## 🎯 Problema de Negócio

Turnover inesperado gera:

Custos de contratação e treinamento

Perda de conhecimento

Redução de produtividade

O objetivo é antecipar desligamentos para apoiar decisões estratégicas do RH.

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

Dataset desbalanceado (~16% de attrition).

Modelos mais complexos não trouxeram ganho estratégico relevante.

O modelo escolhido priorizou maior recall e menor número de falsos negativos.

Recomendação: implementar um score de risco de turnover para apoiar ações preventivas do RH.

## 🚀 Próximos Passos

Avaliar novos modelos visando maior desempenho preditivo, ou seja, previsões mais precisas

Desenvolver dashboard para acompanhamento contínuo

Evoluir para análise baseada em impacto financeiro


# MODELO PREDITIVO TURNOVER DA BASE IBM HR

## 📌 Resumo Executivo

Projeto de modelagem preditiva para identificar colaboradores com maior risco de desligamento (turnover), permitindo ações preventivas da área de RH. 

## 🎯 Problema de Negócio

Altas taxas de turnover geram custos com reposição, perda de conhecimento e impacto na produtividade. O desafio é reduzir desligamentos inesperados e melhorar a retenção de talentos. A escolha do modelo considerou não apenas desempenho estatístico, mas principalmente impacto estratégico no negócio.


## 📊 Fonte dos Dados

IBM HR Analytics Employee Attrition & Performance
Dataset público para fins educacionais, disponibilizado pela IBM e amplamente utilizado em estudos de People Analytics.
Disponível no Kaggle.

## 🔎 Metodologia
Importação de Bibliotecas: Pandas, Scikit-learn, Seaborn, Matplotlib

Carregamento de Dados: IBM HR Analytics → DataFrame Pandas

Análise Exploratória (EDA): estatísticas descritivas, distribuição de variáveis, padrões de turnover

Pré-processamento: Label Encoding em variáveis categóricas

Divisão de Dados: treino 75% / teste 25%, stratify=y, random_state=42

Modelagem Preditiva: Regressão Logística, Random Forest, XGBoost

Ajuste de Hiperparâmetros: número de árvores, profundidade, taxa de aprendizado

Avaliação de Modelos: Recall, Precision, F1-Score, AUC, matriz de confusão

Seleção do Modelo: foco em recall e falsos negativos mínimos para suportar decisões de RH

## 🛠 Skills e Ferramentas

Análise de Dados: exploração, limpeza e pré-processamento de dados

Modelagem Preditiva: Regressão Logística, Random Forest, XGBoost

Programação: Python (Pandas, Scikit-learn, Seaborn, Matplotlib)

Machine Learning: tratamento de desbalanceamento, ajuste de hiperparâmetros, avaliação de métricas

Visualização de Dados: gráficos e análise de padrões para suportar decisões de negócio

Interpretação de Modelos: insights sobre fatores de risco de turnover e apoio estratégico em RH

## 📈 Resultados e Recomendações

As análises identificaram fatores de risco e proteção para turnover. Funcionários solteiros e que realizam hora extra apresentam maior probabilidade de desligamento, enquanto cargos mais altos, maior remuneração e maior tempo com o gestor reduzem o risco. O modelo preditivo final (Regressão Logística) confirmou esses padrões, destacando-se na identificação de colaboradores em risco, fornecendo insights estratégicos para ações de retenção e gestão de talentos.

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


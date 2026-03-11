# MODELO PREDITIVO TURNOVER DA BASE IBM HR 
 <img src="https://github.com/Adriele-Cerqueira/PREVENDO-TURNOVER_IBM-HR/blob/main/Capa_Turnover.png" width="550">
 
## Resumo Executivo
Este projeto teve como objetivo **prever a probabilidade de desligamento de colaboradores (turnover)** utilizando técnicas de ciência de dados e machine learning.  
A partir da modelagem preditiva e análise exploratória, foi possível identificar **fatores organizacionais e comportamentais que aumentam o risco de saída de funcionários**.  
Os resultados podem apoiar decisões estratégicas de **retenção de talentos e gestão de pessoas**.

---

## Problema de Negócio
Empresas frequentemente enfrentam desafios relacionados ao **alto índice de rotatividade de colaboradores**, o que gera custos com recrutamento, treinamento e perda de conhecimento organizacional.  

Neste cenário, compreender **quais fatores influenciam a saída de funcionários** torna-se essencial para melhorar estratégias de retenção e gestão de pessoas.  

Este projeto busca responder à seguinte questão de negócio:  
**É possível prever quais colaboradores possuem maior probabilidade de deixar a empresa com base em características comportamentais, demográficas e organizacionais?**

---

## Fonte de Dados
Os dados utilizados neste projeto foram obtidos a partir de **um dataset público disponibilizado no Kaggle – IBM HR Analytics Attrition Dataset**.  

O dataset contém informações relacionadas a:

- Cargo e departamento
- Remuneração e benefícios
- Satisfação no trabalho
- Tempo de empresa
- Horas extras
- Informações demográficas dos colaboradores

Após a coleta, os dados passaram por etapas de **limpeza, transformação e preparação** para análise e modelagem preditiva.

---

## Metodologia

- Coleta e importação do dataset utilizando KaggleHub
- Análise exploratória dos dados (EDA)
- Verificação de inconsistências e valores ausentes
- Análise de distribuição da variável de turnover
- Construção de visualizações analíticas para identificação de padrões
- Criação de matriz de correlação com variáveis relevantes
- Transformação de variáveis categóricas utilizando One-Hot Encoding
- Separação das variáveis preditoras (X) e variável alvo (Attrition)
- Divisão dos dados em treino (75%) e teste (25%) com stratify
- Construção e comparação de modelos de classificação
- Avaliação com métricas: Recall, Precision, F1-Score e AUC
- Análise de overfitting comparando desempenho treino vs teste
- Interpretação dos resultados sob perspectiva de negócio

---

## Skills e Ferramentas

**Linguagens**
- Python
- SQL

**Bibliotecas**
- Pandas
- NumPy
- Scikit-Learn
- Matplotlib
- Seaborn
- XGBoost

**Ferramentas de BI**
- Power BI

**Banco de Dados**
- SQL / Oracle / PostgreSQL

**Versionamento**
- Git
- GitHub

---

## Resultados e Recomendações de Negócio

A análise revelou que **determinados fatores comportamentais e organizacionais aumentam significativamente o risco de turnover**.  

O modelo escolhido foi a **Regressão Logística, que apresentou o melhor desempenho para o objetivo do negócio**, alcançando:

- **AUC:** 0,77  
- **Recall:** 66% na detecção de desligamentos  
- **Menor número de falsos negativos entre os modelos testados**
 
<img src="https://github.com/Adriele-Cerqueira/PREVENDO-TURNOVER_IBM-HR/blob/main/Curva%20ROC.png" width="550">
  
<img src="https://github.com/Adriele-Cerqueira/PREVENDO-TURNOVER_IBM-HR/blob/main/Comparativo%20Modelos.png" width="550">

Com esse modelo, e as análises exploratórias foi possível observar que **funcionários que realizam horas extras, possuem menor satisfação no trabalho e apresentam menor tempo de empresa** possuem maior probabilidade de desligamento.

Principais fatores associados ao risco de saída:

- Funcionários que realizam **hora extra têm cerca de 69% mais chance de sair**
- Colaboradores **solteiros apresentam maior probabilidade de desligamento**
- Funcionários do **departamento de vendas possuem maior risco**
- **Maior satisfação no ambiente de trabalho reduz o turnover**

 <img src="https://github.com/Adriele-Cerqueira/PREVENDO-TURNOVER_IBM-HR/blob/main/Correlacao%20Vari%C3%A1veis.png" width="550">
 
Com base nesses achados, recomenda-se:

- Direcionar estratégias de retenção para **equipes com maior carga de horas extras**
- Monitorar continuamente **indicadores de satisfação dos colaboradores**
- Criar políticas de incentivo e benefícios para **reduzir riscos de desligamento**

Essas ações podem contribuir para **redução do turnover e otimização da gestão de talentos**.

---

## Próximos Passos

- **Integração com novos dados:** incorporar dados reais da empresa para aumentar a robustez do modelo.

- **Automação da pipeline de dados:** estruturar processos automatizados para atualização contínua das análises.

- **Evolução do modelo analítico:** testar novas abordagens de machine learning e técnicas de balanceamento de classes para melhorar a performance preditiva.

# Predição da qualidade em um processo de mineração - Desafio IHM Stefanini

## Descrição do Projeto
Este projeto tem como objetivo prever a quantidade de impureza (sílica) presente no concentrado de minério de ferro durante o processo de flotação em uma planta de mineração. A previsão da impureza permite que os engenheiros tomem ações corretivas antecipadamente, otimizando o processo e reduzindo a quantidade de minério que vai para os rejeitos, o que contribui para a preservação ambiental.
Os dados utilizados neste projeto foram coletados entre março e setembro de 2017 e incluem medições de qualidade do minério e variáveis de processo como nível e fluxo de ar nas colunas de flotação. O objetivo principal é prever a última coluna do dataset, que representa a porcentagem de sílica no concentrado de minério.

## Dados
Coluna 1: Data e hora (variável temporal).
Colunas 2 e 3: Medidas de qualidade do minério de ferro antes de entrar na planta de flotação.
Colunas 4 a 8: Variáveis mais importantes que impactam a qualidade do minério no final do processo.
Colunas 9 a 22: Dados de processo (nível e fluxo de ar nas colunas de flotação).
Colunas 23 e 24: Medições finais de qualidade do minério de ferro (coluna 24 é o objetivo).

## Objetivo
O objetivo do projeto é prever a porcentagem de sílica no concentrado de minério de ferro (coluna 24) utilizando técnicas de aprendizado de máquina.

## Modelos Utilizados
Foram desenvolvidos dois tipos de modelos preditivos:
1. Modelo de Série Temporal (Prophet)
   O Prophet foi utilizado para capturar a tendência e os padrões temporais dos dados de impureza da sílica ao longo do tempo. Este modelo permite fazer previsões de curto e médio prazo com base em padrões históricos.
2. Modelo de Regressão (XGBRegressor)
   O modelo de regressão XGBoost foi utilizado para prever a porcentagem de sílica no concentrado de minério com base nas variáveis de entrada disponíveis. O XGBoost foi escolhido por sua eficiência em dados tabulares e capacidade de lidar com relações não lineares entre as variáveis.

## Resultados
- Os resultados do modelo Prophet foram avaliados utilizando as métricas RMSE, MAE e MAPE. O modelo apresentou valores de métricas que podem ser melhorados.
- Os resultados do modelo XGBRegressor foram avaliados utilizando as métricas R2, MSE e RMSE. O modelo apresentou resultados satisfatórios, no entanto ainda há espaço para as métricas serem melhoradas.

## Conclusão
Este projeto demonstrou que é possível prever a quantidade de sílica no concentrado de minério de ferro com relativa precisão, utilizando tanto modelos de séries temporais quanto de regressão. A previsão antecipada da impureza pode auxiliar na tomada de decisões dentro da planta de mineração, otimizando o processo e contribuindo para a sustentabilidade ambiental.

## Bibliotecas utilizadas
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `pymannkendall`
- `math`
- `statsmodels`
- `optuna`
- `scikit-learn`
- `neuralprophet`
- `prophet`
- `xgboost`
- `keras`



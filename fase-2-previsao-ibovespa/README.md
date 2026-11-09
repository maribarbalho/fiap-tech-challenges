# Fase 2 · Previsão do fechamento do Ibovespa

**Contexto:** desenvolver um modelo que preveja o valor de fechamento diário do Ibovespa, com horizonte de 10 dias úteis.

## O que foi feito

- **Dados:** histórico diário do Ibovespa de 01/01/2015 a 26/02/2025.
- **Análise da série:** tendência de crescimento, série não estacionária e sazonalidade de baixa amplitude (decomposição e testes estatísticos).
- **Modelos comparados:** Naive (linha de base), AutoARIMA, XGBoost com variáveis de calendário e defasagens, e LSTM com diferentes janelas de defasagem.
- **Ajustes:** várias iterações de hiperparâmetros (profundidade das árvores, tipo de booster, janelas da LSTM), sempre comparadas por WMAPE, MAE, MSE e MAPE.

## Resultado no conjunto de teste (10 dias)

| Modelo | MAPE | Acurácia (100 − MAPE) |
|---|---|---|
| **XGBoost** | **1,64%** | **98,36%** |
| AutoARIMA | 1,76% | 98,24% |
| Naive | 1,92% | 98,08% |

O XGBoost teve os menores erros. A LSTM com janela de 15 dias úteis foi a que melhor acompanhou visualmente a tendência dos valores reais.

## Fonte dos dados

[Investing.com: Ibovespa, dados históricos](https://br.investing.com/indices/bovespa-historical-data).

**Ferramentas:** Python, Pandas, statsmodels, StatsForecast, scikit-learn, XGBoost, TensorFlow/Keras.

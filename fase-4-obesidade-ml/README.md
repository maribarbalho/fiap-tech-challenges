# Fase 4 · Modelo preditivo de obesidade

**Contexto:** como equipe de dados de um hospital, desenvolver um modelo de machine learning que ajude médicos e médicas a prever se uma pessoa pode ter obesidade, além de um painel analítico com os principais insights.

## O que foi feito

- **Análise exploratória** das 17 variáveis (2.111 registros): hábitos alimentares, atividade física, uso de tecnologia, transporte e histórico familiar.
- **Tradução e categorização** das variáveis para o painel em Power BI.
- **Pipeline do scikit-learn** com transformadores próprios: normalização, one-hot encoding, codificação ordinal e binária, remoção de variáveis e balanceamento das classes com oversampling.
- **Modelos comparados:** Regressão Logística (linha de base), Árvore de Decisão, Random Forest e XGBoost.
- **Otimização** com GridSearch e validação cruzada (5 folds).
- **Exportação** da pipeline e do modelo com `joblib` para uso em uma aplicação Streamlit.

## Resultado

O **Random Forest** otimizado teve a melhor acurácia: **83,2%**, acima da meta de 75% do desafio, tanto no teste quanto na validação cruzada.

Os insights do estudo estão no painel em Power BI: [Fatores Associados à Obesidade](https://maribarbalho.github.io/projetos/analise-obesidade).

## Fonte dos dados

Base de obesidade fornecida no desafio, derivada do conjunto público [Estimation of Obesity Levels (UCI)](https://archive.ics.uci.edu/dataset/544/).

**Ferramentas:** Python, Pandas, scikit-learn, imbalanced-learn, XGBoost, Matplotlib, Seaborn, joblib.

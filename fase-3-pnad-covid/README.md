# Fase 3 · PNAD COVID-19

**Contexto:** entender o comportamento da população durante a pandemia para apoiar o planejamento de um hospital em caso de um novo surto.

## O que foi feito

A partir de consultas SQL à base da PNAD COVID-19, o notebook analisa:

- **Perfil dos entrevistados:** faixa etária, sexo, raça, escolaridade, situação de trabalho e região.
- **Comorbidades** mais frequentes.
- **Testes:** tipos de teste e percentual de resultados positivos.
- **Sintomas:** mais comuns entre os positivos e positividade por quantidade de sintomas.
- **Ações tomadas** pelas pessoas com sintomas e necessidade de internação.
- **Evolução semanal** de plano de saúde, média salarial, trabalho e comportamento de isolamento.

## Fonte dos dados

[PNAD COVID-19 (IBGE)](https://covid19.ibge.gov.br/pnad-covid/). O notebook usa os resultados das consultas exportados em CSV, que não estão incluídos no repositório.

**Ferramentas:** SQL, Python, Pandas, Matplotlib, Seaborn, Plotly.

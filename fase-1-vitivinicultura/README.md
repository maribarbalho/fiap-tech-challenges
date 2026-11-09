# Fase 1 · Exportação, consumo e produção de vinho

**Contexto:** análise do mercado de vinhos para apoiar decisões de exportação, com foco nos últimos 15 anos (2009–2023).

## Notebooks

- [`exportacao_vinho.ipynb`](exportacao_vinho.ipynb): exportações brasileiras de vinho por país de destino (quantidade em kg e valor em US$).
- [`consumo_producao_mundial.ipynb`](consumo_producao_mundial.ipynb): consumo e produção mundial de vinho em comparação com o Brasil.

## O que foi feito

- Recorte dos últimos 15 anos e consolidação por país.
- Ranking dos destinos por valor e por volume, com participação percentual e acumulada (curva de Pareto).
- Evolução anual dos principais destinos (Paraguai, Rússia, Estados Unidos, China, Reino Unido, Espanha e Haiti).
- Comparação entre produção e consumo por país em 2022 e 2023.

## Destaques

- **Paraguai** concentrou **37,5% do valor** exportado no período.
- **Rússia** concentrou **39,5% do volume** exportado, em kg.

## Fonte dos dados

Dados de exportação de vinho da [Embrapa Uva e Vinho (VitiBrasil)](http://vitibrasil.cnpuv.embrapa.br/) e planilha pública de consumo e produção mundial fornecida no desafio. Os arquivos não estão incluídos no repositório.

**Ferramentas:** Python, Pandas, Matplotlib, Seaborn.

# Análise de Custos e Faturamento — Grupo OLZ

![Dashboard Grupo OLZ](images/dashboard-overview.png)

Análise de Custos e Faturamento é um projeto de visualização de dados construído em Power BI para apoiar a área contábil/financeira do Grupo OLZ na identificação de onde a empresa está perdendo dinheiro. O dashboard cruza faturamento, custos, resultado e margem, com quebras por mês, centro de custo e classe de custo, permitindo identificar rapidamente os períodos e categorias que mais impactam o resultado.

## Objetivo

Este projeto tem como objetivo apoiar a área contábil/financeira do Grupo OLZ na identificação de **onde a empresa está perdendo dinheiro** — em quais meses e categorias de custo o resultado ficou negativo — para orientar decisões de controle de custos.

## Fonte dos dados

Dados financeiros (faturamento, custos, resultado e margem) já tratados previamente, cobrindo o período de janeiro a dezembro de 2024.

## Ferramentas utilizadas

Power BI (modelagem de dados, medidas DAX e construção do dashboard interativo).

## Indicadores principais (KPIs)

| Indicador | Valor |
|---|---|
| Faturamento | $203 Mil |
| Custos | $182 Mil |
| Resultado | $21 Mil |
| Margem | 10,38% |

## Principais achados

- **Fevereiro e março foram os meses de prejuízo**, com resultados de **-$19 Mil** e **-$27 Mil** respectivamente — os custos superaram o faturamento nesse período.
- **Novembro também fechou no negativo** (-$7 Mil), embora com impacto bem menor.
- **Dezembro foi o melhor mês do ano**, com faturamento de $45 Mil e resultado de +$33 Mil — indício de sazonalidade de fim de ano.
- **A estrutura de custos é dominada por custos fixos** (~67%, ou $123 Mil) contra apenas ~33% de custos variáveis ($59 Mil) — ou seja, a empresa tem pouca margem de manobra para reduzir custo rapidamente.
- **Os cinco maiores itens de custo (Recrutamento, Licenças, Distribuição, Compras e Desenvolvimento) têm peso praticamente igual entre si** (entre $6,2 e $6,3 Mil cada) — não existe um único "vilão"; o gasto está distribuído.

## Recomendações

1. Investigar o que ocorreu especificamente em fevereiro e março (projeto pontual? renovação de contrato? erro de lançamento?), já que concentram praticamente todo o prejuízo do ano.
2. Priorizar a revisão de custos fixos (como licenças e distribuição) antes de cortar variáveis, já que representam a maior fatia do orçamento.
3. Acompanhar o padrão sazonal de dezembro para planejar melhor o fluxo de caixa nos meses de baixa (fev/mar).

## Sobre o dashboard

O dashboard permite filtrar por período e por centro de custo, e alternar a visão de custos entre Centro de Custo, Categoria e Lançamento (Descrição), facilitando o drill-down por quem for consumir a análise.

## Limitações

- A análise cobre apenas um ano fiscal (2024), o que não permite avaliar tendência plurianual.
- Os dados já vieram tratados de uma fonte externa; não houve etapa própria de limpeza/ETL documentada neste projeto.
- Não há detalhamento das causas específicas dos meses de prejuízo (fev/mar) — a recomendação é investigativa, não conclusiva.

## Estrutura do repositório

```
Grupo-Olz---Custos-e-Faturamento/
├── README.md
├── dashboard/
│   └── Financeiro_Custos_Dash.pbix
└── images/
    └── dashboard-overview.png
```

# Custos e Faturamento — Grupo OLZ

![Power BI](https://img.shields.io/badge/power_bi-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Power Query](https://img.shields.io/badge/power_query-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![MS OFFICE](https://img.shields.io/badge/Microsoft_Office-D83B01?style=for-the-badge&logo=microsoft-office&logoColor=white)
![Excel](https://img.shields.io/badge/Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Windows Terminal](https://img.shields.io/badge/Windows_Terminal-4D4D4D?style=for-the-badge&logo=windowsterminal&logoColor=white)
![Google Sheets](https://img.shields.io/badge/Google%20Sheets-34A853?style=for-the-badge&logo=google-sheets&logoColor=white)

---

## Visão geral

Projeto de visualização de dados construído em Power BI para apoiar a área contábil/financeira do Grupo OLZ na identificação de onde a empresa está perdendo dinheiro.  
O dashboard cruza faturamento, custos, resultado e margem, com quebras por mês, centro de custo e classe de custo, permitindo identificar rapidamente os períodos e categorias que mais impactam o resultado.

---

## Visualização

![Dashboard Grupo OLZ](images/dashboard-overview.png)

---

## Fonte dos dados

Os dados financeiros (faturamento, custos, resultado e margem) estão disponíveis em formato **CSV** na pasta `data`, permitindo visualização direta no GitHub.  
Eles cobrem o período de janeiro a dezembro de 2024 e já foram tratados previamente para uso no dashboard.

---

## Características

- Visualização de dados interativa: gráficos e tabelas dinâmicos.  
- Filtrar e pesquisar: filtros por data, categoria de produto, região e mais.  
- Tendências de custos: análise temporal para decisões informadas.  
- Desempenho: avaliação de diferentes áreas da empresa.  
- Exportar dados: download dos dados para análises posteriores.

---

## Indicadores principais (KPIs)

| Indicador   | Valor   |
|-------------|---------|
| Faturamento | $203 Mil |
| Custos      | $182 Mil |
| Resultado   | $21 Mil  |
| Margem      | 10,38%   |

---

## Recomendações

- Investigar o que ocorreu especificamente em fevereiro e março (projeto pontual? renovação de contrato? erro de lançamento?).  
- Priorizar revisão de custos fixos (licenças e distribuição) antes de cortar variáveis.  
- Acompanhar o padrão sazonal de dezembro para planejar melhor o fluxo de caixa nos meses de baixa (fev/mar).

---

## Limitações 

- A análise cobre apenas um ano fiscal (2024).  
- Os dados já vieram tratados de uma fonte externa; não houve etapa própria de limpeza/ETL documentada.  
- Não há detalhamento das causas específicas dos meses de prejuízo (fev/mar) — a recomendação é investigativa, não conclusiva.

---

## Estrutura do repositório

Grupo-Olz---Custos-e-Faturamento/
├── README.md
├── data/
│   └── Base_Financeira.csv
└── images/
└── dashboard-overview.png

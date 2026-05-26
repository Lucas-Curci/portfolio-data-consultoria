# Case 01 — Restaurante Sabor da Vila

## Arquivos deste case

| Arquivo | Descrição |
|---|---|
| `Case_Restaurante_SaborDaVila.xlsx` | Planilha com 4 abas: DADOS_PRODUTOS, HISTORICO_MENSAL, ANALISE_MARGEM, INSIGHTS |
| `Dashboard_Restaurante.pdf` | Dashboard exportado do Power BI |

## Estrutura da planilha Excel

### Aba 1 — DADOS_PRODUTOS
Dados de outubro/2024 por produto com colunas:
- Produto, Categoria, Canal (iFood/Salão/Ambos)
- Qtd_Vendida, Preco_Venda, Custo_Unitario
- Faturamento, Custo_Total, Lucro_Bruto (calculados por fórmula)
- Margem_Pct, Lucro_Unitario (calculados por fórmula)
- Classificacao (ESTRELA / POTENCIAL / REVISAR / OPORTUNIDADE)

### Aba 2 — HISTORICO_MENSAL
Série histórica de janeiro a outubro/2024:
- Faturamento e Custo_Total (dados brutos)
- Lucro_Bruto, Margem_Pct, CMV_Pct (fórmulas)
- Ticket_Medio, Qtd_Pedidos, Crescimento_Fat (fórmulas)
- Ordem_Mes (coluna auxiliar para ordenação no Power BI)

### Aba 3 — ANALISE_MARGEM
Visão consolidada de posicionamento:
- Referencia dados da aba DADOS_PRODUTOS via fórmulas
- Exibe Margem_Pct e Lucro_Unitario por produto
- Classificação de cada produto por rentabilidade

### Aba 4 — INSIGHTS
6 insights estratégicos formatados com título e descrição + ação recomendada.

## Fórmulas principais utilizadas

```excel
Faturamento      = Qtd_Vendida * Preco_Venda
Custo_Total      = Qtd_Vendida * Custo_Unitario
Lucro_Bruto      = Faturamento - Custo_Total
Margem_Pct       = Lucro_Bruto / Faturamento
Lucro_Unitario   = Preco_Venda - Custo_Unitario
CMV_Pct          = Custo_Total / Faturamento
Crescimento_Fat  = (Fat_Mes_Atual - Fat_Mes_Anterior) / Fat_Mes_Anterior
```

## Medidas DAX utilizadas no Power BI

```dax
Faturamento Total = SUM(DADOS_PRODUTOS[Faturamento])
Lucro Total       = SUM(DADOS_PRODUTOS[Lucro_Bruto])
Margem Media      = DIVIDE([Lucro Total], [Faturamento Total])
```

## Visuais do dashboard

1. **KPI Cards** — Faturamento Total, Lucro Total, Margem Média
2. **Gráfico de linha** — Evolução mensal de faturamento e lucro (jan–out)
3. **Barras horizontais** — Ranking de lucro por produto
4. **Segmentação** — Filtro por Canal de Venda (iFood / Salão / Ambos)

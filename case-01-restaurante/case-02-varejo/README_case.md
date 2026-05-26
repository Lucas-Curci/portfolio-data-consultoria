# Case 02 — Loja Estilo Mix

## Arquivos deste case

| Arquivo | Descrição |
|---|---|
| `Case_Varejo_EstiloMix.xlsx` | Planilha com 4 abas: DADOS_PRODUTOS, HISTORICO_MENSAL, ANALISE_ESTOQUE, INSIGHTS |
| `Dashboard_Varejo.pdf` | Dashboard exportado do Power BI |

## Estrutura da planilha Excel

### Aba 1 — DADOS_PRODUTOS
Dados de outubro/2024 por produto com colunas:
- Produto, Categoria
- Qtd_Vendida, Preco_Venda, Custo_Unitario
- Faturamento, Custo_Total, Lucro_Bruto (fórmulas)
- Margem_Pct (fórmula)
- Estoque_Atual, Dias_Cobertura (fórmula)
- Classificacao (ESTRELA / POTENCIAL / OK / OPORTUNIDADE)

### Aba 2 — HISTORICO_MENSAL
Série histórica de janeiro a outubro/2024:
- Faturamento, CMV (dados brutos)
- Lucro_Bruto, Margem_Pct (fórmulas)
- Devolucao, Fat_Liquido (fórmulas)
- Clientes_Novos, Clientes_Recorrentes, Taxa_Retorno (fórmula)
- Ordem_Mes (coluna auxiliar para ordenação no Power BI)

### Aba 3 — ANALISE_ESTOQUE
Visão de giro e cobertura de estoque:
- Dias_Cobertura = Estoque / Qtd_Vendida × 30
- Giro_Mensal = Qtd_Vendida / Estoque
- Status_Estoque (CRÍTICO / ATENÇÃO / OK / EXCESSO)

### Aba 4 — INSIGHTS
6 insights estratégicos com título, descrição e ação recomendada.

## Fórmulas principais utilizadas

```excel
Faturamento      = Qtd_Vendida * Preco_Venda
Custo_Total      = Qtd_Vendida * Custo_Unitario
Lucro_Bruto      = Faturamento - Custo_Total
Margem_Pct       = Lucro_Bruto / Faturamento
Dias_Cobertura   = ROUND(Estoque / Qtd_Vendida * 30, 1)
Giro_Mensal      = ROUND(Qtd_Vendida / Estoque, 1)
Fat_Liquido      = Faturamento - Devolucao
Taxa_Retorno     = Clientes_Recorrentes / (Clientes_Novos + Clientes_Recorrentes)
```

## Visuais do dashboard

1. **KPI Cards** — Faturamento Total, Margem Média, Lucro Bruto
2. **Gráfico de linha dupla** — Clientes novos vs recorrentes por mês
3. **Barras verticais** — Ranking de lucro por produto
4. **Dispersão** — Posicionamento de produtos: Margem vs Volume
3. **Gráfico de linha dupla** — Clientes novos vs recorrentes por mês
4. **Barras verticais** — Ranking de lucro por produto
5. **Dispersão** — Posicionamento de produtos: Margem vs Volume

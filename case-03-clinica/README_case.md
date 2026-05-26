# Case 03 — Clínica Viva Saúde

## Arquivos deste case

| Arquivo | Descrição |
|---|---|
| `Case_Clinica_VivaSaude.xlsx` | Planilha com 4 abas: DADOS_PROCEDIMENTOS, HISTORICO_MENSAL, RANKING_LUCRATIVIDADE, INSIGHTS |
| `Dashboard_Clinica.pdf` | Dashboard exportado do Power BI |

## Estrutura da planilha Excel

### Aba 1 — DADOS_PROCEDIMENTOS
Dados de outubro/2024 por procedimento com colunas:
- Procedimento, Area (Estética / Fisioterapia)
- Qtd_Realizadas, Ticket_Medio, Custo_Direto
- Faturamento, Custo_Total, Lucro_Bruto (fórmulas)
- Margem_Pct (fórmula)
- Duracao_Min, Lucro_Por_Hora (fórmula — métrica exclusiva deste case)
- Rank_Lucro_Hora (fórmula RANK)

### Aba 2 — HISTORICO_MENSAL
Série histórica de janeiro a outubro/2024:
- Faturamento, Custos_Fixos, Custos_Variaveis, Inadimplencia (dados brutos)
- Resultado_Liquido, Margem_Liquida (fórmulas)
- Atendimentos, Ticket_Medio (fórmula)
- Ordem_Mes (coluna auxiliar para ordenação no Power BI)

### Aba 3 — RANKING_LUCRATIVIDADE
Ranking dos 8 procedimentos ordenados por Lucro_Por_Hora decrescente:
- Lucro_Unitario = Ticket - Custo_Direto
- Lucro_Por_Hora = Lucro_Unitario / Duracao_Min × 60
- Lucro_Total_Mes = Lucro_Unitario × Qtd_Mes
- Part_Lucro_Total = Lucro_Total_Mes / Lucro_Total_Geral

### Aba 4 — INSIGHTS
6 insights estratégicos com título, descrição e ação recomendada.

## Fórmulas principais utilizadas

```excel
Faturamento       = Qtd_Realizadas * Ticket_Medio
Custo_Total       = Qtd_Realizadas * Custo_Direto
Lucro_Bruto       = Faturamento - Custo_Total
Margem_Pct        = Lucro_Bruto / Faturamento
Lucro_Por_Hora    = (Ticket_Medio - Custo_Direto) / Duracao_Min * 60
Resultado_Liquido = Faturamento - Custos_Fixos - Custos_Variaveis - Inadimplencia
Margem_Liquida    = Resultado_Liquido / Faturamento
Ticket_Medio      = ROUND(Faturamento / Atendimentos, 2)
```

## Métrica exclusiva — Lucro Por Hora

A métrica **Lucro_Por_Hora** é o principal diferencial deste case.  
Ela revela qual procedimento gera mais retorno por hora de sala ocupada — informação que nenhum dono de clínica acompanha normalmente.

| Procedimento | Lucro/Hora |
|---|---|
| Peeling Químico | R$ 224/h |
| Ultrassom Estético | R$ 150/h |
| RPG | R$ 135/h |
| Pilates Clínico | R$ 105,60/h |
| Fisioterapia Ortopédica | R$ 102/h |
| Avaliação Postural | R$ 93/h |
| Drenagem Linfática | R$ 88/h |
| Massagem Relaxante | R$ 82/h |

## Visuais do dashboard

1. **KPI Cards** — Faturamento Total, Lucro Total, Margem Média (%), Qtd Realizadas
2. **Gráfico de barras** — Lucro por hora por procedimento (com cores por ranking)
3. **Barras empilhadas** — Composição de custos mês a mês
4. **Rosca** — Faturamento por área (Estética vs Fisioterapia)

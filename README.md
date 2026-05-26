# 📊 Portfólio — Consultoria de Análise de Dados para PMEs

> Transformando dados de pequenas e médias empresas em decisões que aumentam o lucro.

**Lucas Curci** · Data Science — FIAP São Paulo  
📱 WhatsApp: (11) (11)919992-9572 · 

---

## 🧭 Sobre este portfólio

Este repositório reúne **3 cases de análise de dados** desenvolvidos para pequenas e médias empresas nos segmentos de alimentação, varejo e saúde.

Cada case inclui:
- 📁 Planilha Excel estruturada com dados brutos, análise de margem e histórico mensal
- 📊 Dashboard interativo em Power BI
- 💡 Relatório de insights com ações concretas e impacto financeiro estimado

**Stack utilizada:** Microsoft Excel · Power BI Desktop · Python (openpyxl, pandas)

---

## 📁 Estrutura do Repositório

```
portfolio-data-consultoria/
│
├── case-01-restaurante/
│   ├── Case_Restaurante_SaborDaVila.xlsx
│   ├── Dashboard_Restaurante.pdf
│   └── README_case.md
│
├── case-02-varejo/
│   ├── Case_Varejo_EstiloMix.xlsx
│   ├── Dashboard_Varejo.pdf
│   └── README_case.md
│
├── case-03-clinica/
│   ├── Case_Clinica_VivaSaude.xlsx
│   ├── Dashboard_Clinica.pdf
│   └── README_case.md
│
└── README.md
```

---

## 🍽️ Case 01 — Restaurante Sabor da Vila

**Segmento:** Restaurante com delivery (iFood) e atendimento no salão  
**Período analisado:** Janeiro a Outubro de 2024  
**Ferramentas:** Excel + Power BI

### Contexto
Restaurante de bairro em São Paulo com faturamento mensal de R$42.000, operando tanto no salão quanto via iFood. O proprietário não sabia quais pratos geravam mais lucro e tomava decisões de cardápio com base em volume de pedidos, não em margem.

### Problema identificado
Os produtos com maior volume de vendas **não eram** os mais lucrativos. A Marmita P liderava em pedidos, mas o Suco Natural tinha margem 21% maior e estava sendo subaproveitado.

### Principais métricas — Out/2024

| Indicador | Valor |
|---|---|
| Faturamento Total | R$ 42.357 |
| Lucro Bruto | R$ 25.490 |
| Margem Média | 60,2% |
| Produto mais lucrativo/hora | Suco Natural (75% de margem) |
| Crescimento jan→out | +30,7% |

### Top 3 Insights

**1. Suco Natural tem a maior margem (75%) mas só representa 3,8% do faturamento**  
→ Ação: criar combo prato + suco com desconto de R$2 — estimativa de +R$1.200/mês em lucro adicional

**2. Comissão do iFood reduz a margem da Marmita P de 61,9% para 38,8%**  
→ Ação: campanha para migração de clientes recorrentes para pedido direto via WhatsApp

**3. Prato Feito Carne é o único produto com margem abaixo de 55%**  
→ Ação: renegociar fornecedor ou reajustar preço de R$28,90 para R$31,90

### Visualizações
📄 [Ver Dashboard completo (PDF)](./case-01-restaurante/Dashboard_Restaurante.pdf)

---

## 👗 Case 02 — Loja Estilo Mix

**Segmento:** Varejo de moda feminina (loja física)  
**Período analisado:** Janeiro a Outubro de 2024  
**Ferramentas:** Excel + Power BI

### Contexto
Loja de roupas femininas em São Paulo com faturamento de R$41.000 em outubro. A proprietária não acompanhava giro de estoque, taxa de retorno de clientes nem margem por produto — gerenciava o negócio pelo feeling de quais peças "vendiam mais".

### Problema identificado
O produto com maior margem (Acessórios, 77,4%) estava com estoque em excesso e sem destaque na loja. Enquanto isso, itens com menor margem ocupavam o espaço principal.

### Principais métricas — Out/2024

| Indicador | Valor |
|---|---|
| Faturamento Total | R$ 41.244 |
| Lucro Bruto | R$ 26.700 |
| Margem Média | 70,0% |
| Taxa de Retorno de Clientes | 35% (era 28% em jan) |
| Crescimento jan→out | +83,9% |

### Top 3 Insights

**1. Acessórios: maior margem (77,4%) + maior volume (120 un) = produto ignorado**  
→ Ação: display no caixa + treino de equipe para oferecer como complemento em toda compra

**2. Devoluções custaram R$13.610 acumulados em 10 meses (4,8% do faturamento)**  
→ Ação: mapear os 2 produtos com maior índice e adicionar tabela de medidas detalhada

**3. Taxa de retorno de clientes cresceu de 28% para 35% — tendência positiva**  
→ Ação: programa de fidelidade via WhatsApp — 4ª compra com 10% de desconto

### Visualizações
📄 [Ver Dashboard completo (PDF)](./case-02-varejo/Dashboard_Varejo.pdf)

---

## 🏥 Case 03 — Clínica Viva Saúde

**Segmento:** Clínica de estética e fisioterapia  
**Período analisado:** Janeiro a Outubro de 2024  
**Ferramentas:** Excel + Power BI

### Contexto
Clínica com 8 procedimentos entre estética e fisioterapia, faturamento de R$57.500 em outubro e 410 atendimentos no mês. A gestora organizava a agenda por demanda dos clientes, sem considerar qual procedimento gerava mais retorno por hora de sala ocupada.

### Problema identificado
O Peeling Químico gerava **R$224/hora de lucro** — o maior da clínica — mas tinha apenas 28 realizações no mês por falta de divulgação. A Massagem Relaxante, com menor retorno por hora (R$82), ocupava a maior parte da agenda.

### Principais métricas — Out/2024

| Indicador | Valor |
|---|---|
| Faturamento Total | R$ 57.540 |
| Resultado Líquido | R$ 27.840 |
| Margem Líquida | 48,4% |
| Procedimento mais lucrativo/hora | Peeling Químico (R$224/h) |
| Crescimento do resultado líquido jan→out | +77,9% |

### Top 3 Insights

**1. Peeling Químico gera R$224/hora mas só tem 28 realizações no mês**  
→ Ação: pacote "3 sessões de Peeling" com 10% de desconto — estimativa de +R$4.700/mês

**2. Inadimplência acumulou R$18.540 em 10 meses sem controle**  
→ Ação: cobrar 50% no agendamento via PIX — redução estimada de 60% na inadimplência

**3. Custos fixos caíram de 35,9% para 25,7% do faturamento — margem de escala disponível**  
→ Ação: contratar profissional part-time focado em Peeling e Massagem — ROI positivo no 1º mês

### Visualizações
📄 [Ver Dashboard completo (PDF)](./case-03-clinica/Dashboard_Clinica.pdf)

---

## 🛠️ Metodologia de trabalho

```
1. COLETA         → Template de planilha por nicho + 5 perguntas de kickoff
2. LIMPEZA        → Padronização, remoção de duplicatas, tipagem correta
3. ANÁLISE        → Margem % por produto, cruzamento volume × margem, histórico
4. VISUALIZAÇÃO   → Dashboard em Power BI com KPIs, tendências e rankings
5. NARRATIVA      → Relatório: Situação → Problema → Impacto (R$) → Ação
6. APRESENTAÇÃO   → Call de 30 min com o cliente + proposta de acompanhamento
```

---

## 💼 Serviços oferecidos

| Serviço | Entrega | Investimento |
|---|---|---|
| **Diagnóstico Pontual** | Relatório PDF + reunião 30min | R$ 350 |
| **Dashboard Mensal** | Power BI atualizado + call mensal | R$ 700/mês |
| **Consultoria Estratégica** | Dashboard + análises + recomendações | R$ 1.500/mês |

---

## 📬 Contato

Atendo PMEs em São Paulo e região. Se você quer saber quais produtos do seu negócio estão gerando mais lucro — e quais estão drenando margem — me chama.

📱 **WhatsApp:** (11) (11)919992-9572
🌐 **Site:**   
📧 **E-mail:** 
💼 **LinkedIn:** 

---

*Cases desenvolvidos com dados simulados representativos dos respectivos segmentos de mercado.*

# Graph Report - processo-iveco-stralis  (2026-10-28)

## Corpus Check
- Corpus is ~16,293 words - fits in a single context window. You may not need a graph.

## Summary
- 26 nodes · 34 edges · 5 communities (4 shown, 1 thin omitted)
- Extraction: 91% EXTRACTED · 9% INFERRED · 0% AMBIGUOUS · INFERRED: 3 edges (avg confidence: 0.85)
- Token cost: 75,142 input · 0 output

## Community Hubs (Navigation)
- Processo administrativo e judicial
- Caminhão e peças ausentes
- Leilão e página do site
- Custos e prejuízo
- Pedido do arrematante

## God Nodes (most connected - your core abstractions)
1. `Iveco Stralis HD 450S38TN1 HGB-3830` - 5 edges
2. `B.O. 2026/1215307 (furto simples, Paiçandu)` - 5 edges
3. `Of. 127/2026-CEPSD (negativa)` - 4 edges
4. `Linha do tempo` - 4 edges
5. `Dossiê: documentos reunidos` - 4 edges
6. `Processo Iveco Stralis page (index.html)` - 3 edges
7. `Leilão SENAD/PR 08/2026 Lote 13` - 3 edges
8. `Pedido de desfazimento da compra` - 3 edges
9. `Edital 790460 (itens 3.6, 3.7, 6.4)` - 3 edges
10. `Peças ausentes e danos (cabeçote, injetores, comando)` - 3 edges

## Surprising Connections (you probably didn't know these)
- `Leilão SENAD/PR 08/2026` --semantically_similar_to--> `Leilão SENAD/PR 08/2026 Lote 13`  [INFERRED] [semantically similar]
  README.md → index.html
- `Processo Iveco Stralis (README)` --references--> `Processo Iveco Stralis page (index.html)`  [EXTRACTED]
  README.md → index.html
- `Vercel deploy (no build)` --rationale_for--> `Processo Iveco Stralis page (index.html)`  [EXTRACTED]
  README.md → index.html

## Import Cycles
- None detected.

## Hyperedges (group relationships)
- **Disputa administrativa do desfazimento** — index_pedido_desfazimento, index_posicao_arrematante, index_posicao_comissao, index_oficio_127_2026_cepsd, index_motor_a_regularizar_vs_ausencia [EXTRACTED 1.00]
- **Cadeia de origem do veículo (apreensão a leilão)** — index_acao_penal_0002664_32_2023, index_auto_apreensao, index_processo_sei_08129_004583_2025_70, index_leilao_senad_pr_08_2026, index_iveco_stralis_hgb_3830 [INFERRED 0.85]

## Communities (5 total, 1 thin omitted)

### Community 0 - "Processo administrativo e judicial"
Cohesion: 0.33
Nodes (6): Ação Penal 0002664-32.2023.8.16.0210 (Vara Criminal de Paiçandu), Comissão de Avaliação e Alienação de Bens do Paraná, Dossiê: documentos reunidos, Edital 790460 (itens 3.6, 3.7, 6.4), Of. 127/2026-CEPSD (negativa), Processo SEI 08129.004583/2025-70

### Community 1 - "Caminhão e peças ausentes"
Cohesion: 0.33
Nodes (5): Auto de exibição e apreensão (caminhão 'avariado'), Iveco Stralis HD 450S38TN1 HGB-3830, Pátio credenciado em Maringá/PR, Peças ausentes e danos (cabeçote, injetores, comando), SENAD / Ministério da Justiça e Segurança Pública

### Community 2 - "Leilão e página do site"
Cohesion: 0.33
Nodes (5): CSS design tokens with light/dark theme, Leilão SENAD/PR 08/2026 Lote 13, Processo Iveco Stralis page (index.html), Leilão SENAD/PR 08/2026, Processo Iveco Stralis (README)

### Community 3 - "Custos e prejuízo"
Cohesion: 0.50
Nodes (4): Semirreboque SR Guerra (Leilão de Dourados, Edital 07/2026), Custos documentados (R$ 45.810,77), Prejuízo total R$ 78.500, Linha do tempo

## Knowledge Gaps
- **2 isolated node(s):** `SENAD / Ministério da Justiça e Segurança Pública`, `CSS design tokens with light/dark theme`
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 3 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)
- **1 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `Leilão SENAD/PR 08/2026 Lote 13` connect `Leilão e página do site` to `Caminhão e peças ausentes`, `Custos e prejuízo`?**
  _High betweenness centrality (0.400) - this node is a cross-community bridge._
- **What connects `SENAD / Ministério da Justiça e Segurança Pública`, `CSS design tokens with light/dark theme` to the rest of the system?**
  _2 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Why does `Linha do tempo` connect `Custos e prejuízo` to `Processo administrativo e judicial`, `Leilão e página do site`, `Pedido do arrematante`?**
  _High betweenness centrality (0.353) - this node is a cross-community bridge._
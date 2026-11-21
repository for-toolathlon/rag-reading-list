# RAG Reading Group Literature Scan — Digest

**Prepared for:** RAG reading group
**Scope:** Recent arXiv preprints on retrieval-augmented generation (RAG)
**Date:** 2026-11-21
**Method:** Four-quadrant scan of arXiv search results (core RAG methods, agentic/multi-step retrieval, long-context vs. retrieval, RAG evaluation/benchmarks); candidates ranked for relevance to RAG. Final six assigned to exactly one theme from {efficiency, reasoning, multimodality, safety}. Runner-up themes noted where a paper arguably fits two.

## Selected preprints (must-read, worth skimming, or background)

### Must-read

1. **2005.11401** — *Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks* (Lewis et al., 2020)
   - A foundational RAG paper establishing that RAG produces more specific, diverse, and factual language than parametric-only baselines. Canonical deployment definition of RAG.

### Worth skimming

2. **2312.10997** — *Retrieval-Augmented Generation for Large Language Models: A Survey* (Gao et al., 2023)
   - Comprehensive survey of RAG paradigm progression (Naive → Advanced). Nice for orientation.

3. **2607.24748** — *VLD-RAG: Agentic Vision-Language RAG for Long, Visually-Rich Multi-Page Documents* (Kim et al., 2026)
   - Agentic multimodal retrieval; effectively multimodality + agentic themes (runner-up noted).

4. **2504.18041** — *RAG LLMs are Not Safer: A Safety Analysis of RAG for LLMs* (An et al., 2025)
   - Found RAG can make models less safe and change safety profile. Must read for safety angle.

5. **2505.20096** — *MA-RAG: Multi-Agent RAG via Collaborative Chain-of-Thought Reasoning* (Nguyen et al., 2025)
   - Multi-agent retrieval with chain-of-thought reasoning; efficiency and reasoning (runner-up noted).

6. **2412.18232** — *Efficient Long Context Language Model Retrieval with Compression* (Seo et al., 2025)
   - Retains 6% retrieval performance gain while compressing context 1.91×; efficiency.

### Background

- **2005.11401** (already noted as must-read) — foundational RAG.
- **2312.10997** (already noted as skimming) — survey.
- **2505.20096** (already noted as worth skimming) — MA-RAG.
- **2412.18232** (already noted as must-read) — compression / efficiency.

## Theme breakdown

| Theme        | Paper (arXiv ID, date) |
|--------------|-------------------------|
| Efficiency   | 2412.18232 (2025)       |
| Reasoning    | 2505.20096 (2025)       |
| Multimodality| 2607.24748 (2026)       |
| Safety       | 2504.18041 (2025)       |

- Ambiguous runners-up: core RAG methods (2005.11401, 2312.10997) and MA-RAG/agentic reasoning run concurrently with agentic/multimodal themes, but assigned to their primary angle.
- 2505.20096 also intersects with reasoning; note as runner-up.
- 2607.24748 also touches agentic retrieval, but assigned to multimodality.

## Recent developments (web chatter)

Recent web coverage notes that agentic/multi-step retrieval and long-context LLMs remain the hottest debate points (per arXiv and industry coverage from Feb–Aug 2026). RAG evaluation benchmarks (GaRAGe, RAGPerf, DRAGON, long²RAG) are gaining traction 2025–2026. One notable gap: chatter around RAG's safety profile (2504.18041) is underweighted on web news; worth flagging.

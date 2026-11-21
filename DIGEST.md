# RAG Reading Group — Literature Scan Digest

_Prepared 2026 by the group's week-0 anchor. Searches of recent arXiv preprints on retrieval-augmented generation (RAG) across four angles: core RAG methods, agentic/multi-step retrieval, long-context vs retrieval, and RAG evaluation/benchmarks. Six papers selected, each mapped to exactly one of the four work themes: efficiency, reasoning, multimodality, safety. Must-reads deserve detail from arXiv abstracts; others get a one-liner._

## Selected papers

### 1. arXiv:2407.16833 — "Retrieval Augmented Generation or Long-Context LLMs?"
**Date: Jul 23, 2024** — Must-read
Direct comparison of RAG vs long-context LLMs (LCs). When LCs are suffciently resourced, LCs outperform RAG in average performance, but RAG is significantly more cost-efficient — the key efficiency tradeoff RAG reads groups cite.

### 2. arXiv:2506.05167 — "ECoRAG: Evidentiality-guided Compression for Long Context RAG"
**Date: Jun 6, 2025** — Worth skimming
Highly cost-efficient compression that reduces latency and token usage by retaining only necessary evidence for long-context RAG — a strong efficiency paper the group should watch.

### 3. arXiv:2501.01880 — "Long Context vs. RAG for LLMs: An Evaluation and Revisits"
**Date: Dec 27, 2024** — Background
Re-evaluates whether long-context LLMs (LCs) broadly beat RAG; shows LC generally outperforms RAG on QA benchmarks, especially Wikipedia-based questions, with summarization-based retrieval giving comparable results.

### 4. arXiv:2505.11180 — "mmRAG: A Modular Benchmark for RAG"
**Date: May 16, 2025** — Must-read
Modular benchmark integrating six diverse QA datasets (text, tables, knowledge graphs) for multimodal RAG evaluation — validates the evaluation angle.

### 5. arXiv:2605.08838 — "Generating Leakage-Free Benchmarks for Robust RAG"
**Date: May 9, 2026** — Must-read
Datasets designed to test RAG performance that must leak-free, addressing a key safety/spread-capability issue for robust evaluation.

### 6. arXiv:2603.07379 — "SoK: Agentic Retrieval-Augmented Generation (RAG)"
**Date: Mar 7, 2026** — Background
Systematic survey defining agentic RAG by an autonomous control policy governing retrieval — the reasoning/agentic-angle reference.

## Theme breakdown

| Theme       | Papers (arXiv ID / date) |
|-------------|--------------------------|
| efficiency  | 2407.16833 (Jul 2024), 2506.05167 (Jun 2025), 2501.01880 (Dec 2024) |
| reasoning   | 2603.07379 (Mar 2026)    |
| multimodality | 2505.11180 (May 2025)   |
| safety      | 2605.08838 (May 2026)    |

Runner-up note: 2501.01880 also arguably fits efficiency; 2603.07379 also arguably fits agentic reasoning.

## Flags

- Must-read — arXiv:2407.16833 (Jul 23, 2024). Core efficiency-tradeoff debate: RAG is cheaper than long-context LLMs when properly resourced.
- Must-read — arXiv:2505.11180 (May 16, 2025). mmRAG benchmarks multimodal RAG across text, tables, and knowledge graphs.
- Must-read — arXiv:2605.08838 (May 9, 2026). Leakage-free benchmarks to make robust RAG evaluation honest and non-parametric-aliasable.
- Worth skimming — arXiv:2506.05167 (Jun 6, 2025). Cost-efficient evidence compression for long-context RAG.
- Background — arXiv:2501.01880 (Dec 27, 2024). LC vs RAG evaluation with costs.
- Background — arXiv:2603.07379 (Mar 7, 2026). Agentic RAG survey / SoK on autonomous control policy.

## Internet chatter — Recent developments

The wider web is treating RAG as in its definitive benchmark/comparison phase: "Retrieval Augmented Generation or Long-Context LLMs?" gains strong RAG endorsement when context is insufficient for LCs; mmRAG (arXiv:2505.11180) leads the new-modality benchmark wave, especially for text-plus-KG; agentic RAG is expanding from survey (arXiv:2603.07379) to practical frameworks (ARAG/ALT, arXiv:2602.03442); and a debate on leakage-free robustness benchmarks is gaining prominence (arXiv:2605.08838). Notably, the chatter circles around multimodality and robust-evaluation safety rather than pure efficiency, so the group can broaden discussion if desired.

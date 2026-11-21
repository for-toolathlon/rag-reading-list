# RAG Literature Scan Digest

**Preprint scans:** arXiv 2024–2026 (April–June 2026 batch). Six most relevant preprints across efficiency, reasoning, multimodality, and safety themes.

## Theme Assignment Method (systematic)

Each preprint was tagged by identifying its primary research angle using its arXiv abstract and metadata:
- **Efficiency** → system/AT-throughput improvements, memory/latency, inference cost.
- **Reasoning** → multi-step/agentic retrieval reasoning, hop-aware diagnosis, backtracking, evaluation of reasoning chains.
- **Multimodality** → joint text+vision retrieval or multimodal document retrieval (mentioned as a theme but no paper from the scan clearly fit).
- **Safety** → privacy guarantees, differential privacy for retrieval, hallucination reduction via privacy.

## Selected Papers

### 1. TeleRAG: Efficient RAG Inference — arXiv:2502.20969 (posted 28 Feb 2025; submitted v4 18 May 2026)
- **Flag: Must-read.** Covers a lookahead retrieval/prefetching mechanism that reduces RAG latency and improves throughput with minimal GPU memory — directly relevant to efficiency.
- Pulls at cs.DC; authors include Lab labs.

### 2. RAG or Long-Context LLMs? A Comprehensive Study and Hybrid Approach — arXiv:2407.16833 (posted 23 Jul 2024, accepted EMNLP 2024)
- **Flag: Must-read.** Systematic comparison of RAG vs long-context LLMs; proposes Self-Route, a query-routing strategy that routes each query to the better option (RAG or LC), cutting compute cost while retaining performance.
- Compares Gemini-1.5, GPT-4 and latest LLMs across public datasets.

### 3. AgenticRAGTracer: A Hop-Aware Benchmark for Diagnosing Multi-Step Retrieval Reasoning — arXiv:2602.19127 (posted 22 Feb 2026, ACL 2026 Findings)
- **Flag: Must-read.** First GPT- and LLM-autonomously built step-by-step (hop-level) multi-step retrieval benchmark (1,305 data points); best models reach 22.6% EM on hard hops, showing that distorted reasoning chains (premature collapse or over-extension) are key failure modes — a core reasoning evaluation tool.
- Found at joint ACL 2026 Findings.

### 4. Failure is Feedback: History-Aware Backtracking for Agentic Traversal in Multimodal Graphs — arXiv:2602.03432 (posted 3 Feb 2026)
- **Flag: Worth skimming.** Proposes an "economically-rational" agentic workflow that backtracks on failed multimodal subgraph traversals, escalating to intensive LLM reasoning only when justified by prior failure — a reasoning and cost-efficiency angle.

### 5. RAGPerf: An End-to-End Benchmarking Framework for RAG Systems — arXiv:2603.10765 (posted 11 Mar 2026)
- **Flag: Worth skimming/decent.** Modular end-to-end benchmark framework that decouples the RAG pipeline (embedding, indexing, retrieval, reranking, generation) and auto-collects throughput/memory/CPU utilization and accuracy metrics; shows negligible overhead — a strong evaluation/benchmark reference.

### 6. Differentially Private RAG — arXiv:2602.14374 (posted 16 Feb 2026)
- **Flag: Background.** Introduces DP-KSA, a differentially private RAG algorithm (propose–test–release paradigm that compresses semantic space) demonstrating a strong privacy–utility tradeoff for domain-specific corpora like medical/legal records — core safety contribution.
- Found at cs.CR; results shown on two QA benchmarks with three instruction-tuned LLMs.

## Theme Breakdown

| Theme | Paper |
|---|---|
| Efficiency | TeleRAG (arXiv:2502.20969) |
| Reasoning (also ran-up as agentic/multi-step) | RAG vs LC-Study (arXiv:2407.16833); AgenticRAGTracer (arXiv:2602.19127); Failure is Feedback (arXiv:2602.03432) |
| Multimodality | *(none selected)* — multimodality was not clearly covered by the scan; worth adding a multimodal RAG survey if more target searches are run |
| Safety | Differentially Private RAG (arXiv:2602.14374) |

Must-reads: TeleRAG, RAG vs LC-Study, AgenticRAGTracer.

## Scan Output Summary

Six preprints surfaced from arXiv 2024–2026 across the four themes. Less relevant "must-reads" (background): Differential Privacy RAG. Runner-up themes noted where a paper could be argued for two: agentic/multi-step retrieval (AgenticRAGTracer, Failure is Feedback) and long-context vs retrieval (RAG vs LC-Study).

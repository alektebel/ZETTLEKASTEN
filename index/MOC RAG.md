# MOC: Retrieval-Augmented Generation (RAG)

date: 2026-06-12
tags: #index #moc #rag
topic: RAG — retrieval-augmented generation

---

## What this map covers

The full landscape of RAG: from foundational architectures to advanced retrieval strategies, indexing methods, evaluation, and graph-based approaches. Goal: understand SOTA well enough to build and evaluate production RAG systems.

---

## Reading order

### 1. Foundations (read first)
- [[Gao 2023 RAG Survey]] — read this first; it's the map of the entire field
- [[Lewis 2020 RAG for Knowledge-Intensive NLP Tasks]] — the original RAG paper; coined the term
- [[Guu 2020 REALM Retrieval-Augmented Language Model Pre-Training]] — retrieval at pre-training time
- [[Izacard 2021 Fusion-in-Decoder]] — FiD; how to scale to many retrieved passages

### 2. Advanced retrieval techniques
- [[Gao 2022 HyDE Precise Zero-Shot Dense Retrieval]] — query expansion via hypothetical documents
- [[Jiang 2023 FLARE Active Retrieval]] — retrieve only when uncertain
- [[Asai 2023 Self-RAG]] — LLM that decides when and what to retrieve, self-critiques output
- [[Yan 2024 CRAG Corrective Retrieval]] — corrective loop when retrieval quality is low

### 3. Indexing and structure
- [[Sarthi 2024 RAPTOR]] — hierarchical tree indexing for multi-hop questions
- [[Edge 2024 GraphRAG]] — knowledge graph indexing for global/sensemaking queries

### 4. Evaluation
- [[Es 2023 RAGAS Evaluation Framework]] — automated metrics: faithfulness, relevancy, precision, recall

---

## Core tensions in the field

- [[Asai 2023 Self-RAG]] vs. [[Jiang 2023 FLARE Active Retrieval]] — different approaches to adaptive retrieval
- [[Sarthi 2024 RAPTOR]] vs. [[Edge 2024 GraphRAG]] — tree summaries vs. knowledge graphs for synthesis
- RAG vs. long-context LLMs — does better context window make retrieval obsolete?

---

## Open questions I'm exploring

- What is the right chunking strategy for different document types?
- When does RAG outperform full fine-tuning, and vice versa?
- How do you evaluate RAG faithfulness reliably at scale?
- Can GraphRAG and vector RAG be combined effectively?

---

## Connected MOCs

- [[MOC LLMs]]
- [[MOC Information Retrieval]]

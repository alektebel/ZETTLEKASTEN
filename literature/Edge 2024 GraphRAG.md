# Edge 2024 — From Local to Global: A Graph RAG Approach to Query-Focused Summarization

date: 2026-06-12
tags: #literature #rag #advanced #graph #knowledge-graph
type: paper
source: https://arxiv.org/abs/2404.16130
author: Darren Edge et al. (Microsoft Research)
year: 2024
status: unread

---

## In one sentence

Builds a knowledge graph from the corpus (entities + relationships + community summaries), then retrieves at the community level to answer global questions no chunk-based RAG can handle.

---

## Key ideas

1. Two-phase: offline graph construction (entity/relation extraction + community detection), online query with community summaries
2. Global queries ("What are the main themes?") require a different retrieval unit than local queries ("What did X say about Y?")
3. Community summaries pre-aggregate information — generation becomes summarization of summaries
4. Much more expensive to index than flat RAG; trade-off is query quality for global questions

---

## Quotes worth keeping

> "Vector RAG performs better for low-level queries, GraphRAG for high-level sensemaking"

---

## My reaction

[Fill after reading]

---

## Permanent notes to write

- [ ] [[]] — Global vs. local queries require fundamentally different retrieval strategies
- [ ] [[]] — Knowledge graphs as a retrieval unit above the chunk level

---

## Links to existing notes

- [[Sarthi 2024 RAPTOR]]
- [[MOC RAG]]

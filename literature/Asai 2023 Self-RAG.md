# Asai 2023 — Self-RAG: Learning to Retrieve, Generate, and Critique through Self-Reflection

date: 2026-06-12
tags: #literature #rag #advanced #self-reflection
type: paper
source: https://arxiv.org/abs/2310.11511
author: Akari Asai et al. (UW / AI2)
year: 2023
status: unread

---

## In one sentence

A single LLM that decides when to retrieve, critiques its own outputs with special reflection tokens, and can skip retrieval entirely when it's unnecessary.

---

## Key ideas

1. Special tokens: [Retrieve], [IsRel], [IsSup], [IsUse] — model learns to self-assess
2. Adaptive retrieval: retrieves only when needed, unlike naive RAG which always retrieves
3. Outperforms ChatGPT and retrieval-augmented Llama2 on several benchmarks while being smaller

---

## Quotes worth keeping

> "Self-RAG trains a single LM to adaptively retrieve passages on demand, and generate and reflect on retrieved passages"

---

## My reaction

[Fill after reading]

---

## Permanent notes to write

- [ ] [[]] — Adaptive retrieval vs. always-retrieve RAG
- [ ] [[]] — Self-critique as a training signal

---

## Links to existing notes

- [[Jiang 2023 FLARE Active Retrieval]]
- [[MOC RAG]]

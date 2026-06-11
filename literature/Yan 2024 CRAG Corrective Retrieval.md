# Yan 2024 — CRAG: Corrective Retrieval Augmented Generation

date: 2026-06-12
tags: #literature #rag #advanced #self-correction
type: paper
source: https://arxiv.org/abs/2401.15884
author: Shi-Qi Yan et al.
year: 2024
status: unread

---

## In one sentence

Adds a lightweight retrieval evaluator that scores retrieved documents and triggers a corrective web search when confidence is low, before passing context to the generator.

---

## Key ideas

1. Three actions based on retrieval confidence: Correct / Incorrect / Ambiguous
2. When incorrect → web search fallback for fresher or broader coverage
3. Knowledge refinement step: strips irrelevant content from retrieved docs before generation
4. Plug-and-play: can wrap any existing RAG pipeline

---

## Quotes worth keeping

> "The retrieval evaluator is key to CRAG's ability to correct retrieval errors before they propagate to generation"

---

## My reaction

[Fill after reading]

---

## Permanent notes to write

- [ ] [[]] — RAG failure modes: retrieval error propagates silently to generation

---

## Links to existing notes

- [[Asai 2023 Self-RAG]]
- [[MOC RAG]]

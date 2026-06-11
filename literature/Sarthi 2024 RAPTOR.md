# Sarthi 2024 — RAPTOR: Recursive Abstractive Processing for Tree-Organized Retrieval

date: 2026-06-12
tags: #literature #rag #advanced #indexing #hierarchical
type: paper
source: https://arxiv.org/abs/2401.18059
author: Parth Sarthi et al. (Stanford)
year: 2024
status: unread

---

## In one sentence

Builds a tree of summaries by recursively clustering and summarizing chunks, then retrieves from all levels — solves multi-hop and high-level questions that flat chunk retrieval misses.

---

## Key ideas

1. Bottom-up: chunk → cluster → summarize → repeat until root
2. At query time, retrieve from any level of the tree (collapsed or tree-traversal modes)
3. Excels at questions requiring synthesis across many passages, not just local lookup

---

## Quotes worth keeping

> "RAPTOR constructs a recursive tree structure that balances both high-level themes and granular details"

---

## My reaction

[Fill after reading]

---

## Permanent notes to write

- [ ] [[]] — Hierarchical indexing solves the multi-hop retrieval problem
- [ ] [[]] — Chunk granularity mismatch: why flat retrieval fails for synthesis questions

---

## Links to existing notes

- [[MOC RAG]]

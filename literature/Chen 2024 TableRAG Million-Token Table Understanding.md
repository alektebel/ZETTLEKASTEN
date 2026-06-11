# Chen 2024 — TableRAG: Million-Token Table Understanding with Retrieval Augmentation

date: 2026-06-12
tags: #literature #rag #structured-data #tables
type: paper
source: https://arxiv.org/abs/2410.04739
author: Si-An Chen et al. (Google)
year: 2024
status: unread

---

## In one sentence

RAG specifically designed for tabular data: separately indexes schema (column names + types) and cell values into a vector store, then retrieves only the relevant schema + cells needed to answer a query — avoids stuffing entire tables into context.

---

## Key ideas

1. Two separate indices: schema index (column metadata) + cell value index (actual data)
2. Schema retrieval: find which columns are relevant to the query
3. Cell retrieval: find which specific values appear in the data
4. Scales to million-row tables where full-table context is impossible
5. Crucial insight: columns and values have very different retrieval needs

---

## Why it matters for the compliance audit system

Your DB has many tables with many columns. You can't dump everything into context.
TableRAG gives you the architecture:
- Vector index of column names/descriptions → retrieve relevant columns for a regulation rule
- Vector index of cell values → retrieve suspicious values before running full SQL

---

## Quotes worth keeping

> "Separating schema retrieval and cell retrieval is critical — conflating them degrades performance significantly"

---

## My reaction

[Fill after reading]

---

## Permanent notes to write

- [ ] [[]] — Schema index vs. cell index: two different retrieval problems in structured data RAG
- [ ] [[]] — Scaling RAG to tabular data requires column-level granularity

---

## Links to existing notes

- [[Gao 2023 RAG Survey]]
- [[MOC Compliance Audit Agent]]
- [[MOC RAG]]

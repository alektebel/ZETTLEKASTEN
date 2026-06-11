# Gao 2022 — Precise Zero-Shot Dense Retrieval without Relevance Labels (HyDE)

date: 2026-06-12
tags: #literature #rag #retrieval #query-expansion
type: paper
source: https://arxiv.org/abs/2212.10496
author: Luyu Gao et al. (CMU)
year: 2022
status: unread

---

## In one sentence

HyDE: use an LLM to hallucinate a hypothetical document answering the query, then use that document's embedding to retrieve real documents — bridges the query-document gap.

---

## Key ideas

1. Queries and documents live in different embedding spaces; a hypothetical answer is closer to real documents than the raw query
2. Works zero-shot: no labeled data needed
3. Simple and effective — just one LLM call before retrieval

---

## Quotes worth keeping

> "Hyde instructs an LLM to generate a hypothetical document to encode, rather than encoding the query directly"

---

## My reaction

[Fill after reading]

---

## Permanent notes to write

- [ ] [[]] — Query-document embedding gap and how to bridge it

---

## Links to existing notes

- [[MOC RAG]]

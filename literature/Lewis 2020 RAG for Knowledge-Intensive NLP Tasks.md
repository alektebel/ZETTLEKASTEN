# Lewis 2020 — Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks

date: 2026-06-12
tags: #literature #rag #foundational
type: paper
source: https://arxiv.org/abs/2005.11401
author: Patrick Lewis et al. (Facebook AI)
year: 2020
status: unread

---

## In one sentence

The paper that coined "RAG": combines a dense retriever (DPR) with a seq2seq generator (BART), jointly trained end-to-end.

---

## Key ideas

1. Two variants: RAG-Sequence (retrieve once per answer) and RAG-Token (retrieve per token)
2. Non-parametric memory (retrieval) + parametric memory (LM weights) complement each other
3. Knowledge can be updated without retraining by swapping the document index

---

## Quotes worth keeping

> "We combine parametric and non-parametric memory for language generation"

---

## My reaction

[Fill after reading]

---

## Permanent notes to write

- [ ] [[]] — RAG as parametric + non-parametric memory fusion
- [ ] [[]] — When retrieval beats fine-tuning for knowledge tasks

---

## Links to existing notes

- [[MOC RAG]]

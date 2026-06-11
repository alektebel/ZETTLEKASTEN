# Es 2023 — RAGAS: Automated Evaluation of Retrieval Augmented Generation

date: 2026-06-12
tags: #literature #rag #evaluation
type: paper
source: https://arxiv.org/abs/2309.15217
author: Shahul Es et al.
year: 2023
status: unread

---

## In one sentence

A reference-free evaluation framework for RAG pipelines with four metrics: faithfulness, answer relevancy, context precision, and context recall.

---

## Key ideas

1. Faithfulness: does the answer follow from the retrieved context? (hallucination detection)
2. Answer relevancy: does the answer address the question?
3. Context precision: is the retrieved context ranked well? Are relevant chunks at the top?
4. Context recall: did retrieval surface all the necessary information?
5. All metrics are computed using an LLM-as-judge — no human labels needed

---

## Quotes worth keeping

> "RAGAS provides a suite of metrics that can evaluate RAG pipelines without requiring ground truth labels"

---

## My reaction

[Fill after reading]

---

## Permanent notes to write

- [ ] [[]] — The four axes of RAG quality: faithfulness, relevance, precision, recall
- [ ] [[]] — LLM-as-judge enables scalable evaluation without human annotation

---

## Links to existing notes

- [[MOC RAG]]

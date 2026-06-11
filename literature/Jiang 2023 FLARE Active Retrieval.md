# Jiang 2023 — Active Retrieval Augmented Generation (FLARE)

date: 2026-06-12
tags: #literature #rag #advanced #active-retrieval
type: paper
source: https://arxiv.org/abs/2305.06983
author: Zhengbao Jiang et al. (CMU)
year: 2023
status: unread

---

## In one sentence

FLARE retrieves only when the model is uncertain — detected by low-probability tokens in the generation — then reformulates the query from the upcoming sentence.

---

## Key ideas

1. Retrieval triggered by uncertainty (token probability below threshold), not by fixed intervals
2. Uses the partially generated sentence as a search query — more contextually grounded than the original question
3. Iterative generation: generate → check uncertainty → retrieve if needed → continue

---

## Quotes worth keeping

> "An active retrieval approach that anticipates future content and proactively retrieves when necessary"

---

## My reaction

[Fill after reading]

---

## Permanent notes to write

- [ ] [[]] — Token probability as a proxy for knowledge uncertainty

---

## Links to existing notes

- [[Asai 2023 Self-RAG]]
- [[MOC RAG]]

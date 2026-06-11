# Izacard 2021 — Leveraging Passage Retrieval with Generative Models for Open Domain QA (FiD)

date: 2026-06-12
tags: #literature #rag #foundational #fusion
type: paper
source: https://arxiv.org/abs/2007.01282
author: Gautier Izacard, Edouard Grave (Facebook AI)
year: 2021
status: unread

---

## In one sentence

Fusion-in-Decoder (FiD): encode each retrieved passage independently, then fuse all encodings in the decoder — scales retrieval to many passages cheaply.

---

## Key ideas

1. Encoding passages independently allows scaling to 100+ passages without quadratic attention cost
2. The decoder attends over the concatenation of all encoded passages
3. More retrieved passages consistently improves performance — a strong argument for retrieval breadth

---

## Quotes worth keeping

> "Processing passages independently in the encoder, but jointly in the decoder"

---

## My reaction

[Fill after reading]

---

## Permanent notes to write

- [ ] [[]] — Encoding and fusion are separable concerns in RAG architectures

---

## Links to existing notes

- [[Lewis 2020 RAG for Knowledge-Intensive NLP Tasks]]
- [[MOC RAG]]

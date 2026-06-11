# Gao 2023 — DAIL-SQL: Efficient Prompt Engineering for Large Language Models and Text-to-SQL

date: 2026-06-12
tags: #literature #text-to-sql #structured-data
type: paper
source: https://arxiv.org/abs/2308.15363
author: Dawei Gao et al.
year: 2023
status: unread

---

## In one sentence

Systematically studies prompt design for Text-to-SQL: which schema representation, which few-shot examples, and which format maximize accuracy — establishes best practices for production systems.

---

## Key ideas

1. Question similarity + query similarity together are the best criteria for selecting few-shot examples
2. Masked question similarity: mask entity values to focus on query structure, not surface forms
3. Efficient representation: full DDL (CREATE TABLE) as schema format outperforms others
4. Top result on Spider at time of publication — practical, not just theoretical

---

## Why it matters for the compliance audit system

This paper tells you exactly how to format your DB schema in the prompt and how to select examples so the LLM generates correct SQL for regulation-derived queries.

---

## Quotes worth keeping

> "Question similarity alone is insufficient — you also need similar SQL structure in the few-shot examples"

---

## My reaction

[Fill after reading]

---

## Permanent notes to write

- [ ] [[]] — Few-shot example selection strategy for Text-to-SQL
- [ ] [[]] — DDL as the superior schema representation format for LLMs

---

## Links to existing notes

- [[Guo 2023 DIN-SQL Text-to-SQL with Self-Correction]]
- [[MOC Compliance Audit Agent]]

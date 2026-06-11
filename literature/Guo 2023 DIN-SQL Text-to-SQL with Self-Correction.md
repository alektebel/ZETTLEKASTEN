# Guo 2023 — DIN-SQL: Decomposed In-Context Learning of Text-to-SQL with Self-Correction

date: 2026-06-12
tags: #literature #text-to-sql #agents #structured-data
type: paper
source: https://arxiv.org/abs/2304.11015
author: Mohammadreza Pourreza, Davood Rafiei
year: 2023
status: unread

---

## In one sentence

Decomposes Text-to-SQL into sub-problems (schema linking → SQL classification → SQL generation → self-correction), achieving near-human performance on the Spider benchmark.

---

## Key ideas

1. Schema linking: identify which tables/columns in the schema are relevant to the question — critical for large DBs
2. Query classification: is this a simple, nested, or non-nested query? Different prompts for each
3. Self-correction: the model reviews and corrects its own SQL before execution
4. Each step is a separate LLM call — modular and debuggable

---

## Why it matters for the compliance audit system

The audit system needs to translate regulation rules into SQL queries automatically.
Example: "provision_period < 90 days" → `SELECT * FROM loans WHERE provision_period < 90`
Schema linking is essential when the DB has hundreds of tables.

---

## Quotes worth keeping

> "Decomposing the problem into sub-tasks dramatically reduces the complexity of each individual step"

---

## My reaction

[Fill after reading]

---

## Permanent notes to write

- [ ] [[]] — Schema linking as the bottleneck in Text-to-SQL for large databases
- [ ] [[]] — Decomposition as a general strategy for complex LLM tasks

---

## Links to existing notes

- [[Gao 2023 DAIL-SQL SOTA Text-to-SQL]]
- [[MOC Compliance Audit Agent]]

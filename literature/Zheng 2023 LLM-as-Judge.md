# Zheng 2023 — Judging LLM-as-a-Judge with MT-Bench and Chatbot Arena

date: 2026-06-12
tags: #literature #evaluation #llm-as-judge
type: paper
source: https://arxiv.org/abs/2306.05685
author: Lianmin Zheng et al. (UC Berkeley)
year: 2023
status: unread

---

## In one sentence

Formalizes and validates using a strong LLM (GPT-4) as an automated evaluator of other LLMs, showing high agreement with human judgments — and identifies key failure modes.

---

## Key ideas

1. Position bias: the judge favors the first answer presented — mitigate with swapped-order averaging
2. Verbosity bias: longer answers rated higher regardless of quality
3. Reference-guided scoring: providing the correct answer reduces hallucination in the judge
4. GPT-4 as judge achieves >80% agreement with humans on most tasks

---

## Why it matters for the compliance audit system

Your audit system's output ("this record violates regulation X because Y") needs to be evaluated.
LLM-as-judge lets you automate quality checks:
- Is the cited regulation clause actually relevant?
- Is the violation reasoning correct?
- Is the finding actionable?

---

## Quotes worth keeping

> "LLM-as-a-judge is a scalable and explainable alternative to human evaluation for many tasks"

---

## My reaction

[Fill after reading]

---

## Permanent notes to write

- [ ] [[]] — Position and verbosity biases in LLM judges — how to mitigate
- [ ] [[]] — LLM-as-judge enables scalable evaluation of generative audit findings

---

## Links to existing notes

- [[Es 2023 RAGAS Evaluation Framework]]
- [[MOC Compliance Audit Agent]]

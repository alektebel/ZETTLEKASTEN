# Schick 2023 — Toolformer: Language Models Can Teach Themselves to Use Tools

date: 2026-06-12
tags: #literature #agents #tool-use #fine-tuning
type: paper
source: https://arxiv.org/abs/2302.04761
author: Timo Schick et al. (Meta AI)
year: 2023
status: unread

---

## In one sentence

Fine-tunes an LLM to decide when to call which tool (calculator, search, SQL, calendar, etc.) by self-supervised annotation of when tool calls would have helped.

---

## Key ideas

1. Self-supervised: model annotates its own training data by sampling tool calls and keeping the ones that reduce perplexity
2. Tools are invoked inline within generated text — natural integration, not a separate planning step
3. Works for heterogeneous tools simultaneously (different tools for different needs)
4. Contrast with ReAct: Toolformer is fine-tuned; ReAct is prompting-only

---

## Why it matters for the compliance audit system

If you want the audit system to autonomously decide "I need to run a SQL query here" vs. "I need to look up the regulation here" without being told — Toolformer shows how to train that capability.

---

## Quotes worth keeping

> "The model learns to use tools in a self-supervised way, without requiring human demonstrations"

---

## My reaction

[Fill after reading]

---

## Permanent notes to write

- [ ] [[]] — Self-supervised tool use annotation: reducing perplexity as a training signal
- [ ] [[]] — Fine-tuning vs. prompting for tool selection in agents

---

## Links to existing notes

- [[Yao 2022 ReAct Synergizing Reasoning and Acting]]
- [[MOC Compliance Audit Agent]]

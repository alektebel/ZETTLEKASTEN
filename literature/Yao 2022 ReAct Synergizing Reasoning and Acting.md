# Yao 2022 — ReAct: Synergizing Reasoning and Acting in Language Models

date: 2026-06-12
tags: #literature #agents #reasoning #tool-use
type: paper
source: https://arxiv.org/abs/2210.03629
author: Shunyu Yao et al. (Princeton / Google)
year: 2022
status: unread

---

## In one sentence

Interleaves chain-of-thought reasoning (Think) with tool calls (Act) so the model can plan, query external systems, observe results, and loop — the foundation of most agent frameworks.

---

## Key ideas

1. Thought → Action → Observation loop: the model reasons, calls a tool, reads the output, reasons again
2. Grounded reasoning: observations from tools prevent hallucination by anchoring the chain of thought
3. Works with any tool (search, SQL, calculator, API) — the interface is just text in/out
4. Directly applicable: database query + regulation lookup both map cleanly to ReAct tools

---

## Why it matters for the compliance audit system

An audit agent needs to:
- Think: "This column is provision_period — I need to check if it's < 3 months"
- Act: query the DB (SQL tool)
- Observe: get the records
- Think: "Now retrieve the relevant regulation clause"
- Act: vector search over regulation corpus
- Observe: regulation text
- Think: "Record X violates clause Y because..."

ReAct is the skeleton of that loop.

---

## Quotes worth keeping

> "ReAct prompts LLMs to generate both verbal reasoning traces and actions pertaining to a task in an interleaved manner"

---

## My reaction

[Fill after reading]

---

## Permanent notes to write

- [ ] [[]] — The Think-Act-Observe loop as the universal agent pattern
- [ ] [[]] — Tool calls as grounding mechanisms against hallucination

---

## Links to existing notes

- [[MOC Compliance Audit Agent]]
- [[MOC RAG]]

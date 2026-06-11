# MOC: Compliance Audit Agent (DB + Regulation RAG)

date: 2026-06-12
tags: #index #moc #agents #compliance #rag #structured-data
topic: Building an agent that audits database records against regulatory text

---

## What this map covers

How to build a system that takes a relational database and a corpus of regulations, and autonomously finds audit findings (e.g. "provision period < 3 months") by combining vector search, Text-to-SQL, and LLM reasoning.

---

## System architecture (how the pieces connect)

```
REGULATIONS (text)                    DATABASE (structured)
      │                                       │
 chunk + embed                        embed schema + cells
      │                                       │
REGULATION VECTOR DB              TABLE VECTOR INDEX (TableRAG)
      │                                       │
      └──────────────┬────────────────────────┘
                     │
              AUDIT AGENT (ReAct loop)
                     │
        ┌────────────┼─────────────────┐
        │            │                 │
   Think step    SQL tool         Regulation
  (reasoning)  (Text-to-SQL)     retrieval tool
                     │                 │
              DB records          Relevant clause
                     │                 │
                     └────────┬────────┘
                          LLM judge
                      (is this a finding?)
                              │
                       AUDIT REPORT
```

---

## Reading order

### 1. Agent backbone
- [[Yao 2022 ReAct Synergizing Reasoning and Acting]] — the Think-Act-Observe loop your agent runs on
- [[Schick 2023 Toolformer Language Models Teach Themselves Tool Use]] — how to make the agent decide which tool to call

### 2. Structured data + SQL
- [[Guo 2023 DIN-SQL Text-to-SQL with Self-Correction]] — translate regulation rules to SQL queries
- [[Gao 2023 DAIL-SQL SOTA Text-to-SQL]] — best practices: schema format, few-shot selection

### 3. RAG over tabular data
- [[Chen 2024 TableRAG Million-Token Table Understanding]] — vector index of schema + cell values; the bridge between DB and LLM context

### 4. Regulation retrieval (RAG)
- Start from [[MOC RAG]] — especially Self-RAG and CRAG for adaptive retrieval
- [[Asai 2023 Self-RAG]] — let the agent decide when to retrieve a regulation clause
- [[Yan 2024 CRAG Corrective Retrieval]] — fallback when regulation retrieval confidence is low

### 5. Evaluation
- [[Es 2023 RAGAS Evaluation Framework]] — evaluate retrieval quality of regulation chunks
- [[Zheng 2023 LLM-as-Judge]] — evaluate quality of audit findings automatically

---

## Key design decisions to make

| Decision | Options | Key tradeoff |
|---|---|---|
| How to represent regulations | Chunked text vs. structured rules | Free text is flexible; structured rules are auditable |
| How to query the DB | Text-to-SQL vs. predefined SQL templates | LLM-generated SQL is flexible but risky |
| When to retrieve regulations | Always vs. adaptively (Self-RAG) | Always is simpler; adaptive saves cost |
| How to loop over records | Row-by-row vs. SQL filter first | SQL filter is far more scalable |
| How to evaluate findings | Human review vs. LLM-as-judge | LLM judge scales; human review is ground truth |

---

## Open questions

- How do you handle regulation ambiguity? ("reasonable period" — what's reasonable?)
- How do you avoid false positives at scale (100k records)?
- How do you keep the regulation index fresh when rules change?
- Can you generate the SQL filter directly from the regulation text (regulation → SQL → filter → report)?

---

## Connected MOCs

- [[MOC RAG]]

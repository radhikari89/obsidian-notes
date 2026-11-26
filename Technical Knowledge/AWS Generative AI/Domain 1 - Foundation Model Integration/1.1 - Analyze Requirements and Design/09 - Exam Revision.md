---
tags: [aws, aip-c01, domain-1, task-1-1]
status: to-review
---

# Exam Revision
## Decision cues
| Scenario | Likely approach |
|---|---|
| Validate uncertain business value | Scoped PoC with measurable baseline |
| Answer from changing private documents | RAG with access controls |
| Compare candidate models | Representative evaluation dataset |
| Consistent deployment across teams | Versioned IaC and shared adapters |
| Architecture risk review | Well-Architected Tool and GenAI Lens |
| Throttling | Bounded backoff, quota review and load management |
| Poor answer despite good retrieval | Inspect prompt and generation behavior |

## Active recall
- What requirements should precede model selection? :: Quality, latency, cost, modality, security and operational constraints.
- How does RAG differ from fine-tuning? :: RAG adds retrieved context; tuning changes parameters.
- What is a PoC success criterion? :: A measurable threshold agreed before testing.
- Why use p95 latency? :: It exposes slow-tail behavior hidden by averages.
- Does a guardrail replace IAM? :: No.
- What makes components reusable? :: Stable interfaces, versioning, testing and documentation.
- What are the six Well-Architected pillars? :: Operational excellence, security, reliability, performance efficiency, cost optimization and sustainability.

## Revision checklist
- [ ] Explain architecture choices without looking at notes.
- [ ] Design a PoC and calculate potential ROI.
- [ ] Explain production failure modes and mitigations.
- [ ] Complete the practical exercise.
- [ ] Compare these notes against actual Skill Builder lessons and fill gaps.

Back: [[00 - Course Overview]]

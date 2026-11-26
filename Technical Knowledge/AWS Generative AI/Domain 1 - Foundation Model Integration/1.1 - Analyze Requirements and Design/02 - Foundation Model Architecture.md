---
tags: [aws, aip-c01, domain-1, task-1-1]
status: to-review
---

# Foundation Model Architecture
## Requirements first
Identify users, task, modalities, accuracy, latency, throughput, budget, data residency, privacy and acceptable failure modes. Define measurable acceptance criteria before selecting technology.

| Requirement | Design choice |
|---|---|
| Current private information | RAG with authorized documents |
| Consistent task behavior | Prompt examples; consider tuning if insufficient |
| Multi-step deterministic workflow | Step Functions or application orchestration |
| Image and text input | Compatible multimodal model |
| Simple classification | Consider a small model or conventional ML |

## Integration approaches
- Managed model APIs: reduce infrastructure responsibilities (Bedrock).
- Hosted/custom models: greater infrastructure or model control (SageMaker AI), with additional operational responsibility.
- Model chaining: pass validated output from one stage to the next; track cumulative latency, cost and errors.
- Routing: select a model according to task complexity, security constraints and evaluated quality.

RAG retrieves external information at inference time; fine-tuning changes model parameters and is not a reliable substitute for fresh factual retrieval.

> [!tip] Exam
> Choose the simplest pattern satisfying all constraints, rather than automatically choosing the largest model.

Related: [[03 - Amazon Bedrock Integration]] · [[04 - Proof of Concept]]

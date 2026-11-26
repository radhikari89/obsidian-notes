---
tags: [aws, aip-c01, domain-1, task-1-1]
status: to-review
---

# Production Readiness
A successful demo is not evidence that an application is safe, reliable or scalable in production.

## Controls
- Reliability: timeouts, bounded retries with exponential backoff and jitter for transient failures, circuit breakers and safe fallback.
- Security: IAM isolation, encryption, document-level authorization, input/output validation.
- Observability: CloudWatch metrics and alarms, correlated application traces, privacy-aware logs.
- Deployment: version prompts, model configuration and retrieval settings; use CI/CD and rollback mechanisms.
- Quality: regression evaluations, adversarial tests, human feedback, periodic review.
- Cost: token budgets, model routing, safe caching and usage monitoring.

## RAG failure diagnosis
| Symptom | Investigation |
|---|---|
| Relevant document absent | Ingestion, parsing, chunking, metadata filters or retrieval |
| Retrieved context correct but answer wrong | Prompt, model, context ordering or generation settings |
| Old answer | Source freshness and index synchronization |
| Unauthorized answer | Access filters and identity propagation |

## Rollout
Offline evaluation → staging → limited pilot → measured rollout → ongoing monitoring. Use fallback only if the alternative meets safety and data-residency rules.

Related: [[06 - Well-Architected Framework]] · [[07 - Standardized Components]]

---
tags: [aws, aip-c01, domain-1, task-1-1]
status: to-review
---

# Amazon Bedrock Integration
Amazon Bedrock provides managed access to supported foundation models and capabilities for building GenAI applications.

| Feature | Purpose |
|---|---|
| Converse / ConverseStream | Common conversational interface across supported models |
| InvokeModel / InvokeModelWithResponseStream | Native model-specific invocation |
| Knowledge Bases | Managed retrieval and grounding workflows |
| Guardrails | Configurable content and safety controls |
| Model evaluation | Compare model behavior on representative tasks |

## Prompt design
Specify task, context, constraints, examples and output format. Validate structured responses against an application schema. Treat retrieved content as untrusted data, not instructions.

## Security and integration
Use IAM workload roles and least privilege; avoid hardcoded keys. Verify model/feature availability in the intended Region. Use private connectivity where required. Review logging and retention settings for sensitive inputs.

## Performance
Measure first-token latency for streaming, end-to-end latency, token usage and error rates. Streaming improves perceived responsiveness but does not necessarily reduce total compute time.

> [!warning] Guardrails are not authorization
> Enforce access control independently in the application and retrieval layers.

Related: [[05 - Production Readiness]]

---
tags: [aws, aip-c01, domain-1, task-1-1]
status: to-review
---

# Standardized Components
Build reusable, versioned modules rather than duplicating model integration logic across applications.

| Component | Responsibility |
|---|---|
| Model adapter | Normalize invocation, errors and telemetry |
| Prompt registry | Version prompts and configuration |
| Retrieval adapter | Retrieve authorized context |
| Policy layer | Apply access controls and safety checks |
| Evaluation harness | Run regression datasets and quality gates |
| IaC module | Repeatable IAM, networking and deployment |

## Governance and testing
Define interfaces, ownership, approved configurations, changelogs and exception processes. Test unit behavior with mocks, integration with actual APIs and end-to-end response quality with representative data. Publish templates via CI/CD.

## Multi-Region considerations
Check model availability, quotas, data residency, failover behavior and consistency of indexes and configuration. Cross-Region inference may distribute requests across supported Regions; check permitted destinations before enabling it.

Related: [[05 - Production Readiness]] · [[08 - Practical Implementation]]

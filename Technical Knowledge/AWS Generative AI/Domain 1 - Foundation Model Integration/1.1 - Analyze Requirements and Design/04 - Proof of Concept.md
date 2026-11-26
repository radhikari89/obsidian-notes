---
tags: [aws, aip-c01, domain-1, task-1-1]
status: to-review
---

# Proof of Concept (PoC)
A PoC is a limited experiment that tests whether a proposed solution can satisfy measurable requirements before a full rollout.

## Process
1. Choose a narrowly scoped business problem and baseline.
2. Build a representative evaluation dataset with expected answers and failure cases.
3. Compare candidate models and prompts under equivalent conditions.
4. Measure quality, latency, throughput, cost and safety.
5. Document tradeoffs, unresolved risks and go/no-go criteria.

## Example acceptance criteria (illustrative)
- At least 90% correct answers on a curated test set.
- p95 end-to-end latency under 5 seconds.
- No unauthorized document disclosure in access-control tests.
- Human review for high-impact decisions.

## Business value
Monthly net benefit = realized time savings + other measurable benefit − monthly operating cost.
ROI (%) = (benefits − costs) / costs × 100 (use the same period for both).
Example: 1,000 tasks/month × 5 minutes saved × $60/hour = $5,000 potential monthly labor value. If operating cost is $1,000, net potential value is $4,000 before other costs. Time saved is not necessarily cash saved.

> [!question] Recall
> Why not use only model benchmark scores? They may not represent your own data, workload or quality requirements.

Related: [[02 - Foundation Model Architecture]] · [[05 - Production Readiness]]

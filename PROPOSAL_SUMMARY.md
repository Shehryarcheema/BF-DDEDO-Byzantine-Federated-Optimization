# PhD Research Proposal Summary

## Quick Facts

- **Title**: A Byzantine-Robust Federated Data-Driven Evolutionary Dynamic Optimization Framework for Secure Financial Edge Networks
- **Field**: Machine Learning, Evolutionary Computation, Federated Learning, Financial AI
- **Duration**: 3 years (36 months)
- **Key Innovation**: Novel drift-aware Byzantine-robust aggregation operator

## The Research Gap

Three mature research areas exist independently:
1. ✅ Byzantine-robust federated learning
2. ✅ Evolutionary dynamic optimisation
3. ✅ Surrogate-assisted evolutionary optimisation

**But no framework addresses all three together, especially under concept drift where legitimate environmental changes are indistinguishable from adversarial poisoning.**

## What Makes This Novel

### Problem
When a financial market shifts, all edge nodes' models change abruptly. Standard Byzantine aggregators (Krum, trimmed-mean) treat this abrupt change as suspicious poisoning and reject good updates.

### Solution
A **drift-aware aggregation operator** that:
- Maintains a global drift-trajectory reference
- Compares each node's update against expected drift
- Distinguishes legitimate evolution from Byzantine attacks
- Tolerates bounded malicious fraction f

## Regulatory Relevance

Directly addresses the **FCA–BoE Joint Discussion Paper (DP5/22)** which calls for:
- Byzantine robustness in financial AI
- Explainability in autonomous decision-making
- Regulatory compliance frameworks

## Expected Outputs

### Academic
- 1 survey paper (WP1)
- 1 conference paper (WP3)
- 2+ journal papers (WP4, WP5)
- 1 PhD thesis

### Practical
- Open-source benchmark suite
- Reference implementation of BF-DDEDO framework
- Deployment guidance for financial institutions
- Practitioner insights from 30+ domain experts

## Risk Management

| Risk | Mitigation |
|------|------------|
| Theoretical intractability of tolerance proof | Empirical guarantees with comprehensive stress-testing |
| Computational cost of large experiments | DMU HPC cluster access + staged scaling |
| Low survey/interview response | Early fintech community engagement |
| Third-party library restrictions | Open-source simulation fallbacks |

## Why This Matters

### For Industry
Edge-based financial systems (fraud detection, portfolio rebalancing, risk management) can operate robustly even with compromised nodes.

### For Regulators
Evidence-based technical standards for trustworthy AI in regulated financial infrastructure.

### For Researchers
A new problem class and novel technique applicable to any federated evolutionary system under drift (beyond finance).

## Timeline Snapshot

- **Months 1–6**: Literature & gap analysis
- **Months 5–12**: Benchmark suite & problem formalisation
- **Months 11–19**: Federated architecture prototype
- **Months 18–27**: Novel drift-aware aggregator development
- **Months 25–33**: Benchmarking, practitioner studies, validation
- **Months 31–36**: Thesis writing, open dissemination

---

**For full details, see `P2952028__SHEHRYAR.pdf`**

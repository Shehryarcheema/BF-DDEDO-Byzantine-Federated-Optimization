# BF-DDEDO: A Byzantine-Robust Federated Data-Driven Evolutionary Dynamic Optimization Framework for Secure Financial Edge Networks

**Author:** Shehryar (P2952028), MSc Artificial Intelligence  
**Institution:** De Montfort University, Leicester  
**Proposal date:** June 2nd, 2026

## Project Overview

This repository documents a PhD research proposal for a three-year doctoral
project to design, implement, and rigorously evaluate a **Byzantine-robust
federated framework for data-driven evolutionary dynamic optimization
(BF-DDEDO)** in secure financial edge networks.

## Problem Statement

Financial services are rapidly migrating computation to the network edge, where
decisions must be optimised under continuously shifting market conditions.
This research addresses three critical, unsolved problems:

1. **Dynamic Optimization** — fitness landscapes change over time; algorithms
   must track a moving optimum.
2. **Data-Driven Surrogate Assistance** — evaluating candidate solutions on live
   financial infrastructure is prohibitively expensive, so optimisation must
   rely on surrogate models.
3. **Federated Byzantine Robustness** — edge nodes are geographically
   distributed and untrusted, yet federated systems are vulnerable to Byzantine
   participants that can poison shared surrogate models.

**No existing framework unifies these three requirements.**

## The Research Gap

Three mature research areas exist independently — Byzantine-robust federated
learning, evolutionary dynamic optimisation, and surrogate-assisted
evolutionary optimisation — but no framework addresses all three together,
especially under **concept drift**, where legitimate environmental change is
indistinguishable from adversarial poisoning.

That distinction is the crux of the problem: when a financial market shifts,
all edge nodes' models change abruptly, and standard Byzantine aggregators
(Krum, trimmed-mean) can mistake this abrupt legitimate change for poisoning
and reject good updates.

## Key Innovation

A **drift-aware Byzantine-robust aggregation operator** that:

- Maintains a global drift-trajectory reference,
- Compares each node's update against the expected drift,
- Distinguishes legitimate environmental evolution from Byzantine attacks,
- Tolerates a bounded malicious fraction *f*.

## Research Aims

To design, implement, and rigorously evaluate a Byzantine-robust federated
framework for data-driven evolutionary dynamic optimisation that enables secure
and adaptive optimisation in distributed financial edge environments subject to
concept drift and adversarial participants.

## Key Objectives

1. **Literature Review** — systematic review across EDO, surrogate-assisted
   optimisation, federated learning, and Byzantine-robust aggregation.
2. **Benchmark Suite** — combine the Moving Peaks Benchmark and GDBG with a
   parameterised financial-edge simulation.
3. **Federated Architecture** — design local surrogate models with a secure
   aggregation protocol.
4. **Novel Operator** — develop the drift-aware Byzantine-robust aggregation
   operator.
5. **Evaluation** — empirical evaluation against baselines with statistical
   rigour.
6. **Practitioner Validation** — questionnaire and interview studies with
   domain experts.

## Research Methodology

### Computational Strand

- **Formalisation** of federated data-driven DOP and adversary models.
- **Algorithm Design** producing the drift-aware robust aggregator.
- **Benchmarking** on Moving Peaks and GDBG.
- **Statistical Validation** using ≥30 independent runs, Wilcoxon tests, and
  effect sizes.

### Qualitative Strand

- **Questionnaires** (n ≥ 30 practitioners).
- **Semi-structured Interviews** (n = 10–15 domain experts).
- **Thematic Analysis** using Braun and Clarke's reflexive method.

## Work Packages Timeline

| WP     | Phase | Duration   | Deliverables |
|--------|-------|------------|--------------|
| **WP1** | Literature Review & Gap Formalisation | Months 1–6  | Survey manuscript, Gap report |
| **WP2** | Problem Formulation & Benchmark Suite | Months 5–12 | Open benchmark suite, Technical report |
| **WP3** | Federated Data-Driven EDO Architecture | Months 11–19 | Working prototype, Conference paper |
| **WP4** | Byzantine-Robust Aggregation Operator | Months 18–27 | Novel operator, Journal paper |
| **WP5** | Experimental Evaluation & Practitioner Validation | Months 25–33 | Evaluation dataset, Validated guidance framework |
| **WP6** | Ethics/Legal Analysis, Thesis & Dissemination | Months 31–36 | PhD thesis, ≥2 journal papers |

## Expected Outputs

**Academic:** 1 survey paper (WP1), 1 conference paper (WP3), 2+ journal papers
(WP4, WP5), 1 PhD thesis.  
**Practical:** open-source benchmark suite, reference implementation of the
BF-DDEDO framework, deployment guidance for financial institutions, and
practitioner insights from 30+ domain experts.

## Risk Management

| Risk | Mitigation |
|------|------------|
| Theoretical intractability of the tolerance proof | Empirical guarantees with comprehensive stress-testing |
| Computational cost of large experiments | DMU HPC cluster access + staged scaling |
| Low survey/interview response | Early fintech community engagement |
| Third-party library restrictions | Open-source simulation fallbacks |

## Relevance and Impact

### For Financial Institutions

- Method to optimise under changing conditions while maintaining robustness
  against compromised nodes.
- Reduces operational and systemic risk (fraud detection, portfolio
  rebalancing, risk management can operate robustly even with compromised
  nodes).

### For Regulators

- Evidence-based technical foundations (addressing the FCA–BoE joint
  discussion paper DP5/22) for AI robustness requirements in financial
  systems.

### For Scientific Communities

- **Evolutionary Computation**: a new federated data-driven DOP problem class.
- **Trustworthy AI**: a drift-aware Byzantine-robust technique with analysed
  guarantees, applicable to any federated evolutionary system under drift
  (beyond finance).
- **Practitioners**: a validated deployment framework grounded in real-world
  requirements.

### For Society

- More resilient financial infrastructure.
- Safer autonomous optimisation in regulated systems.

## Regulatory Compliance

The research addresses key regulatory requirements:

- **Financial Conduct Authority (FCA)**: Senior Managers Regime for algorithmic
  accountability.
- **Bank of England**: AI robustness and explainability requirements.
- **UK GDPR & Data Protection Act 2018**: federated design avoids centralising
  regulated data.
- **EU AI Act 2024**: applicable provisions for autonomous financial systems.

## Technical Highlights

### Surrogate Models

- Gaussian Processes (GP)
- Radial Basis Function (RBF) networks
- Neural networks (NN)

### Robust Aggregation

- Baselines: Krum, coordinate-wise median / trimmed-mean.
- Novel: drift-aware aggregator distinguishing legitimate environmental drift
  from adversarial poisoning.

### Tools & Technologies

- **Python ecosystem**: NumPy, scikit-learn, PyTorch, DEAP.
- **Federated learning**: Flower framework.
- **Version control**: Git.
- **Statistical analysis**: Wilcoxon rank-sum, Friedman post-hoc, effect
  sizes.

## Ethical and Legal Considerations

- **Data Protection**: federated design, anonymised data, GDPR compliance.
- **Security**: Byzantine attacks confined to simulation, responsible
  disclosure.
- **Reproducibility**: open code, fixed random seeds, documented benchmarks.
- **Professional Standards**: ACM & BCS codes of conduct.

## Repository Contents

- `README.md` — this file.
- `PROPOSAL_SUMMARY.md` — condensed summary of the proposal (quick facts,
  novelty, regulatory relevance, outputs, risks, timeline).
- `LICENSE` — MIT License.

The full six-page proposal PDF referenced in the summary is not hosted in this
repository; request it from the candidate or the supervisory team.

## Getting Started

To explore this research:

1. **Read the summary**: see `PROPOSAL_SUMMARY.md` for the quick facts, gap,
   novelty, and timeline snapshot.
2. **Review the methods**: the "Research Methodology" section above outlines
   the computational and qualitative research design.
3. **Understand the timeline**: the Work Packages table above (Months 1–36).
4. **Explore the impact**: the "Relevance and Impact" section above discusses
   beneficiaries.

## Contact & Supervision

- **Candidate**: Shehryar (MSc AI, De Montfort University)
- **Primary Supervisor**: Evolutionary Dynamic Optimisation specialist
- **Co-Supervisor**: Distributed/Secure Systems specialist
- **Institution**: De Montfort University, Leicester, UK

## Research Status

- **Phase**: Research proposal development (2026)
- **Expected PhD Duration**: 3 years (Months 1–36)
- **Funding**: Supported by DMU research infrastructure and HPC cluster access

## Keywords

`Byzantine-Robustness` · `Federated-Learning` · `Evolutionary-Algorithms` ·
`Dynamic-Optimization` · `Surrogate-Models` · `Financial-AI` ·
`Edge-Computing` · `Concept-Drift` · `Secure-Computation` ·
`Robust-Aggregation`

---

**For inquiries or feedback:** Contact the supervisory team at De Montfort
University.  
**License:** MIT License — see [LICENSE](LICENSE) for details.

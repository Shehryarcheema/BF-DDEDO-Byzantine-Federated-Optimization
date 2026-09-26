# Byzantine-Robust Federated Data-Driven Evolutionary Dynamic Optimization Framework for Secure Financial Edge Networks

**Author:** Shehryar  
**Student ID:** P2952028  
**Programme:** MSc Artificial Intelligence  
**Institution:** De Montfort University, Leicester  
**Submission Date:** June 2nd, 2026

## Project Overview

This repository contains the PhD research proposal for a three-year doctoral project focused on designing, implementing, and evaluating a **Byzantine-robust federated framework for data-driven evolutionary dynamic optimization (BF-DDEDO)** in secure financial edge networks.

## Problem Statement

Financial services are rapidly migrating computation to the network edge—where decisions must be optimised under continuously shifting market conditions. This research addresses three critical unsolved problems:

1. **Dynamic Optimization**: Fitness landscapes change over time; algorithms must track a moving optimum
2. **Data-Driven Surrogate Assistance**: Evaluating candidate solutions on live financial infrastructure is prohibitively expensive
3. **Federated Byzantine Robustness**: Edge nodes are geographically distributed and untrusted, yet federated systems are vulnerable to Byzantine participants that can poison shared surrogate models

**No existing framework unifies these three requirements.**

## Research Aims

To design, implement, and rigorously evaluate a Byzantine-robust federated framework for data-driven evolutionary dynamic optimisation that enables secure and adaptive optimisation in distributed financial edge environments subject to concept drift and adversarial participants.

## Key Objectives

1. **Literature Review**: Systematic review across EDO, surrogate-assisted optimisation, federated learning, and Byzantine-robust aggregation
2. **Benchmark Suite**: Combine Moving Peaks Benchmark and GDBG with parameterised financial-edge simulation
3. **Federated Architecture**: Design local surrogate models with secure aggregation protocol
4. **Novel Operator**: Develop drift-aware Byzantine-robust aggregation operator
5. **Evaluation**: Empirical evaluation against baselines with statistical rigour
6. **Practitioner Validation**: Questionnaire and interview studies with domain experts

## Research Methodology

### Computational Strand
- **Formalisation** of federated data-driven DOP and adversary models
- **Algorithm Design** producing drift-aware robust aggregator
- **Benchmarking** on Moving Peaks and GDBG
- **Statistical Validation** using ≥30 independent runs, Wilcoxon tests, and effect sizes

### Qualitative Strand
- **Questionnaires** (n ≥ 30 practitioners)
- **Semi-structured Interviews** (n = 10–15 domain experts)
- **Thematic Analysis** using Braun and Clarke's reflexive method

## Work Packages Timeline

| WP | Phase | Duration | Deliverables |
|----|-------|----------|---------------|
| **WP1** | Literature Review & Gap Formalisation | Months 1–6 | Survey manuscript, Gap report |
| **WP2** | Problem Formulation & Benchmark Suite | Months 5–12 | Open benchmark suite, Technical report |
| **WP3** | Federated Data-Driven EDO Architecture | Months 11–19 | Working prototype, Conference paper |
| **WP4** | Byzantine-Robust Aggregation Operator | Months 18–27 | Novel operator, Journal paper |
| **WP5** | Experimental Evaluation & Practitioner Validation | Months 25–33 | Evaluation dataset, Validated guidance framework |
| **WP6** | Ethics/Legal Analysis, Thesis & Dissemination | Months 31–36 | PhD thesis, ≥2 journal papers |

## Relevance and Impact

### For Financial Institutions
- Method to optimise under changing conditions while maintaining robustness against compromised nodes
- Reduces operational and systemic risk

### For Regulators
- Evidence-based technical foundations (addressing FCA–BoE joint discussion paper DP5/22)
- Guidance for AI robustness requirements in financial systems

### For Scientific Communities
- **Evolutionary Computation**: New federated data-driven DOP problem class
- **Trustworthy AI**: Drift-aware Byzantine-robust technique with analysed guarantees
- **Practitioners**: Validated deployment framework grounded in real-world requirements

### For Society
- More resilient financial infrastructure
- Safer autonomous optimisation in regulated systems

## Regulatory Compliance

The research addresses key regulatory requirements:
- **Financial Conduct Authority (FCA)**: Senior Managers Regime for algorithmic accountability
- **Bank of England**: AI robustness and explainability requirements
- **UK GDPR & Data Protection Act 2018**: Federated design avoids centralising regulated data
- **EU AI Act 2024**: Applicable provisions for autonomous financial systems

## Technical Highlights

### Surrogate Models
- Gaussian Processes (GP)
- Radial Basis Function (RBF) Networks
- Neural Networks (NN)

### Robust Aggregation
- Baseline: Krum, coordinate-wise median/trimmed-mean
- Novel: Drift-aware aggregator distinguishing legitimate environmental drift from adversarial poisoning

### Tools & Technologies
- **Python Ecosystem**: NumPy, scikit-learn, PyTorch, DEAP
- **Federated Learning**: Flower framework
- **Version Control**: Git
- **Statistical Analysis**: Wilcoxon rank-sum, Friedman post-hoc, effect sizes

## Ethical and Legal Considerations

✅ **Data Protection**: Federated design, anonymised data, GDPR compliance  
✅ **Security**: Byzantine attacks confined to simulation, responsible disclosure  
✅ **Reproducibility**: Open code, fixed random seeds, documented benchmarks  
✅ **Professional Standards**: ACM & BCS codes of conduct  

## Files in This Repository

- `README.md` - This file
- `P2952028__SHEHRYAR.pdf` - Full PhD research proposal (6 pages + Gantt chart)
- `LICENSE` - MIT License

## Getting Started

To explore this research:

1. **Read the Proposal**: See `P2952028__SHEHRYAR.pdf` for the complete proposal
2. **Review Methods**: Section 5 outlines the computational and qualitative research design
3. **Understand Timeline**: Work Package structure in Section 6 with associated Gantt chart
4. **Explore Impact**: Section 8 discusses relevance to beneficiaries

## Contact & Supervision

- **Candidate**: Shehryar (MSc AI, De Montfort University)
- **Primary Supervisor**: Evolutionary Dynamic Optimisation specialist
- **Co-Supervisor**: Distributed/Secure Systems specialist
- **Institution**: De Montfort University, Leicester, UK

## Research Status

📋 **Phase**: Research proposal development (2026)  
📅 **Expected PhD Duration**: 3 years (Months 1–36)  
🎯 **Funding**: Supported by DMU research infrastructure and HPC cluster access  

## Keywords

`Byzantine-Robustness` · `Federated-Learning` · `Evolutionary-Algorithms` · `Dynamic-Optimization` · `Surrogate-Models` · `Financial-AI` · `Edge-Computing` · `Concept-Drift` · `Secure-Computation` · `Robust-Aggregation`

---

**For inquiries or feedback:** Contact supervisory team at De Montfort University  
**Licence:** MIT License (see LICENSE file)

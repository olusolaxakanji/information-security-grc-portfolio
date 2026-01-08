# Business Continuity & Disaster Recovery

**Emyzer Technology – ServiceNow GRC Project**

---

## Overview

This folder contains Emyzer Technology's Business Continuity Management System (BCMS) documentation, developed in ServiceNow GRC and aligned with ISO 22301:2019, ISO/IEC 27031:2011, BCI Good Practice Guidelines, and NIST SP 800-34 Rev. 1.

The documentation demonstrates the complete BC/DR lifecycle: governance, analysis, validation, and framework alignment.

---

## Documents

| Document | Purpose | Framework Alignment |
|----------|---------|---------------------|
| [Business Continuity and Disaster Recovery Policy](business-continuity-disaster-recovery-policy.md) | Establishes governance, roles, and procedures for BC/DR program | ISO 22301 Clauses 4–10, BCI PP1, NIST 3.1 |
| [Business Impact Analysis](business-impact-analysis-example.md) | Identifies critical functions, dependencies, and recovery targets (RTO/RPO) | ISO 22301 Clause 8.2.2, BCI PP3, NIST 3.2 |
| [Tabletop Exercise Summary](bcdr-tabletop-exercise-summary.md) | Validates BC/DR procedures through ransomware response scenario | ISO 22301 Clause 8.5, BCI PP6, NIST 3.5 |
| [Framework Alignment Matrix](framework-alignment-matrix.md) | Maps documentation to ISO 22301, ISO 27031, BCI GPG, and NIST 800-34 | Audit and compliance readiness |

---

## BC/DR Lifecycle Coverage

```
┌─────────────────────────────────────────────────────────────────┐
│                        BC/DR LIFECYCLE                          │
├─────────────┬─────────────┬─────────────┬─────────────┬────────┤
│  GOVERNANCE │  ANALYSIS   │   DESIGN    │ VALIDATION  │ AUDIT  │
│             │             │             │             │        │
│   Policy    │    BIA      │   Policy    │  Tabletop   │ Matrix │
│             │             │  (Procedures)│  Exercise   │        │
└─────────────┴─────────────┴─────────────┴─────────────┴────────┘
```

---

## Key Metrics

| Metric | Value |
|--------|-------|
| **Critical Functions Analyzed** | 5 |
| **RTO Range** | 4–24 hours |
| **RPO Range** | 1–24 hours |
| **Exercise Findings** | 7 |
| **Improvement Actions** | 7 |
| **Frameworks Aligned** | 4 |

---

## Skills Demonstrated

- Business Impact Analysis methodology
- RTO/RPO determination and dependency mapping
- BC/DR policy development aligned to ISO 22301
- Tabletop exercise design and facilitation
- Gap analysis and corrective action planning
- Multi-framework compliance mapping

---

## Tools Used

- **ServiceNow GRC** – Policy management, workflow, and documentation
- **Markdown** – Portfolio formatting and version control

---

## Related Documentation

- [Risk Management Policy](../risk-management/) (parent policy)
- [Information Security Policy](../governance/)
- [Incident Management Policy](../incident-management/)
- [Access Control Policy](../access-control/)

---

*This documentation was developed as part of a ServiceNow GRC implementation project for Emyzer Technology (case study).*

# Veridian AI: Acquired Entity Documentation

**Emyzer Nexus: M&A Integration Programme | Fictional case study.**

> All entities, systems, personnel, and risk findings are invented for professional demonstration purposes. Framework references are accurate as of the document dates.

---

## What This Directory Represents

Veridian AI was an AI-native startup acquired by Emyzer Technology in Q4 2024. At acquisition close, Veridian had two operational AI systems and no formal GRC programme.

This directory contains the two documents produced specifically for Veridian AI as part of post-acquisition governance integration: the due diligence risk assessment conducted on the inherited AI systems, and the AI vendor due diligence addendum created to govern Veridian's inherited vendor relationships and future AI vendor procurement.

For the ongoing AI governance programme governing PCM-001 and CRT-001, see [ai-governance/](../ai-governance/readme.md). For the broader M&A integration programme, see [integration-management/](../integration-management/readme.md).

---

## What Was Found at Acquisition

The due diligence risk assessment of Veridian's two systems produced 8 risk findings, including 4 rated Critical:

| System ID | System | Governance Maturity at Acquisition | Critical Findings |
|---|---|---|---|
| PCM-001 | Predictive Customer Churn Model | Level 1: Ad hoc. No documented validation, monitoring cadence, or bias testing on record. | Training data bias, model drift not monitored, no explainability documentation |
| CRT-001 | AI-Assisted Contract Review Tool | Partial documentation. LLM API data processor relationship not governed under GDPR. | GDPR Article 28 position unresolved, no DPA executed with LLM vendor, contract review outputs not subject to human oversight requirements |

CRT-001 use was restricted to contracts containing no personal data immediately on legal advice. That restriction remained in place until a Data Processing Agreement was executed with the LLM API vendor.

These findings are what triggered the Phase 2 AI governance programme. Without this assessment, the compliance gaps would have remained unquantified and unowned after the acquisition closed.

---

## Documents

### [Veridian AI Risk Assessment](ai-risk-assessments/veridian-ai-risk-assessment.md)

Veridian's systems were in production when acquired. This assessment established what governance obligations existed, what was missing, and what remediation was required before normal operation could continue.

The assessment applies the Phase 1 Emyzer Technology risk methodology, extended with AI-specific risk categories: model drift, training data bias, explainability gaps, and third-party model dependency. Using the Phase 1 methodology rather than a separate framework keeps AI risk findings comparable to the rest of the enterprise risk register.

**Contents:** System inventory, 8 risk findings (4 Critical), gap analysis against EU AI Act standards, EU AI Act risk tier classification recommendation, remediation plan with owners and target dates.

**Frameworks:** NIST AI RMF 1.0, ISO 31000:2018, NIST SP 800-30, EU AI Act

### [AI Vendor Risk Due Diligence Addendum](vendor-risk-addendum/ai-vendor-risk-addendum.md)

Standard TPRM controls were not designed to evaluate AI vendors. Veridian's most significant inherited vendor relationship, the LLM API provider for CRT-001, required assessment criteria that the Phase 1 Third-Party Risk Management Policy did not cover: model transparency, training data provenance, bias audit availability, EU AI Act compliance status, and contractual liability for model errors.

This addendum extends the Phase 1 TPRM Policy for AI vendors rather than creating a parallel vendor risk framework. Design decisions include:

- The addendum is a subordinate document rather than a policy amendment, so it can be updated independently as EU AI Act implementing acts develop without triggering a full policy revision cycle.
- Contractual requirements include the right to audit model documentation and the right to terminate if the vendor fails to maintain EU AI Act compliance, provisions tested against the CRT-001 vendor relationship.
- LLM API vendors are subject to enhanced due diligence covering API output variability, model versioning disclosure, and incident notification SLAs, requirements not present in standard vendor assessment frameworks.

**Frameworks:** ISO 27001:2022 A.5.19-A.5.23, NIST AI RMF, EU AI Act, GDPR

---

## Related Documentation

| Document | Description |
|---|---|
| [AI Governance Programme](../ai-governance/readme.md) | Ongoing governance of PCM-001 and CRT-001 post-acquisition |
| [Integration Management Programme](../integration-management/readme.md) | M&A integration context: policy application, risk register integration, data governance |
| [Emyzer Nexus Overview](../emyzer-nexus/readme.md) | Phase 2 programme overview and key governance decisions |
| [Portfolio Overview](../README.md) | Top-level narrative and 60-second review path |

---

*All content in this portfolio is a fictional case study. Framework and regulatory references are accurate as of the document publication dates.*

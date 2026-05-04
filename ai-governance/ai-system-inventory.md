# AI System Inventory and Classification Register

**Emyzer Nexus: AI Governance Programme**

---

## Document Information

| Attribute | Value |
|---|---|
| **Document ID** | AI-INV-001 |
| **Document Type** | Operational Register |
| **Version** | 1.0 |
| **Effective Date** | 2025-06-01 |
| **Owner** | CISO / AI Governance Committee |
| **Classification** | Internal Use |
| **Review Cadence** | Annual + upon any material change to a registered system |
| **Governing Policy** | [AI Governance Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/enterprise-policies/ai-governance-policy.md) |

---

## 1. Purpose

This register is the authoritative record of all artificial intelligence and machine learning systems owned, operated, or procured by Emyzer Nexus and its subsidiaries. It documents the formal EU AI Act risk tier classification of each system, the governance obligations that classification triggers, the current governance status, and the evidence maintained to demonstrate compliance.

The register is maintained by the GRC Team in the GRC platform, updated within 30 days of any system identification, acquisition, or material change, and reviewed at each quarterly AI Governance Committee meeting. It serves as:

- The primary evidence of EU AI Act Article 9 risk management system establishment [VERIFY]
- The basis for conformity assessment scoping and prioritisation
- The single source of truth for AI system ownership and lifecycle status
- Audit evidence of AI governance programme operation

All systems classified as High-Risk are subject to the full conformity obligations set out in Section 6. Systems classified as Limited Risk are subject to transparency obligations only. Systems classified as Minimal Risk are subject to standard information security controls.

---

## 2. System Registry Summary

| System ID | System Name | Origin | EU AI Act Risk Tier | AI System Owner | Deployment Status | Last Classification Review |
|---|---|---|---|---|---|---|
| PCM-001 | Predictive Customer Churn Model | Veridian AI (acquired Q4 2024) | **High-Risk** | VP, Customer Success | Active: in production | 2025-06-01 |
| CRT-001 | AI-Assisted Contract Review Tool | Veridian AI (acquired Q4 2024) | **High-Risk** | General Counsel | Active: restricted use pending DPA | 2025-06-01 |

---

## 3. Detailed System Profile: PCM-001

### Predictive Customer Churn Model

| Field | Detail |
|---|---|
| **System ID** | PCM-001 |
| **Full System Name** | Predictive Customer Churn Model |
| **Business Domain** | Sales and Customer Success: Retention Management |
| **Origin** | Veridian AI (acquired Q4 2024) |
| **Acquisition Date** | 2024-Q4 (exact date confidential) |
| **EU AI Act Risk Tier** | **High-Risk** [VERIFY: Annex III §5(b) applicability to commercial B2B churn scoring contexts] |
| **AI System Owner** | VP, Customer Success |
| **Deployment Status** | Active: in production |
| **Deployment Environment** | Internal AWS (Emyzer Nexus cloud tenancy, eu-west-1 region) |

#### Development and Technical Profile

| Field | Detail |
|---|---|
| **Development Approach** | Supervised machine learning: Random Forest ensemble model; retrained on a quarterly cycle using 36 months of rolling historical data |
| **Model Architecture** | Ensemble of 500 decision trees; hyperparameters optimised via cross-validation at each retraining cycle |
| **Training Dataset** | Approximately 48,000 B2B client records drawn from Veridian AI's client base; data types: product usage telemetry (daily active usage, feature adoption, session frequency), support ticket history (volume, severity distribution, resolution time), billing records (payment timeliness, contract value, upgrade/downgrade events), contract metadata (contract age, renewal history, tier) |
| **Training Dataset Provenance** | Collected by Veridian AI pre-acquisition; provenance documentation incomplete: gap identified (see AI-RISK-2025-004) |
| **Input Variables at Inference** | Product usage telemetry (7-day rolling average, 30-day rolling average, year-on-year delta), open support ticket count (by severity), days since last support ticket, billing payment status, contract days remaining, contract tier, customer segment (Enterprise / Mid-Market / SMB) |
| **Output Format** | Churn probability score (0.00–1.00) mapped to four risk tiers: Low (<0.25), Medium (0.25–0.50), High (0.50–0.75), Critical (>0.75) |
| **Output Consumers** | Sales and Customer Success teams receive a weekly scored client list via internal dashboard; scores used to prioritise retention outreach calls and escalation workflows |
| **Retraining Cycle** | Quarterly; retraining triggered by calendar schedule or when drift detection threshold is exceeded (performance degradation >5% on held-out validation set) |
| **Third-Party Dependencies** | None for the ML model itself; AWS infrastructure for hosting; no external AI API dependencies |
| **Data Retention (Training)** | Not yet formally governed: gap identified, DPO review in progress |

#### Classification Rationale

PCM-001 is classified as High-Risk under EU AI Act Annex III [VERIFY]. The classification reflects that the system's outputs materially influence business decisions that affect clients' continued access to services: clients scoring in the High and Critical tiers are subject to proactive outreach that may include contract renegotiation offers, pricing adjustments, and service-level discussions. Where such outreach does not occur (due to a missed or incorrect score), a client's access to continued service may be effectively affected by an omission driven by the AI output.

The AI Governance Committee reviewed the classification rationale at its 2025-06-01 meeting and confirmed the High-Risk designation under the precautionary principle [VERIFY: confirm correct Annex III category], noting that while Annex III §5(b) is most directly applicable to individual consumer creditworthiness, the committee assessed that the spirit of the provision applies to business decisions materially affecting ongoing service access in a B2B context.

**[VERIFY: Legal Counsel to confirm Annex III classification basis and whether PCM-001 falls within scope of EU AI Act implementation guidelines for B2B AI systems. Classification to be revisited if implementing acts provide clarifying guidance.]**

#### Known Limitations

- Model outputs are not explainable at the individual client level: the Random Forest ensemble cannot generate a per-client rationale for the assigned score
- Quarterly retraining creates a lag period during which model performance may degrade if client behavior patterns shift rapidly
- Training data reflects Veridian AI's legacy client base only; model performance for Emyzer Technology's client segments (hardware and managed services clients) has not been validated

#### Current Governance Status

| Governance Obligation | Status | Evidence Reference | Notes |
|---|---|---|---|
| Conformity assessment (Article 9 [VERIFY]) | In Progress | AI-GOV-CA-PCM-001 | Initiated 2025-06-01; target completion 2025-09-30 |
| Technical documentation (Article 11 [VERIFY]) | Partial | AI-GOV-TD-PCM-001-DRAFT | Engineering documentation partially available from Veridian AI; gaps being remediated |
| Human oversight protocol (Article 14 [VERIFY]) | Documented | AI-GOV-HO-PCM-001 | Human override procedure documented; CS managers can suppress or override score-triggered workflows |
| Post-market monitoring (Article 72 [VERIFY]) | Active | GRC Platform: PCM-001 Monitoring | Monthly performance review; quarterly drift assessment; Q1 2025 baseline established |
| Operator training | Complete | LMS: PCM-001 Training Module | 23 designated operators trained; 100% completion (see training completion record) |
| Training data governance (Article 10 [VERIFY]) | Gap | — | DPO review in progress; retention schedule not yet documented |

---

## 4. Detailed System Profile: CRT-001

### AI-Assisted Contract Review Tool

| Field | Detail |
|---|---|
| **System ID** | CRT-001 |
| **Full System Name** | AI-Assisted Contract Review Tool |
| **Business Domain** | Legal: Contract Review and Risk Assessment |
| **Origin** | Veridian AI (acquired Q4 2024) |
| **Acquisition Date** | 2024-Q4 |
| **EU AI Act Risk Tier** | **High-Risk** [VERIFY: Annex III applicability to legal decision-support AI tools; precautionary classification confirmed by AI Governance Committee pending implementing act guidance] |
| **AI System Owner** | General Counsel |
| **Deployment Status** | Active: **restricted use** pending DPA execution with LLM API vendor |
| **Use Restriction** | Tool may only be used for contracts containing no personal data or commercially sensitive third-party information pending DPA execution (interim measure from 2025-01-15) |
| **Deployment Environment** | Internal cloud preprocessing layer (Emyzer Nexus AWS tenancy) + external LLM API call |

#### Development and Technical Profile

| Field | Detail |
|---|---|
| **Development Approach** | LLM-based natural language processing; Veridian AI engineering built a custom prompting layer and preprocessing pipeline on top of a third-party foundation model API |
| **Model Architecture** | Third-party foundation model accessed via API; custom system prompt engineering; document segmentation preprocessing layer; output parsing and formatting layer |
| **Input Processing** | PDF and DOCX contract documents ingested via preprocessing pipeline; documents segmented into clause-level chunks; each chunk submitted to LLM API with structured prompt context |
| **Output Format** | Clause-by-clause analysis (plain language summary of each clause); flagged anomalies (clauses deviating from standard templates); negotiation suggestions (areas where clause terms are unfavourable); compliance risk flags (potential conflicts with regulatory requirements) |
| **Output Consumers** | Legal team only (8 designated operators); outputs treated as first-pass analysis only: all outputs require solicitor review before acting |
| **Third-Party Dependency** | External LLM API, **CRITICAL DEPENDENCY**, vendor identity redacted pending contract review and DPA execution; tool is entirely non-functional if the API is unavailable, discontinued, or access is revoked |
| **Sub-processor Chains** | LLM API vendor may use sub-processors for model hosting; sub-processor list not yet obtained: gap identified |
| **Data Transmitted to External API** | Contract document text (clauses, commercial terms, party names, consideration amounts, conditions): may include personal data and commercially sensitive third-party information |

#### Classification Rationale

CRT-001 is classified as High-Risk under the EU AI Act [VERIFY] on the basis of the precautionary principle. The tool's outputs directly inform legal decisions with material financial and operational consequences: contract terms accepted or rejected on the basis of CRT-001 analysis may affect obligations worth hundreds of thousands of euros. The AI Governance Committee assessed that the risk profile, including the third-party LLM API dependency, the opacity of the model's reasoning, and the potential for confident but incorrect legal analysis (hallucination), warranted High-Risk classification and the corresponding conformity obligations.

**[VERIFY: Legal Counsel to assess whether CRT-001 falls within an Annex III category or whether the High-Risk classification is a voluntary precautionary election. Confirm treatment under EU AI Act Article 6 [VERIFY] if voluntary. Note that voluntary High-Risk classification triggers full conformity obligations.]**

#### Known Limitations

- **Hallucination risk**: LLM models can generate confident, plausible, but factually incorrect legal analysis; the tool's outputs cannot be treated as authoritative
- **Explainability**: The third-party LLM API provides no explanation of its reasoning; CRT-001 cannot tell a user why it flagged or recommended a particular position
- **Data privacy**: Contract text transmitted to the external API may include personal data and commercially sensitive information; GDPR Article 28 [VERIFY] compliance requires a DPA that has not yet been executed
- **Model opacity**: Emyzer Nexus has no visibility into the third-party model's training data, bias testing, or performance characteristics; EU AI Act Article 10 [VERIFY] requirements regarding training data quality cannot be directly satisfied

#### Current Governance Status

| Governance Obligation | Status | Evidence Reference | Notes |
|---|---|---|---|
| Conformity assessment (Article 9 [VERIFY]) | In Progress | AI-GOV-CA-CRT-001 | Initiated 2025-06-01; complex due to third-party API dependency; target 2025-12-31 |
| Technical documentation (Article 11 [VERIFY]) | **Gap: Critical** | — | Third-party API technical documentation not available; Emyzer Nexus cannot produce full Article 11 documentation without vendor cooperation |
| Human oversight protocol (Article 14 [VERIFY]) | Documented | AI-GOV-HO-CRT-001 | Mandatory solicitor review of all outputs; override policy: all CRT-001 analysis treated as advisory only |
| Post-market monitoring (Article 72 [VERIFY]) | **Partial** | GRC Platform: CRT-001 | Output quality sampling programme in place; hallucination rate tracking; API availability monitoring |
| Operator training | Complete | LMS: CRT-001 Training Module | 8 designated Legal operators trained; training includes hallucination awareness and override protocol |
| Data processing agreement (GDPR Art.28 [VERIFY]) | **Gap: Critical** | — | DPA with LLM API vendor not yet executed; use restriction in effect; DPA target: 2025-09-30 |
| LLM API vendor due diligence | In Progress | SR-2025-001 | AI-specific due diligence initiated; approved with conditions pending DPA |

---

## 5. Classification History

| System ID | Previous Tier | Current Tier | Effective Date | Committee Meeting | Decision Rationale |
|---|---|---|---|---|---|
| PCM-001 | Unclassified (pre-acquisition) | High-Risk | 2025-06-01 | AI-GOV-MTG-2025-001 | Precautionary classification; Annex III §5(b) applicability assessed; outputs influence service access decisions |
| CRT-001 | Unclassified (pre-acquisition) | High-Risk | 2025-06-01 | AI-GOV-MTG-2025-001 | Precautionary classification; material legal decision influence; third-party LLM dependency; hallucination risk |

---

## 6. Governance Obligations by Risk Tier

### High-Risk Systems (PCM-001, CRT-001)

| Obligation | EU AI Act Article | Requirement Summary | PCM-001 Status | CRT-001 Status |
|---|---|---|---|---|
| Risk Management System | Article 9 [VERIFY] | Establish and maintain an AI risk management system throughout the lifecycle; identify, estimate, evaluate, and adopt risk mitigation measures | In Progress | In Progress |
| Data Governance | Article 10 [VERIFY] | Training, validation, and test data meets quality requirements; data provenance documented; biases examined; relevance and completeness assessed | Gap (provenance incomplete) | Gap (API training data unknown) |
| Technical Documentation | Article 11 [VERIFY] | Complete technical documentation maintained before deployment; kept up-to-date; available to authorities on request | Partial | Gap: Critical |
| Transparency to Deployers | Article 13 [VERIFY] | System provides sufficient transparency for deployers to interpret outputs; instructions for use; capability and limitation disclosure | Partial (no individual explanation) | Partial (limitation disclosures in operator training) |
| Human Oversight | Article 14 [VERIFY] | Human oversight measures enabling monitoring, intervention, override, and system suspension | Documented | Documented |
| Accuracy, Robustness, Cybersecurity | Article 15 [VERIFY] | Declared performance level; resilience to errors and adversarial inputs; cybersecurity measures | Partial (performance baselined; adversarial testing not completed) | Gap (cannot test opaque third-party model) |
| Post-Market Monitoring | Article 72 [VERIFY] | Post-market monitoring plan; data collection; performance anomaly reporting | Active | Partial |
| Serious Incident Reporting | Article 73 [VERIFY] | Report serious incidents to national market surveillance authority; defined timeframes | Procedure documented; no incidents to date | Procedure documented; no incidents to date |

---

## 7. Evidence Index

| Evidence Type | System of Record | Owner | Retention Period |
|---|---|---|---|
| AI System Inventory Register | GRC Platform | GRC Team | Indefinite (current version with full version history) |
| Classification Decisions and Rationale | GRC Platform | AI Governance Committee | Life of system + 7 years |
| Conformity Assessment Reports | Document Repository | AI System Owner | Life of system + 7 years |
| Technical Documentation Packages | Document Repository | AI System Owner | Life of system + 7 years |
| Human Oversight Validation Reports | Document Repository | AI System Owner | 5 years |
| Post-Market Monitoring Reports | GRC Platform | AI System Owner | 5 years |
| Operator Training Records | Learning Management System | Human Resources | 3 years |
| Override and Intervention Logs | GRC Platform / Application Logs | AI System Owner | 3 years |
| AI Governance Committee Minutes | Document Repository | CISO | 7 years |
| AI Vendor Due Diligence Records | GRC Platform | GRC Team / Vendor Risk Manager | Contract duration + 5 years |
| Data Processing Agreements | Legal Repository | Legal Counsel | Contract duration + 7 years |
| Classification Review Records | GRC Platform | AI Governance Committee | Life of system + 7 years |

---

## 8. Document Control

| Version | Date | Author | Changes |
|---|---|---|---|
| 1.0 | 2025-06-01 | GRC Team | Initial publication following AI Governance Committee classification decisions |

- **Document ID:** AI-INV-001
- **Classification:** Internal Use
- **Next Review Date:** 2026-06-01 (annual) or upon material change to any registered system

---

*This document was developed as part of the Emyzer Nexus Phase 2 AI Governance Programme and formatted for portfolio presentation.*

# AI Governance Programme

**Emyzer Nexus — Phase 2 GRC Programme**

---

> **Simulated Environment**
>
> Emyzer Nexus is a fictional organisation created for this GRC portfolio. All entities, personnel, systems, policies, risk entries, and regulatory scenarios described in this repository are invented for professional demonstration purposes. Framework and regulatory references — EU AI Act (Regulation 2024/1689), NIST AI RMF 1.0, ISO/IEC 42001:2023, and others — are accurate as of the document dates; their application to Emyzer Nexus is illustrative only. No real organisation, individual, or incident is represented.

---

## About This Programme

The Emyzer Nexus AI Governance Programme was established following the acquisition of Veridian AI in Q4 2024. The acquisition introduced two operational AI systems — a Predictive Customer Churn Model and an AI-Assisted Contract Review Tool — that required immediate formal governance under the EU AI Act (Regulation 2024/1689) [VERIFY].

Both systems were assessed and classified as High-Risk under the EU AI Act, triggering the full suite of conformity obligations defined in EU AI Act Title III [VERIFY]. This programme documents the governance structures, system classifications, control mappings, and risk assessments developed to meet those obligations.

The programme operates under the [AI Governance Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/enterprise-policies/ai-governance-policy.md) and is overseen by the AI Governance Committee, chaired by the CISO.

---

## Document Index

| Document | Description | Status |
|---|---|---|
| [AI Governance README](readme.md) | Programme overview and document index | ✓ Published |
| [AI System Inventory and Classification](ai-system-inventory.md) | Formal EU AI Act risk tier classification of PCM-001 and CRT-001; system profiles, governance obligations, and classification history | ✓ Published |
| [EU AI Act Control Mapping](eu-ai-act-mapping.md) | Article-by-article compliance mapping for Articles 9, 10, 11, 13, 14, 15, 72, and 73; gap identification and remediation priorities | ✓ Published |
| [AI System Risk Assessments](risk-assessments.md) | Risk assessments for PCM-001 and CRT-001 applying the Phase 1 methodology extended with AI-specific categories: model drift, training data bias, explainability gaps, third-party model dependency | ✓ Published |

---

## Governing Policies

| Policy | Owner | Scope |
|---|---|---|
| [AI Governance Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/enterprise-policies/ai-governance-policy.md) | CISO | Parent governance framework; AI system lifecycle, classification, conformity, human oversight, post-market monitoring, incident management, and retirement |
| [Model Risk Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/enterprise-policies/model-risk-policy.md) | CRO | Operational model lifecycle; bias testing cadence; explainability standards; human oversight validation; model failure incident response |
| [Third-Party Risk Management Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/third-party-risk-management-policy.md) | ISO | Vendor risk requirements; extended by AI Vendor Risk Due Diligence Addendum for AI-specific obligations |
| [Privacy and Data Protection Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/enterprise-policies/privacy-and-data-protection-policy.md) | DPO | Training data governance; GDPR obligations for AI system data processing; data subject rights in automated decision contexts |

---

## AI Systems in Scope

| System ID | System Name | Origin | EU AI Act Risk Tier | Status |
|---|---|---|---|---|
| PCM-001 | Predictive Customer Churn Model | Veridian AI (acquired Q4 2024) | High-Risk | Active — Under Governance |
| CRT-001 | AI-Assisted Contract Review Tool | Veridian AI (acquired Q4 2024) | High-Risk | Active — Under Governance (restricted use pending DPA) |

---

## Frameworks Referenced

| Framework | Application |
|---|---|
| **[EU AI Act (Regulation 2024/1689)](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32024R1689)** [VERIFY] | Risk tier classification (Annex III); High-Risk system obligations (Articles 9–15); post-market monitoring (Article 72); serious incident reporting (Article 73) |
| **[NIST AI Risk Management Framework (AI RMF 1.0)](https://www.nist.gov/artificial-intelligence/ai-risk-management-framework)** | Programme structure: Govern, Map, Measure, Manage functions aligned to AI system lifecycle |
| **[ISO/IEC 42001:2023](https://www.iso.org/standard/81230.html)** | AI management system requirements; Clause 8 operational controls; Annex A AI management controls |
| **[ISO/IEC 23894:2023](https://www.iso.org/standard/77304.html)** | AI risk management guidance; AI-specific threat and risk scenario identification |
| **[GDPR (Regulation 2016/679)](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32016R0679)** [VERIFY] | Training data governance; data subject rights in automated decision-making contexts (Article 22 [VERIFY]) |

---

## Related Programmes

| Programme | Link | Relationship |
|---|---|---|
| M&A Integration Management | [integration-management/](https://github.com/olusolaxakanji/information-security-grc-portfolio/tree/main/integration-management) | Provides governance context for Veridian AI acquisition; M&A Risk Assessment covers AI-specific integration risks |
| Enterprise Policies | [enterprise-policies/](https://github.com/olusolaxakanji/information-security-grc-portfolio/tree/main/enterprise-policies) | AI Governance Policy and Model Risk Policy govern this programme |
| Phase 1 Controls Library | [controls/](https://github.com/olusolaxakanji/information-security-grc-portfolio/tree/main/controls) | ET-CTRL-008 (AI System Inventory and Risk Classification Review) is the operational control supporting this programme |
| Risk Assessments | [risk-assessments/](https://github.com/olusolaxakanji/information-security-grc-portfolio/tree/main/risk-assessments) | Phase 1 methodology extended with AI-specific categories for AI system risk assessments in this folder |

---

*All content in this portfolio is a fictional case study developed for professional demonstration purposes. Framework and regulatory references are accurate as of the document publication dates.*

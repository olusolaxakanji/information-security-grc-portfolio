# AI Governance Programme

**Emyzer Nexus: Phase 2 | Fictional case study.**

> All entities, systems, personnel, and risk findings are invented for professional demonstration purposes. EU AI Act, NIST AI RMF 1.0, ISO/IEC 42001:2023, and other framework references are accurate as of the document dates. `[VERIFY]` tags flag regulatory citations requiring legal confirmation before use in a real context.

---

## The Problem This Programme Was Built to Solve

Veridian AI's two production AI systems had never been assessed under the EU AI Act before the acquisition closed. From the moment Emyzer Nexus became the legal operator, it inherited the compliance gap.

Both systems were classified as High-Risk under EU AI Act Annex III [VERIFY]:

| System ID | System | EU AI Act Risk Tier | Governance Status at Acquisition |
|---|---|---|---|
| PCM-001 | Predictive Customer Churn Model | High-Risk | In production. No conformity assessment on record. |
| CRT-001 | AI-Assisted Contract Review Tool | High-Risk | In production. GDPR data processor obligations for external LLM API unresolved. |

High-Risk classification triggers the full suite of conformity obligations under EU AI Act Title III [VERIFY]: risk management systems under Article 9, training data governance under Article 10, technical documentation under Article 11, transparency requirements under Article 13, human oversight mechanisms under Article 14, and accuracy and robustness standards under Article 15. None of these were in place at acquisition close.

CRT-001 use was restricted to contracts containing no personal data immediately on acquisition close, pending execution of a Data Processing Agreement with the LLM API vendor. This restriction was implemented on legal advice given the unresolved GDPR Article 28 [VERIFY] position.

---

## What This Programme Produced

| Document | What it resolves |
|---|---|
| [AI System Inventory and Classification](ai-system-inventory.md) | Formal EU AI Act risk tier classification of PCM-001 and CRT-001. Includes system profiles, the classification rationale under Annex III, Article 9 risk management system requirements, and the full set of conformity obligations that apply per classification. |
| [EU AI Act Control Mapping](eu-ai-act-mapping.md) | Article-by-article control mapping for Articles 9, 10, 11, 13, 14, 15, 72, and 73. Each gap is identified with a remediation priority and named owner. Gaps are not left as open findings. |
| [AI System Risk Assessments](risk-assessments.md) | Risk assessments for PCM-001 and CRT-001 using the Phase 1 methodology extended with AI-specific risk categories: model drift, training data bias, explainability gaps, and third-party model dependency. The methodology is extended, not replaced, so risk findings are comparable across the full enterprise risk register. |

---

## Governing Policies

| Policy | What it establishes |
|---|---|
| [AI Governance Policy](../enterprise-policies/ai-governance-policy.md) | Parent governance framework. Creates the AI Governance Committee, defines High-Risk system obligations, sets conditions for post-market monitoring activation, and establishes prohibited AI practices. |
| [Model Risk Policy](../enterprise-policies/model-risk-policy.md) | Operational model lifecycle controls. Bias testing cadence, human oversight validation, explainability standards, and model failure incident response. Addresses the specific failure modes of PCM-001 (training data bias, model drift) and CRT-001 (LLM hallucination, third-party model dependency). |
| [Privacy and Data Protection Policy](../enterprise-policies/privacy-and-data-protection-policy.md) | Training data governance for PCM-001. GDPR data processor obligations for CRT-001's LLM API. Data subject rights in automated decision contexts. |
| [Third-Party Risk Management Policy](../policies/third-party-risk-management-policy.md) | Extended by the AI Vendor Risk Due Diligence Addendum for AI-specific vendor obligations not covered in the Phase 1 base policy. |

---

## AI Governance Committee

The AI Governance Committee is the classification and conformity assessment authority for all AI systems at Emyzer Nexus. It is not a vague stakeholder group. It has defined cross-functional membership, a quarterly cadence, and an emergency convening obligation: within 5 business days of a significant AI incident.

**Authority includes:** AI system risk classification decisions, conformity assessment governance, post-market monitoring oversight, risk acceptance for High-Risk systems, and emergency response coordination for material AI incidents.

---

## Frameworks Applied

| Framework | Application |
|---|---|
| EU AI Act (Regulation 2024/1689) [VERIFY] | Risk tier classification (Annex III); High-Risk system obligations (Articles 9-15); post-market monitoring (Art. 72); serious incident reporting (Art. 73) |
| NIST AI RMF 1.0 | Programme structure: Govern, Map, Measure, Manage functions applied to AI system lifecycle |
| ISO/IEC 42001:2023 | AI management system requirements; Clause 8 operational controls; Annex A AI management controls |
| ISO/IEC 23894:2023 | AI risk management guidance; AI-specific threat and risk scenario identification |
| GDPR (Regulation 2016/679) [VERIFY] | Training data governance; data subject rights in automated decision-making contexts |

---

## Related Documentation

| Document | Description |
|---|---|
| [Portfolio Overview](../README.md) | Top-level narrative and 60-second review path |
| [Emyzer Nexus Overview](../emyzer-nexus/readme.md) | Phase 2 programme context and key governance decisions |
| [Integration Management Programme](../integration-management/readme.md) | M&A integration context: how the AI governance problem was scoped at acquisition close |
| [Veridian AI Documentation](../veridian-ai/README.md) | Acquisition-stage risk assessment and AI vendor due diligence addendum |

---

*All content in this portfolio is a fictional case study. Framework and regulatory references are accurate as of the document publication dates.*

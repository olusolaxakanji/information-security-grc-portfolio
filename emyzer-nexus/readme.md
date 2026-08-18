# Emyzer Nexus: Phase 2 GRC Programme

**Post-acquisition parent entity. Fictional case study.**

> All entities, personnel, systems, policies, risk entries, and regulatory scenarios in this portfolio are invented for professional demonstration purposes. Framework references (EU AI Act, ISO 27001:2022, NIST CSF 2.0, GDPR, and others) are accurate as of the document dates; their application to Emyzer Nexus is illustrative only. `[VERIFY]` tags flag regulatory citations that require legal confirmation before use in a real context.

---

## The Governance Problem Phase 2 Was Built to Solve

Emyzer Technology acquired Veridian AI in Q4 2024. Veridian was an AI-native startup with two operational AI systems and no formal GRC programme. From the moment the acquisition closed, Emyzer Nexus inherited Veridian's compliance gaps as its own.

Four specific problems required immediate governance response:

**1. AI governance under the EU AI Act.** Veridian's two systems (a Predictive Customer Churn Model and an AI-Assisted Contract Review Tool) were in production without conformity assessments. Both were classified as High-Risk under EU AI Act Annex III [VERIFY]. Full conformity obligations under Articles 9-15 applied from acquisition close, not from some future compliance date.

**2. M&A policy integration.** Veridian had no documented policies. Emyzer Technology's Phase 1 policies were written for a hardware and services business, not an AI-native entity. Absorbing Veridian expanded the scope of nearly every existing policy and created governance domains that Phase 1 had not addressed.

**3. Expanded GDPR obligations.** Veridian's churn model trained on customer PII. Its contract review tool transmitted contract data to an external LLM API. Neither data flow had a formal GDPR basis. Both became Emyzer Nexus compliance gaps on Day 0.

**4. AI vendor risk.** Standard TPRM controls were not designed to evaluate LLM API providers. Model transparency, training data provenance, bias audit availability, and AI error liability were not covered in the Phase 1 Third-Party Risk Management Policy.

---

## Corporate Structure

```
Emyzer Nexus  (parent: Phase 2 GRC programme)
├── Emyzer Technology  (subsidiary: Phase 1 GRC programme in effect as subsidiary documentation)
└── Veridian AI  (acquired: governance integration in progress)
```

Emyzer Nexus enterprise policies take precedence. Where Emyzer Nexus has not issued a policy in a given domain, the applicable Emyzer Technology Phase 1 policy governs. Veridian AI legacy documentation (where any existed) was superseded by Emyzer Nexus and Emyzer Technology policies from acquisition close. Full hierarchy and transition timeline are in the [M&A GRC Integration Charter](../integration-management/ma-grc-integration-charter.md).

---

## Key Governance Decisions Made

The Integration Management Committee (IMC), chaired by the CRO and approved by the CEO, made seven binding decisions at acquisition close:

1. **Immediate policy application (Day 0).** All Emyzer Nexus and Emyzer Technology policies applied to Veridian AI personnel from acquisition close. Personnel acknowledged policies within 30 days.

2. **AI system classification.** PCM-001 and CRT-001 were classified as High-Risk under EU AI Act Annex III [VERIFY] pending formal conformity assessment. Interim human review protocols were implemented for both systems immediately.

3. **CRT-001 restricted use.** CRT-001 use was restricted to contracts containing no personal data pending execution of a Data Processing Agreement with the LLM API vendor. This restriction was implemented on legal advice given the unresolved GDPR Article 28 [VERIFY] position.

4. **Integration Management Committee formed.** A monthly IMC was established comprising the CRO (chair), CISO, CTO, Legal Counsel, and GRC Lead, with authority to make integration governance decisions within the remit of the charter.

5. **External GRC consultant engaged.** An external consultant was engaged for a 6-month sprint to support risk register integration, policy rationalization, and AI governance documentation given integration workstream volume.

6. **Phase 1 policies remain in effect.** No Phase 1 policy was retired without a formal rationalization decision recorded in the Policy Rationalization Roadmap.

7. **AI Governance Committee convened.** The AI Governance Committee was convened in January 2025. Its first meeting was dedicated to formal classification of PCM-001 and CRT-001.

---

## Programme Areas

### M&A Integration Governance

The integration programme answers three questions every acquisition creates: which policies govern the acquired entity from Day 0, what compliance gaps were inherited, and what existing documentation needs to change to reflect the expanded scope.

| Document | What it resolves |
|---|---|
| [M&A GRC Integration Charter](../integration-management/ma-grc-integration-charter.md) | Establishes the post-acquisition policy hierarchy. Defines which governance body has authority to accept inherited risk. Sets the conditions that trigger a policy review or retirement. Includes a 15-entry integration risk register with owners and target resolution dates. |
| [Policy Rationalization Roadmap](../integration-management/rationalization-roadmap.md) | Phase 1 policies were written for Emyzer Technology as a standalone entity. This document schedules their review under the expanded Nexus scope, identifies conflicts between legacy and new obligations, and prioritizes remediation order. |
| [M&A Risk Assessment](../integration-management/ma-risk-assessment.md) | Formal risk register for GRC risks introduced by the acquisition across five categories: Technology, Regulatory, Data/Privacy, Personnel, and Operational. |

### AI Governance Programme

Veridian's two systems entered production without conformity assessments. The AI governance programme was built to close that gap and establish ongoing governance for both systems under the EU AI Act.

| Document | What it resolves |
|---|---|
| [AI Governance Policy](../enterprise-policies/ai-governance-policy.md) | Parent-level policy governing AI/ML development, acquisition, validation, monitoring, and retirement across Emyzer Nexus. Creates the AI Governance Committee, defines High-Risk system obligations, and sets conditions for post-market monitoring activation. |
| [Model Risk Policy](../enterprise-policies/model-risk-policy.md) | Each inherited system had specific failure modes: LLM hallucination in CRT-001, training data bias and model drift in PCM-001, and shared third-party model dependency. This policy sets the bias testing cadence, human oversight requirements, explainability standards, and model failure incident response procedures that address those modes specifically. |
| [AI System Inventory and Classification](../ai-governance/ai-system-inventory.md) | Formal EU AI Act risk tier classification of PCM-001 and CRT-001. Includes system profiles, Article 9 risk management system requirements, and the full set of conformity obligations per classification. |
| [EU AI Act Control Mapping](../ai-governance/eu-ai-act-mapping.md) | Article-by-article control mapping for Articles 9, 10, 11, 13, 14, 15, 72, and 73. Each gap is identified with a remediation priority and owner rather than left as an open finding. |
| [AI System Risk Assessments](../ai-governance/risk-assessments.md) | Phase 1 risk methodology applied to AI-specific risk categories: model drift, training data bias, explainability gaps, and third-party model dependency. The methodology is extended, not replaced. |
| [AI Vendor Risk Due Diligence Addendum](../veridian-ai/vendor-risk-addendum/ai-vendor-risk-addendum.md) | Standard TPRM controls do not evaluate LLM API providers. This addendum extends the Phase 1 Third-Party Risk Management Policy to cover model transparency, training data provenance, bias audit availability, EU AI Act compliance status, and contractual liability for model errors. |

### Enterprise Policies

Phase 2 enterprise policies govern Emyzer Nexus as the parent entity. They address obligations that the Phase 1 Emyzer Technology policies did not cover.

| Policy | What gap it closes | Frameworks |
|---|---|---|
| [AI Governance Policy](../enterprise-policies/ai-governance-policy.md) | Phase 1 had no AI governance framework. This policy creates the governance structure for AI systems across the expanded entity. | EU AI Act, NIST AI RMF 1.0, ISO/IEC 42001:2023 |
| [Model Risk Policy](../enterprise-policies/model-risk-policy.md) | Phase 1 had no model lifecycle controls. This policy establishes operational requirements for the two inherited High-Risk systems. | SR 11-7, NIST AI RMF, EU AI Act |
| [Privacy and Data Protection Policy](../enterprise-policies/privacy-and-data-protection-policy.md) | Veridian's data processing activities (PII-trained models, external LLM API) created GDPR obligations not addressed in Phase 1. This policy establishes the lawful basis, data processor obligations, and subject rights procedures for those activities. | GDPR, UK GDPR, ISO 27701:2019 |
| [Security Awareness and Training Policy (Tier 2)](../enterprise-policies/security-awareness-and-training-policy.md) | EU AI Act Article 14 requires human oversight training for staff interacting with High-Risk AI systems. The Phase 1 training policy did not include this obligation. | ISO 27001:2022, NIST SP 800-50, EU AI Act Art. 14 |

---

## Governance Authority

| Role / Body | Authority |
|---|---|
| **CEO** | Board-level accountability for responsible AI governance; approves AI Governance Policy and material AI strategy changes |
| **CISO** | Executive oversight of ISMS and AI governance programme; chairs AI Governance Committee; approves risk acceptance for High-Risk systems |
| **CRO** | Enterprise risk register ownership; chairs Integration Management Committee; risk appetite governance |
| **DPO** | Privacy programme ownership; GDPR obligations for AI training data and external API data processing; DPIA governance |
| **CTO** | AI system technical governance; human oversight mechanism implementation; change management for AI systems |
| **AI Governance Committee** | AI system risk classification authority; EU AI Act conformity assessment governance; post-market monitoring oversight. Meets quarterly and on an emergency basis within 5 business days of a significant AI incident. |
| **Integration Management Committee** | M&A integration governance; monthly cadence during integration period; policy hierarchy oversight; inherited risk acceptance authority |

---

## Frameworks Applied

| Framework | Application in Phase 2 |
|---|---|
| EU AI Act (Regulation 2024/1689) [VERIFY] | Primary regulatory driver; classification of PCM-001 and CRT-001; Articles 9-15 conformity obligations; post-market monitoring (Art. 72); serious incident reporting (Art. 73) |
| NIST AI RMF 1.0 | AI governance programme structure: Govern, Map, Measure, Manage functions applied to AI system lifecycle |
| ISO/IEC 42001:2023 | AI management system requirements; Clause 8 operational controls; Annex A AI management controls |
| ISO 27001:2022 | ISMS continuity; policy hierarchy for expanded scope; supplier relationship controls |
| GDPR (Regulation 2016/679) [VERIFY] | Training data governance; data processor obligations for LLM API; data subject rights in automated decision contexts |
| ISO 31000:2018 | M&A risk identification and treatment methodology |
| NIST CSF 2.0 | Govern (GV) function applied to post-acquisition GRC integration |

---

## Related Documentation

| Document | Description |
|---|---|
| [Portfolio Overview](../README.md) | Top-level narrative, 60-second review path, and skills demonstrated |
| [Emyzer Technology Overview](../emyzer-technology/README.md) | Phase 1 GRC programme: 10 policies, risk programme, business continuity |
| [AI Governance Programme](../ai-governance/readme.md) | AI programme detail: system inventory, EU AI Act mapping, risk assessments |
| [Integration Management Programme](../integration-management/readme.md) | M&A integration detail: charter, rationalization roadmap, M&A risk assessment |
| [CONTRIBUTING.md](../CONTRIBUTING.md) | How changes are proposed, reviewed, approved, and merged |

---

*All content in this portfolio is a fictional case study developed for professional demonstration purposes. Framework and regulatory references are accurate as of the document publication dates.*

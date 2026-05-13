# Emyzer Technology: Phase 1 GRC Programme

**Foundational GRC build. Fictional case study.**

> All entities, personnel, systems, policies, risk entries, and regulatory scenarios in this portfolio are invented for professional demonstration purposes. Framework references (ISO 27001:2022, NIST CSF 2.0, GDPR, and others) are accurate as of the document dates; their application to Emyzer Technology is illustrative only.

---

## What Phase 1 Builds and Why It Matters

Phase 1 establishes the governance baseline that Phase 2 depends on. Before Emyzer Technology acquired Veridian AI, it needed a functioning GRC programme: documented policies that actually govern behaviour, a risk methodology that produces defensible decisions, and business continuity documentation grounded in real operational data.

Without Phase 1, Phase 2 has nothing to extend. The M&A Integration Charter works because there is a policy hierarchy to apply to the acquired entity. The AI Governance Policy works because there is a risk methodology to extend with AI-specific categories. The Phase 2 Tier 2 Training Policy works because there is a Phase 1 training programme to build on.

All Phase 1 artefacts are implemented in ServiceNow GRC and remain in effect as subsidiary documentation under Emyzer Nexus.

---

## Position in the Corporate Structure

Emyzer Technology is a subsidiary of Emyzer Nexus, the post-acquisition parent entity formed following the acquisition of Veridian AI in Q4 2024. Phase 1 covers the period before that acquisition: the GRC programme built for Emyzer Technology as a standalone entity.

```
Emyzer Nexus  (parent: Phase 2)
├── Emyzer Technology  (subsidiary: Phase 1 GRC programme, this folder)
└── Veridian AI  (acquired: governance integration in progress)
```

Where Emyzer Nexus has not issued a policy in a given domain, the applicable Phase 1 policy governs. No Phase 1 policy is retired without a formal rationalization decision recorded in the [Policy Rationalization Roadmap](../integration-management/rationalization-roadmap.md).

---

## Security Policies

Ten core information security policies developed for Emyzer Technology and implemented in ServiceNow GRC. Each policy contains a full evidence index specifying the system of record, owner, and retention period for every required evidence type.

| Policy | Key design decision | Frameworks |
|---|---|---|
| [Information Security Policy](../policies/information-security-policy.md) | Parent policy establishing the ISMS. Sets the Security Steering Committee as the exception escalation authority and defines the review cadence that all other policies inherit. Without this policy, exceptions and reviews have no governance home. | NIST CSF 2.0, ISO 27001:2022, COBIT |
| [Access Control Policy](../policies/access-control-policy.md) | Role-based access with privileged access controls and access review attestation requirements. At Phase 2, the AI Governance Committee is added as an access authority for AI system records, extending rather than replacing the Phase 1 framework. | NIST SP 800-53, ISO 27001:2022 A.5.15-A.5.18, COBIT DSS05 |
| [Incident Management Policy](../policies/incident-management-policy.md) | IRT activation criteria are defined at incident classification, not at escalation. This design choice prevents the assessment delay that commonly causes organisations to miss the 72-hour GDPR notification window. A 4-hour initial assessment SLA reinforces that timeline. | NIST SP 800-61, ISO 27035, GDPR Art. 33-34 |
| [Risk Management Policy](../policies/risk-management-policy.md) | Establishes the 5x5 hybrid scoring matrix used in all Phase 1 and Phase 2 risk assessments. Defines the materiality threshold above which Risk Management Committee formal acceptance is required, ensuring risk acceptance decisions are governed rather than informal. | ISO 31000:2018, NIST CSF 2.0, COSO ERM |
| [BC/DR Policy](../policies/bcdr-policy.md) | Recovery objectives are grounded in a 42-stakeholder BIA rather than estimated. Four-tier process prioritisation and financial exposure quantification across 12 critical processes give the RTO/RPO targets operational meaning. | ISO 22301:2019, NIST SP 800-34 |
| [Change Management and Configuration Policy](../policies/change-management-and-configuration-policy.md) | Three-tier change classification with defined CAB authority limits. At Phase 2, AI system material changes are escalated to the AI Governance Committee rather than handled through standard CAB review, extending this policy's change authority structure. | ITIL 4, ISO 27001:2022, COBIT BAI06 |
| [Acceptable Use Policy](../policies/acceptable-use-policy.md) | Covers personal device use, shadow IT, and staff use of AI tools. The AI tool provisions were written with awareness of the Veridian AI acquisition context, reducing the policy update burden at Phase 2. | ISO 27001:2022 A.5.10, NIST CSF |
| [Data Classification Policy](../policies/data-classification-policy.md) | Four-tier classification (Public, Internal, Confidential, Restricted) with handling, labeling, and disposal requirements per tier. At Phase 2, AI training data is classified under this scheme and subject to additional GDPR controls without requiring a new classification framework. | NIST SP 800-60, ISO 27001:2022 A.5.12-A.5.13, GDPR |
| [Third-Party Risk Management Policy](../policies/third-party-risk-management-policy.md) | Risk tiering criteria for vendors with review cadences by tier. At Phase 2, the AI Vendor Risk Due Diligence Addendum extends this policy for LLM API providers where model transparency, training data provenance, and AI error liability require assessment beyond the standard TPRM controls. | ISO 27036, NIST SP 800-161, NIST CSF ID.SC |
| [Security Awareness and Training Policy](../policies/security-awareness-and-training-policy.md) | Completion tracking and role-based curriculum requirements. At Phase 2, a Tier 2 policy adds EU AI Act Article 14 human oversight training obligations for staff interacting with High-Risk AI systems. The Phase 1 programme is the curriculum baseline that obligation is added to. | ISO 27001:2022 A.6.3, NIST SP 800-50 |

---

## Risk Assessment Programme

| Artefact | What it shows |
|---|---|
| [Risk Assessment Methodology](../risk-assessments/risk-assessment-methodology.md) | Six-step hybrid qualitative/quantitative methodology. 5x5 scoring matrix with inherent and residual rating distinction. Tiered monitoring cadences by residual rating level: Critical risks are reviewed monthly, High risks quarterly, Medium risks semi-annually. Multi-framework alignment across NIST SP 800-30, ISO 27005, and FAIR. At Phase 2, the methodology is extended with AI-specific risk categories rather than replaced. |
| [Asset Risk Register](../risk-assessments/asset-risk-register.md) | 15 entries across information security, privacy, operational, and third-party risk categories. One entry documents a budget-blocked Critical risk at its actual residual rating rather than adjusted downward to match available resources. The budget constraint is identified as the root cause and the risk is escalated accordingly. That entry demonstrates that the programme documents actual risk posture, not a posture shaped by what is comfortable to report. |
| [Risk Appetite Statement](../risk-assessments/risk-appetite-statement.md) | Domain-specific tolerance thresholds covering information security, privacy, operational, and third-party risk. Defines unacceptable risk conditions that cannot be accepted regardless of compensating controls, setting a ceiling on risk acceptance decisions. Current posture is assessed against defined appetite at each review cycle. |

---

## Business Continuity

| Artefact | What it shows |
|---|---|
| [Business Impact Analysis Report](../business-continuity/business-impact-analysis-report.md) | 42-stakeholder interviews. Four-tier process prioritisation. RTO/RPO targets set per tier based on actual operational data. Financial exposure quantified across 12 critical processes. Recovery objectives in the BC/DR Policy trace directly back to this analysis, so the targets are defensible during an audit or a real incident. |
| [Business Continuity Plan](../business-continuity/business-continuity-plan.md) | Activation criteria, Crisis Management Team runbook, five recovery scenarios with step-by-step procedures, and a multi-type exercise programme. The plan is designed to be usable under actual incident conditions, not just during tabletop reviews. |

---

## ServiceNow Evidence

Raw policy exports from ServiceNow GRC. These PDFs show ownership, approval workflows, validity periods, and compliance mappings as generated by the platform. They are evidence that the policies exist and were managed in a GRC platform, not documentation about platform work.

| Export | Linked Policy |
|---|---|
| Access Control Policy.pdf | [Access Control Policy](../policies/access-control-policy.md) |
| Business Continuity and DR Policy.pdf | [BC/DR Policy](../policies/bcdr-policy.md) |
| Incident Management Policy.pdf | [Incident Management Policy](../policies/incident-management-policy.md) |
| Information Security Policy.pdf | [Information Security Policy](../policies/information-security-policy.md) |
| Risk Management Policy.pdf | [Risk Management Policy](../policies/risk-management-policy.md) |

All exports are in [/servicenow-evidence/](../servicenow-evidence/).

---

## Governance Authority

| Role / Body | Authority in Phase 1 |
|---|---|
| **CISO** | Executive sponsor of the ISMS; final approver on all security policies |
| **Information Security Officer** | ISMS operational ownership; policy drafting; exception approval; day-to-day compliance monitoring |
| **CRO** | Enterprise risk register ownership; risk appetite governance; business continuity oversight |
| **Risk Management Committee** | Risk escalation and formal acceptance authority; approves treatment decisions above materiality thresholds; receives budget-blocked risk escalations |
| **Security Steering Committee** | Cross-functional ISMS governance body; exception escalation authority; programme performance oversight |
| **Change Advisory Board** | Change request governance; authorises standard, normal, and emergency changes |
| **Incident Response Team** | Incident identification, classification, containment, eradication, and recovery operations |
| **GRC Analyst** | Policy document reviewer; framework alignment verification; evidence register maintenance |

---

## Frameworks Applied

| Framework | Application in Phase 1 |
|---|---|
| ISO 27001:2022 | ISMS policy architecture; Annex A control alignment across all 10 policies |
| NIST CSF 2.0 | Security policy structure and control categories; ID.RA and ID.RM risk functions |
| NIST SP 800-30 Rev. 1 | Risk assessment process guidance; applied in risk methodology |
| ISO 31000:2018 | Enterprise risk management principles; risk appetite governance |
| ISO 22301:2019 | Business continuity management system; BIA and BCP structure |
| NIST SP 800-34 Rev. 1 | Contingency planning guidance; applied in BC/DR policy and BIA |
| GDPR | Data protection compliance; breach notification obligations in Incident Management Policy |
| COBIT 2019 | IT governance objectives; change management and access control alignment |
| ITIL 4 | IT service management; change advisory board structure |
| COSO ERM | Enterprise risk management integration in Risk Management Policy |

---

## Related Documentation

| Document | Description |
|---|---|
| [Portfolio Overview](../README.md) | Top-level narrative, 60-second review path, and skills demonstrated |
| [Emyzer Nexus Overview](../emyzer-nexus/readme.md) | Phase 2 GRC programme: M&A integration, AI governance, post-acquisition policies |
| [Enterprise Policies README](../enterprise-policies/readme.md) | Phase 2 policy architecture and design decisions |
| [CONTRIBUTING.md](../CONTRIBUTING.md) | How changes are proposed, reviewed, approved, and merged |

---

*All content in this portfolio is a fictional case study developed for professional demonstration purposes. Framework and regulatory references are accurate as of the document publication dates.*

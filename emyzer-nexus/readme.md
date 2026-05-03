# Emyzer Nexus — GRC Programme Overview

**Phase 2 Parent Entity | Information Security GRC Portfolio**

---

> **Simulated Environment**
>
> Emyzer Nexus is a fictional organisation created for this GRC portfolio. All entities, personnel, systems, policies, risk entries, and regulatory scenarios described in this repository are invented for professional demonstration purposes. Framework and regulatory references — ISO 27001:2022, NIST CSF 2.0, EU AI Act (Regulation 2024/1689), GDPR, and others — are accurate as of the document dates; their application to Emyzer Nexus is illustrative only. No real organisation, individual, or incident is represented. This portfolio was developed to demonstrate applied GRC competency across AI governance, M&A integration, policy architecture, risk programme design, business continuity, and compliance mapping using a fictionalized enterprise environment.

---

## About Emyzer Nexus

Emyzer Nexus is the post-acquisition parent entity formed in Q4 2024 when Emyzer Technology acquired Veridian AI. As parent entity, Emyzer Nexus holds governance authority over both subsidiaries and is the entity subject to EU AI Act obligations arising from Veridian AI's AI systems.

The Phase 2 GRC programme expands beyond the foundational work done in Phase 1 (Emyzer Technology) to address four new governance challenges introduced by the acquisition:

1. **AI governance under the EU AI Act** — two Veridian AI systems classified as High-Risk require full conformity governance
2. **M&A policy integration** — Veridian AI had no formal GRC programme; absorbing it into the Emyzer Nexus governance structure required deliberate integration management
3. **Expanded privacy obligations** — AI training data governance and external LLM API data transmission created new GDPR obligations not addressed in Phase 1
4. **Enhanced third-party risk** — AI vendor relationships require AI-specific due diligence beyond standard TPRM controls

---

## Corporate Structure

```
Emyzer Nexus  (parent — Phase 2 GRC programme)
├── Emyzer Technology  (subsidiary — Phase 1 GRC programme in effect as subsidiary documentation)
└── Veridian AI  (acquired entity — governance integration in progress under Integration Management Charter)
```

**Policy authority:** Emyzer Nexus enterprise policies take precedence. Where Emyzer Nexus has not issued a policy in a given domain, the applicable Emyzer Technology Phase 1 policy governs. Veridian AI legacy documentation (where it existed) was superseded by Emyzer Nexus/Emyzer Technology policies from acquisition close. See the [M&A GRC Integration Charter](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/integration-management/m%26a-grc-integration-charter.md) for full hierarchy and transition timeline.

---

## Governance Bodies and Accountable Roles

All named individuals below are fictional.

| Role / Body | Function | Referenced In |
|---|---|---|
| **Chief Executive Officer (CEO)** | Board-level accountability for responsible AI governance; approves AI Governance Policy and material AI strategy changes; receives quarterly AI risk briefings | AI Governance Policy, M&A GRC Integration Charter |
| **Chief Information Security Officer (CISO)** | Executive oversight of ISMS and AI governance programme; chairs AI Governance Committee; approves AI risk acceptance for High-Risk systems; escalates unresolvable compliance gaps | All Phase 2 policies, AI system governance documentation |
| **Chief Risk Officer (CRO)** | Enterprise risk register ownership; risk appetite governance; chairs Integration Management Committee; business continuity oversight. *Named: Susan Orwell* | Risk Management Policy, M&A GRC Integration Charter, BC/DR Policy |
| **Data Protection Officer (DPO)** | Privacy programme ownership; GDPR obligations; DPIA governance; data subject request management; AI training data governance | Privacy and Data Protection Policy, AI System Inventory |
| **Chief Technology Officer (CTO)** | AI system technical governance; human oversight mechanism implementation; conformity assessment technical lead; change management for AI systems | AI Governance Policy, Change Management Policy |
| **General Counsel / Legal Counsel** | EU AI Act regulatory advice; GDPR notification obligations; conformity assessment legal review; contract AI governance clauses; serious incident notification to authorities | AI Governance Policy, AI System Inventory, Integration Charter |
| **Information Security Officer (ISO)** | ISMS operational ownership; policy drafting and maintenance; exception approval; day-to-day compliance monitoring. *Named: Susan Orwell* | All Phase 1 and Phase 2 security policies |
| **AI Governance Committee** | AI system risk classification authority; EU AI Act conformity assessment governance; post-market monitoring oversight. Meets quarterly and on emergency basis within 5 business days of significant AI incident | AI Governance Policy, AI System Inventory |
| **Integration Management Committee (IMC)** | M&A integration governance; monthly meetings during integration period; policy hierarchy oversight; inherited risk acceptance authority | M&A GRC Integration Charter, M&A Risk Assessment |
| **Risk Management Committee** | Risk escalation and formal acceptance authority; approves treatment decisions above materiality thresholds; receives budget-blocked risk escalations | Risk Management Policy, Asset Risk Register |
| **AI System Owners** | Per-system lifecycle accountability (PCM-001: VP Customer Success; CRT-001: General Counsel); conformity assessment coordination; post-market monitoring; override log review | AI Governance Policy, AI System Inventory |
| **GRC Team** | AI System Inventory maintenance; compliance reporting; risk assessment coordination; policy rationalization tracking; audit readiness | All GRC programme documents |

---

## Phase 2 Document Index

Status key: ✓ Published | ✓ Complete | ⧖ In Development | ☐ Planned

### Enterprise Policies — Emyzer Nexus

| Policy | Owner | Status | Frameworks |
|---|---|---|---|
| [AI Governance Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/enterprise-policies/ai-governance-policy.md) | CISO | ✓ Published | EU AI Act, NIST AI RMF 1.0, ISO/IEC 42001:2023 |
| [Model Risk Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/enterprise-policies/model-risk-policy.md) | CRO | ✓ Published | SR 11-7, NIST AI RMF, EU AI Act |
| [Privacy and Data Protection Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/enterprise-policies/privacy-and-data-protection-policy.md) | DPO | ✓ Published | GDPR, UK GDPR, ISO 27701:2019 |
| [Security Awareness and Training Policy (Tier 2)](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/enterprise-policies/security-awareness-and-training-policy.md) | CISO | ✓ Published | ISO 27001:2022, NIST SP 800-50, EU AI Act Art.14 |

### AI Governance Programme

| Document | Description | Status |
|---|---|---|
| [AI Governance README](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/ai-governance/readme.md) | Programme overview, document index, frameworks | ✓ Published |
| [AI System Inventory and Classification](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/ai-governance/ai-system-inventory.md) | Formal EU AI Act risk tier classification of PCM-001 and CRT-001; system profiles and governance obligations | ✓ Published |
| [EU AI Act Control Mapping](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/ai-governance/eu-ai-act-mapping.md) | Article-by-article compliance mapping; gap identification and remediation priorities | ✓ Published |
| [AI System Risk Assessments](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/ai-governance/risk-assessments.md) | Risk assessments for PCM-001 and CRT-001 using extended AI-specific methodology | ✓ Published |

### Integration Management Programme

| Document | Description | Status |
|---|---|---|
| [Integration Management README](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/integration-management/readme.md) | Programme purpose, scope, key decisions | ✓ Published |
| [M&A GRC Integration Charter](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/integration-management/m%26a-grc-integration-charter.md) | Post-acquisition policy hierarchy; subsidiary governance; policy review/retirement conditions | ✓ Published |
| [Policy Rationalization Roadmap](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/integration-management/rationalization-roadmap.md) | Phase 1 policy review schedule; conflict identification; gap analysis; Veridian AI remediation priorities | ✓ Published |
| [M&A Risk Assessment](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/integration-management/ma-risk-assessment.md) | Risk register for GRC risks arising from Veridian AI acquisition | ✓ Published |

---

## Relationship to Phase 1 Documentation

All Phase 1 documentation developed for Emyzer Technology remains in effect as subsidiary governance under the policy hierarchy established in the M&A GRC Integration Charter. Phase 1 artifacts are not superseded by Phase 2 unless a formal rationalization decision is made and recorded in the Policy Rationalization Roadmap.

For Phase 1 documentation, see [Emyzer Technology — GRC Programme Overview](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/emyzer-technology/README.md).

---

## Frameworks Referenced

| Framework | Application in Phase 2 |
|---|---|
| **[EU AI Act (Regulation 2024/1689)](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32024R1689)** [VERIFY] | Primary regulatory driver for Phase 2; classification of PCM-001 and CRT-001 as High-Risk; Articles 9–15 conformity obligations; post-market monitoring (Art.72); serious incident reporting (Art.73) |
| **[NIST AI Risk Management Framework (AI RMF 1.0)](https://www.nist.gov/artificial-intelligence/ai-risk-management-framework)** | AI governance programme structure — Govern, Map, Measure, Manage functions applied to AI system lifecycle |
| **[ISO/IEC 42001:2023](https://www.iso.org/standard/81230.html)** | AI management system standard; Clause 8 operational controls; Annex A AI management controls |
| **[ISO 27001:2022](https://www.iso.org/standard/82875.html)** | ISMS continuity; policy hierarchy for expanded scope; A.8.2 access control; A.5.19 supplier relationships |
| **[GDPR (Regulation 2016/679)](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32016R0679)** [VERIFY] | Training data governance (PCM-001); external API data processor obligations (CRT-001); DPIA requirements; Article 28 processor agreements [VERIFY] |
| **[ISO 31000:2018](https://www.iso.org/standard/65694.html)** | Enterprise risk management methodology; M&A risk identification and treatment |
| **[NIST CSF 2.0](https://www.nist.gov/cyberframework)** | Govern (GV) function applied to post-acquisition GRC integration; identification and protection across expanded asset scope |

---

## Related Documentation

| Document | Description |
|---|---|
| [Portfolio Overview](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/README.md) | Top-level narrative, 60-second review path, and skills demonstrated |
| [Emyzer Technology Overview](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/emyzer-technology/README.md) | Phase 1 GRC programme — 10 policies, risk programme, business continuity |
| [CONTRIBUTING.md](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/CONTRIBUTING.md) | How changes are proposed, reviewed, approved, and merged across the portfolio |

---

*All content in this portfolio is a fictional case study developed for professional demonstration purposes. Framework and regulatory references are accurate as of the document publication dates.*

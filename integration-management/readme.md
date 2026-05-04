# Integration Management

**Emyzer Nexus: M&A GRC Integration Programme**

---

> **Simulated Environment**
>
> Emyzer Nexus is a fictional organisation created for this GRC portfolio. All entities, personnel, systems, policies, risk entries, and regulatory scenarios described in this repository are invented for professional demonstration purposes. Framework and regulatory references are accurate as of the document dates; their application to Emyzer Nexus is illustrative only.

---

## Programme Purpose

This folder contains the governance documentation for the GRC integration of Veridian AI into Emyzer Nexus following the Q4 2024 acquisition. The integration programme exists to answer three questions that every M&A transaction creates:

1. **Which policies now govern the acquired entity?** Veridian AI operated informally without a documented GRC programme. From the acquisition close date, Emyzer Nexus policies apply: but the transition must be managed rather than assumed.
2. **What compliance gaps did we inherit?** Veridian AI's two operational AI systems (PCM-001 and CRT-001) were in production without EU AI Act conformity assessments. The GDPR data processing situation for CRT-001's external LLM API was unresolved. These gaps became Emyzer Nexus compliance gaps on acquisition close.
3. **What Phase 1 documentation needs to change?** Emyzer Technology's policies were written for a hardware and services business. Absorbing an AI-native startup expands the scope of nearly every policy and creates entirely new governance domains.

The programme is governed by the Integration Management Committee (IMC), chaired by the CRO, and reports to the CEO quarterly.

---

## Integration Scope

| Domain | Description |
|---|---|
| **AI System Governance** | Formal EU AI Act classification and conformity assessment initiation for PCM-001 and CRT-001; ongoing post-market monitoring establishment |
| **Policy Application** | Application of Emyzer Nexus and Emyzer Technology policies to Veridian AI personnel and systems from acquisition close; gap remediation for domains where ET policies do not address AI-specific obligations |
| **Risk Register Integration** | Identification and registration of risks inherited through the acquisition; integration of Veridian AI asset risks into the enterprise risk register |
| **Data Governance** | Classification of training data (PCM-001) and contract data (CRT-001); resolution of GDPR data processing gaps; DPA execution with LLM API vendor |
| **Vendor Contract Review** | Novation of Veridian AI vendor contracts to Emyzer Nexus; AI-specific due diligence on inherited vendor relationships including the LLM API provider |
| **Personnel Obligations** | Mandatory security awareness and AI governance training for all Veridian AI staff; policy acknowledgement; role-specific obligations for AI system operators |
| **Policy Rationalization** | Scheduled review and update of Phase 1 Emyzer Technology policies to address expanded scope created by Veridian AI's AI-native operations |

---

## Document Index

| Document | Description | Status |
|---|---|---|
| [Integration Management README](readme.md) | Programme purpose, scope, key decisions, and document index | ✓ Published |
| [M&A GRC Integration Charter](m&a-grc-integration-charter.md) | Establishes the post-acquisition policy hierarchy; defines which entity's policies govern; sets conditions triggering policy review or retirement; subsidiary documentation governance | ✓ Published |
| [Policy Rationalization Roadmap](rationalization-roadmap.md) | Scheduled review timeline for all Phase 1 documentation; conflict identification log; gap analysis; Veridian AI documentation remediation priorities | ✓ Published |
| [M&A Risk Assessment](ma-risk-assessment.md) | Risk register for GRC risks arising from the Veridian AI acquisition; covers Technology, Regulatory, Data/Privacy, Personnel, and Operational risk categories | ✓ Published |

---

## Key Governance Decisions

The following decisions were made by the Integration Management Committee and approved by the CEO:

1. **Immediate policy application (Day 0):** All Emyzer Nexus and Emyzer Technology policies apply to Veridian AI personnel from acquisition close date (2024-Q4). Personnel were notified by HR on acquisition close and required to acknowledge policies within 30 days.

2. **AI system classification:** PCM-001 (Predictive Customer Churn Model) and CRT-001 (AI-Assisted Contract Review Tool) were classified as **High-Risk** under the EU AI Act [VERIFY: Annex III applicability] pending formal conformity assessment. Interim human review protocols were implemented for both systems pending conformity completion.

3. **CRT-001 restricted use:** CRT-001 use was restricted to contracts containing no personal data pending execution of a Data Processing Agreement (DPA) with the LLM API vendor. This restriction was implemented immediately on legal advice given the unresolved GDPR Article 28 [VERIFY] position.

4. **Integration Management Committee formed:** A monthly IMC was established comprising the CRO (chair), CISO, CTO, Legal Counsel, and GRC Lead, with authority to make integration governance decisions within the remit of this charter.

5. **External GRC consultant engaged:** Given integration workstream volume, an external GRC consultant was engaged for a 6-month sprint to support risk register integration, policy rationalization, and AI governance documentation.

6. **Phase 1 policies remain in effect:** All Emyzer Technology Phase 1 policies remain in effect as subsidiary documentation under the Emyzer Nexus policy hierarchy. No Phase 1 policy was retired without a formal rationalization decision.

7. **AI Governance Committee convened:** The AI Governance Committee, established under the AI Governance Policy, was convened in January 2025 with its first meeting dedicated to formal classification of PCM-001 and CRT-001.

---

## Frameworks Referenced

| Framework | Application |
|---|---|
| **[ISO 31000:2018](https://www.iso.org/standard/65694.html)** | Enterprise risk management: M&A risk identification and treatment methodology |
| **[ISO 27001:2022](https://www.iso.org/standard/82875.html)** | Information security management: policy hierarchy and scope expansion |
| **[EU AI Act (Regulation 2024/1689)](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32024R1689)** [VERIFY] | AI system classification obligations triggered by acquisition of Veridian AI systems |
| **[GDPR (Regulation 2016/679)](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32016R0679)** [VERIFY] | Data governance obligations for inherited training data and external API data transmission |
| **[NIST CSF 2.0](https://www.nist.gov/cyberframework)** | Govern (GV) function: organisational GRC integration following material organisational change |

---

## Related Documentation

| Document | Link |
|---|---|
| Portfolio Overview | [README.md](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/README.md) |
| Emyzer Nexus Overview | [emyzer-nexus/readme.md](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/emyzer-nexus/readme.md) |
| AI Governance Programme | [ai-governance/readme.md](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/ai-governance/readme.md) |
| Enterprise Policies | [enterprise-policies/readme.md](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/enterprise-policies/readme.md) |
| Phase 1 GRC Programme | [emyzer-technology/README.md](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/emyzer-technology/README.md) |

---

*All content in this portfolio is a fictional case study developed for professional demonstration purposes. Framework and regulatory references are accurate as of the document publication dates.*

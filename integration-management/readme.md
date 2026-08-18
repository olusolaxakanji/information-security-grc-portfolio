# Integration Management Programme

**Emyzer Nexus: M&A GRC Integration | Fictional case study.**

> All entities, systems, personnel, and risk findings are invented for professional demonstration purposes. Framework references are accurate as of the document dates.

---

## The Three Questions Every Acquisition Creates

When Emyzer Technology acquired Veridian AI in Q4 2024, the GRC team faced the same three questions that arise in every M&A transaction:

**1. Which policies govern the acquired entity, and from when?**
Veridian operated informally without a documented GRC programme. The acquisition could not wait for new policies to be written. Emyzer Nexus policies had to apply from Day 0, but that transition required formal documentation to be enforceable rather than assumed.

**2. What compliance gaps were inherited?**
Veridian's two AI systems (PCM-001 and CRT-001) were in production without EU AI Act conformity assessments. CRT-001's external LLM API had an unresolved GDPR data processor position. These became Emyzer Nexus compliance gaps on acquisition close, not at some future point when governance caught up.

**3. What existing documentation needs to change?**
Emyzer Technology's Phase 1 policies were written for a hardware and services business. Absorbing an AI-native startup expanded the scope of nearly every existing policy and created governance domains Phase 1 had not addressed. Every policy required a scheduled review, and some required immediate amendment.

This programme answers all three.

---

## Key Governance Decisions

The Integration Management Committee (IMC), chaired by the CRO and approved by the CEO, made seven binding decisions at acquisition close. These are documented in the Integration Charter and govern how the programme operates.

1. **Day 0 policy application.** All Emyzer Nexus and Emyzer Technology policies apply to Veridian AI personnel from acquisition close. Personnel acknowledged policies within 30 days.
2. **AI system classification.** PCM-001 and CRT-001 were classified as High-Risk pending formal conformity assessment. Interim human review protocols were implemented immediately.
3. **CRT-001 restricted use.** CRT-001 was restricted to contracts containing no personal data pending DPA execution with the LLM API vendor.
4. **IMC formation.** A monthly committee of CRO (chair), CISO, CTO, Legal Counsel, and GRC Lead was established with authority to make integration governance decisions within the charter's remit.
5. **External GRC consultant engaged.** An external consultant was engaged for a 6-month sprint given integration workstream volume.
6. **Phase 1 policies remain in effect.** No Phase 1 policy was retired without a formal rationalization decision recorded in the Roadmap.
7. **AI Governance Committee convened.** The AI Governance Committee first met in January 2025. Its opening session was dedicated to formal classification of PCM-001 and CRT-001.

---

## What This Programme Produced

| Document | What it resolves |
|---|---|
| [M&A GRC Integration Charter](ma-grc-integration-charter.md) | Which policies govern Veridian from Day 0. Which governance body has authority to accept inherited risk. What conditions trigger a policy review or retirement. A 15-entry integration risk register with owners and target resolution dates. |
| [Policy Rationalization Roadmap](rationalization-roadmap.md) | Phase 1 policies were written for Emyzer Technology as a standalone entity. This document schedules their review under the expanded Nexus scope, identifies conflicts, and prioritizes remediation. Without this document, Phase 1 policies remain in force indefinitely without a deliberate decision to keep or retire them. |
| [M&A Risk Assessment](ma-risk-assessment.md) | Formal risk register for GRC risks introduced by the acquisition across five categories: Technology, Regulatory, Data/Privacy, Personnel, and Operational. 15 risks with owners, inherent ratings, current controls, residual ratings, and target resolution dates. |

---

## Integration Scope

| Domain | What was required |
|---|---|
| AI System Governance | Formal EU AI Act classification and conformity assessment initiation for PCM-001 and CRT-001; post-market monitoring establishment |
| Policy Application | Application of Emyzer Nexus and Emyzer Technology policies to Veridian personnel from acquisition close; gap remediation for AI-specific domains Phase 1 did not cover |
| Risk Register Integration | Identification and registration of inherited risks; integration of Veridian asset risks into the enterprise register |
| Data Governance | Classification of training data (PCM-001) and contract data (CRT-001); resolution of GDPR data processing gaps; DPA execution with LLM API vendor |
| Vendor Contract Review | Novation of Veridian vendor contracts to Emyzer Nexus; AI-specific due diligence on inherited vendor relationships |
| Personnel Obligations | Mandatory security awareness and AI governance training for all Veridian staff; policy acknowledgement; role-specific obligations for AI system operators |
| Policy Rationalization | Scheduled review of all Phase 1 Emyzer Technology policies to address scope expansion created by Veridian's AI-native operations |

---

## Frameworks Applied

| Framework | Application |
|---|---|
| ISO 31000:2018 | M&A risk identification and treatment methodology |
| ISO 27001:2022 | Policy hierarchy and scope expansion governance |
| EU AI Act (Regulation 2024/1689) [VERIFY] | AI system classification obligations triggered by acquisition |
| GDPR (Regulation 2016/679) [VERIFY] | Data governance obligations for inherited training data and external API data transmission |
| NIST CSF 2.0 | Govern (GV) function applied to post-acquisition GRC integration |

---

## Related Documentation

| Document | Description |
|---|---|
| [Portfolio Overview](../README.md) | Top-level narrative and 60-second review path |
| [Emyzer Nexus Overview](../emyzer-nexus/readme.md) | Phase 2 programme context |
| [AI Governance Programme](../ai-governance/readme.md) | AI programme detail: system inventory, EU AI Act mapping, risk assessments |
| [Enterprise Policies](../enterprise-policies/readme.md) | Phase 2 policy architecture and design decisions |
| [Emyzer Technology Overview](../emyzer-technology/README.md) | Phase 1 foundation programme |

---

*All content in this portfolio is a fictional case study. Framework and regulatory references are accurate as of the document publication dates.*

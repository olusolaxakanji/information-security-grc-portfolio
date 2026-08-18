# M&A GRC Integration Charter

**Emyzer Nexus: Integration Management Programme**

---

## Document Metadata

| Attribute | Value |
|---|---|
| **Document ID** | INT-CHR-001 |
| **Document Type** | Charter |
| **Version** | 1.0 |
| **Effective Date** | 2025-01-15 |
| **Valid To** | 2026-01-15 (renewable annually) |
| **Owner** | Chief Risk Officer |
| **Approver** | Chief Executive Officer |
| **Reviewers** | CISO; Legal Counsel; GRC Team |
| **State** | Published |
| **Governing Framework** | ISO 31000:2018; NIST CSF 2.0 Govern function; ISO 27001:2022 |
| **Published Document** | INT-CHR-001 |

---

## Description

This charter establishes the governance framework for the GRC integration of Veridian AI into Emyzer Nexus following the Q4 2024 acquisition. It defines the post-acquisition policy hierarchy, the governance bodies responsible for integration oversight, the workstreams governing the transition, and the conditions that trigger policy review or retirement.

**Impact:** Provides the legal and governance basis for applying Emyzer Nexus policies to Veridian AI personnel and systems from acquisition close. Prevents compliance gaps from forming at the entity boundary. Establishes accountability for each integration workstream and the escalation path when integration decisions require executive resolution.

---

## A. Purpose

To establish a comprehensive, documented governance framework for the GRC integration of Veridian AI into Emyzer Nexus, ensuring that:

1. All Veridian AI personnel, systems, and operations are subject to appropriate governance from acquisition close
2. The post-acquisition policy hierarchy is clearly defined and consistently applied
3. Compliance gaps inherited through the acquisition, particularly those arising from Veridian AI's AI systems and their obligations under the EU AI Act, are identified, prioritised, and remediated on a structured timeline
4. Phase 1 Emyzer Technology documentation remains in effect as subsidiary governance and is not inadvertently superseded by Phase 2 activity
5. Integration governance decisions are made by the appropriate authority, documented, and traceable

This charter is the authoritative document for integration governance. It does not supersede the [AI Governance Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/enterprise-policies/ai-governance-policy.md), [Risk Management Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/risk-management-policy.md), or any other Emyzer Nexus policy: it operates alongside those policies to manage the transition period.

---

## B. Scope

This charter covers all GRC-relevant activities arising from the integration of Veridian AI into Emyzer Nexus:

| In Scope | Description |
|---|---|
| Policy application | Application of Emyzer Nexus and Emyzer Technology policies to Veridian AI personnel and systems |
| AI system governance | EU AI Act classification and conformity assessment for inherited AI systems PCM-001 and CRT-001 |
| Risk register integration | Identification and registration of risks inherited through the acquisition |
| Data governance | Classification of training data (PCM-001) and contract data (CRT-001); GDPR compliance for inherited data processing |
| Vendor contract management | Novation of Veridian AI vendor contracts; AI-specific due diligence on inherited vendors |
| Personnel obligations | Security awareness and AI governance training; policy acknowledgement; role-specific requirements for AI operators |
| Policy rationalization | Scheduled review and update of Phase 1 Emyzer Technology policies where Veridian AI's operations expand their scope |

| Out of Scope | Description |
|---|---|
| Technical integration | System and infrastructure integration is governed by a separate technical integration project |
| Commercial integration | Financial reporting consolidation, pricing, and commercial terms are managed by Finance |
| HR integration | Employment contracts, benefits harmonisation, and organisational design are managed by HR, with GRC team support for policy-specific obligations only |

---

## C. Organisational Hierarchy

The post-acquisition corporate structure is:

```
Emyzer Nexus  (parent: Phase 2 GRC programme)
├── Emyzer Technology  (subsidiary: Phase 1 GRC programme in effect)
└── Veridian AI  (acquired entity: governance integration in progress)
```

**Emyzer Nexus** holds governance authority over both subsidiaries. All Emyzer Nexus enterprise policies (AI Governance Policy, Model Risk Policy, Privacy and Data Protection Policy, Security Awareness and Training Policy Tier 2) take precedence.

**Emyzer Technology** operates under its established Phase 1 GRC programme, which remains in effect as subsidiary documentation. Phase 1 policies apply across Emyzer Technology and, where relevant, extend to Veridian AI as the applicable Emyzer Nexus group standard where no Phase 2 policy yet governs that domain.

**Veridian AI** is subject to Emyzer Nexus group policies from the acquisition close date. Veridian AI did not operate a formal GRC programme; where legacy Veridian AI documentation existed, it is superseded by Emyzer Nexus and Emyzer Technology policies from the effective date of this charter (2025-01-15).

---

## D. Policy Hierarchy

### D.1 Hierarchy Principles

1. Emyzer Nexus enterprise policies take precedence over all subsidiary documentation
2. Where Emyzer Nexus has not issued a policy in a given domain, the applicable Emyzer Technology Phase 1 policy governs
3. Veridian AI legacy documentation is superseded by Emyzer Nexus / Emyzer Technology policies upon integration date (2025-01-15)
4. Phase 1 Emyzer Technology policies remain in effect as subsidiary documentation unless formally retired through the Policy Rationalization Roadmap process

### D.2 Policy Domain Hierarchy Table

| Policy Domain | Phase 2 Governing Document | Phase 1 Applicable Document | Effective for Veridian AI | Notes |
|---|---|---|---|---|
| AI Governance | [AI Governance Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/enterprise-policies/ai-governance-policy.md) | N/A (Phase 2 only) | 2025-01-15 | No Phase 1 equivalent; new domain |
| Model Risk | [Model Risk Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/enterprise-policies/model-risk-policy.md) | N/A (Phase 2 only) | 2025-01-15 | New domain |
| Privacy / Data Protection | [Privacy and Data Protection Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/enterprise-policies/privacy-and-data-protection-policy.md) | [Data Classification Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/data-classification-policy.md) (partial) | 2025-01-15 | Phase 2 policy extends GDPR obligations |
| Information Security | — | [Information Security Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/information-security-policy.md) | 2025-01-15 | Phase 1 governs until Phase 2 updates scope |
| Access Control | — | [Access Control Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/access-control-policy.md) | 2025-01-15 | Phase 1 applies; Veridian AI IAM gap identified |
| Incident Management | — | [Incident Management Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/incident-management-policy.md) | 2025-01-15 | Phase 1 applies; AI incident extensions from AI Governance Policy |
| Risk Management | — | [Risk Management Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/risk-management-policy.md) | 2025-01-15 | Phase 1 methodology extended for AI-specific risks |
| Business Continuity | — | [BC/DR Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/bcdr-policy.md) | 2025-01-15 | Phase 1 applies; BCP extended to cover AI system outage scenarios |
| Change Management | — | [Change Management and Configuration Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/change-management-and-configuration-policy.md) | 2025-01-15 | Gap: AI model retraining not covered; extension required |
| Acceptable Use | — | [Acceptable Use Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/acceptable-use-policy.md) | 2025-01-15 | AI tool use provisions not addressed; update required |
| Data Classification | — | [Data Classification Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/data-classification-policy.md) | 2025-01-15 | Critical gap: training data and model outputs unclassified |
| Third-Party Risk | — | [Third-Party Risk Management Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/third-party-risk-management-policy.md) | 2025-01-15 | AI vendor due diligence addendum required immediately |
| Security Awareness / Training | [Security Awareness and Training Policy (Tier 2)](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/enterprise-policies/security-awareness-and-training-policy.md) | [Security Awareness and Training Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/security-awareness-and-training-policy.md) | 2025-01-15 | Tier 2 adds AI governance and operator-specific training |

---

## E. Governance Bodies

### E.1 Integration Management Committee (IMC)

**Chair:** Chief Risk Officer (Susan Orwell)  
**Members:** CISO; CTO; Legal Counsel; GRC Lead  
**Cadence:** Monthly during the integration period (2025-01-15 to 2026-01-15); quarterly thereafter until charter renewal  
**Authority:** Make integration governance decisions within this charter's remit; escalate decisions beyond charter remit to the CEO; approve integration workstream closures; accept integration risks within CRO delegated authority

### E.2 AI Governance Committee

**Chair:** CISO  
**Members:** CRO; Legal Counsel; CTO; AI System Owners  
**Cadence:** Quarterly; emergency within 5 business days of significant AI incident  
**Authority:** AI system risk classification; conformity assessment approval; EU AI Act compliance decisions; AI risk acceptance within CISO delegated authority

### E.3 Risk Management Committee

**Authority:** Risk escalation for integration risks above materiality thresholds; formal acceptance of inherited risks that cannot be remediated within standard treatment timelines

### E.4 Legal Counsel

**Authority:** Regulatory notification obligations; contract novation; GDPR DPA execution; EU AI Act implementing act interpretation [VERIFY]

---

## F. Integration Workstreams

| Workstream | Description | Lead | Target Completion | Status |
|---|---|---|---|---|
| W1: Policy application | Issue policy acknowledgement notices to all Veridian AI staff; collect signed acknowledgements; resolve policy queries | ISO (Susan Orwell) | 2025-03-31 | Complete |
| W2: AI system governance | Complete EU AI Act classification; initiate conformity assessments for PCM-001 and CRT-001; establish post-market monitoring | CISO / AI Governance Committee | 2025-12-31 | In Progress |
| W3: Risk register integration | Identify and register all GRC risks inherited from Veridian AI; integrate into enterprise risk register | CRO / GRC Team | 2025-03-31 | Complete |
| W4: Data governance | Complete DPO audit of PCM-001 training data; execute DPA with LLM API vendor; classify all Veridian AI data assets | DPO | 2025-09-30 | In Progress |
| W5: Vendor contract management | Novate all Veridian AI vendor contracts to Emyzer Nexus; complete AI-specific due diligence on LLM API vendor | Vendor Risk Manager / Legal Counsel | 2025-06-30 | In Progress |
| W6: Personnel obligations | Complete security awareness training and AI governance training for all Veridian AI staff; complete AI operator training for PCM-001 and CRT-001 operators | HR / GRC Team | 2025-03-31 | Complete |
| W7: Policy rationalization | Complete review of Phase 1 policies against expanded Veridian AI scope; update or extend policies where gaps identified | GRC Team | 2025-12-31 | In Progress |
| W8: Shadow AI discovery | Conduct discovery exercise to identify any AI systems developed or used by Veridian AI beyond PCM-001 and CRT-001 | CTO / GRC Team | 2025-06-30 | Complete: no additional systems identified |

---

## G. Policy Application Timeline

| Policy | Applies to Veridian AI From | Compliance Mode | Notes |
|---|---|---|---|
| All Emyzer Nexus enterprise policies | Day 0 (2025-01-15) | Immediate | Distributed on acquisition close; acknowledgement required within 30 days |
| All Emyzer Technology Phase 1 policies | Day 0 (2025-01-15) | Immediate | Full application from integration date |
| AI Governance Policy: conformity assessment | 2025-06-01 | Phased | Conformity assessment initiation deferred 6 months to allow documentation sprint |
| Change Management Policy: AI model retraining | 2025-03-31 | Phased | AI retraining brought under CAB process from Q1 2025; CAB briefed on technical requirements |
| Third-Party Risk Management: AI vendor due diligence | 2025-03-31 | Phased | AI vendor assessments initiated Q1 2025 |

---

## H. Conditions Triggering Policy Review or Retirement

The following conditions trigger a formal review of applicable policies under this charter, managed through the Policy Rationalization Roadmap:

1. **Material change to EU AI Act implementing acts**: any published implementing act or delegated regulation that affects the classification or obligations of PCM-001 or CRT-001 triggers immediate review of the AI Governance Policy and this charter [VERIFY: monitor EU AI Office publications]
2. **Integration of additional acquired entities**: any further acquisition by Emyzer Nexus triggers a new integration charter; existing charter updated to reflect expanded scope
3. **Material change to AI system architecture**: significant change to PCM-001 or CRT-001 (new model type, new use case, new data source) triggers reclassification and policy review
4. **Regulatory investigation or enforcement action**: any regulatory contact regarding EU AI Act or GDPR compliance triggers immediate IMC convening and policy review
5. **Phase 1 policy conflicts identified**: if the Policy Rationalization Roadmap identifies a material conflict between a Phase 1 policy and Veridian AI's operational model, the relevant Phase 1 policy is added to the rationalization queue with priority determined by risk level
6. **Significant AI-related incident**: any High or Critical AI incident triggers review of the AI Governance Policy, applicable risk assessments, and this charter
7. **Completion of conformity assessments**: when PCM-001 or CRT-001 conformity assessments are complete, this charter is reviewed to confirm integration workstream W2 closure conditions are met
8. **Charter renewal**: annual review at Valid To date (2026-01-15); charter renewed or replaced by IMC with CEO approval

---

## I. Legacy Documentation Governance

Veridian AI did not maintain a formal GRC programme. Where informal documentation existed (standard operating procedures, vendor agreements, engineering documentation), the following applies:

- **Vendor agreements**: novated to Emyzer Nexus per Workstream W5; AI-specific terms reviewed and supplemented with Emyzer Nexus requirements
- **Engineering documentation**: transferred to Emyzer Nexus document repository; forms the basis of technical documentation development for Article 11 [VERIFY] compliance
- **Informal SOPs**: superseded by applicable Emyzer Technology Phase 1 and Emyzer Nexus Phase 2 policies; staff retrained accordingly
- **Historical data and records**: retained in Veridian AI archive under applicable retention schedules; DPO to assess against GDPR retention obligations

---

## J. Subsidiary Documentation Governance

Phase 1 Emyzer Technology documentation remains in effect as subsidiary governance under this charter with the following rules:

1. Phase 1 policies are not retired without a formal rationalization decision recorded in the [Policy Rationalization Roadmap](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/integration-management/rationalization-roadmap.md)
2. Where a Phase 2 Emyzer Nexus policy covers the same domain as a Phase 1 policy, the Phase 2 policy takes precedence; the Phase 1 policy remains as subsidiary guidance unless the Phase 2 policy explicitly retires it
3. Phase 1 policies subject to rationalization review retain their current status until a replacement or update is formally approved
4. The GRC Team maintains a current version of all Phase 1 documentation and ensures currency with Phase 2 policy hierarchy

---

## K. Related Policies

1. [**Information Security Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/information-security-policy.md): parent ISMS framework; provides the governance structure this charter operates within
2. [**AI Governance Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/enterprise-policies/ai-governance-policy.md): governs AI system lifecycle; defines AI Governance Committee authority; specifies EU AI Act compliance programme
3. [**Risk Management Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/risk-management-policy.md): methodology applied in M&A Risk Assessment; Risk Management Committee authority referenced
4. [**Third-Party Risk Management Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/third-party-risk-management-policy.md): vendor contract novation and AI vendor due diligence requirements
5. [**Privacy and Data Protection Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/enterprise-policies/privacy-and-data-protection-policy.md): GDPR obligations for inherited data processing

---

## L. Framework Alignment

| Framework | Applicable Elements |
|---|---|
| **ISO 31000:2018** | Risk identification and treatment across integration workstreams; inherited risk assessment methodology |
| **ISO 27001:2022 Cl.4.3** [VERIFY] | Determining the scope of the ISMS: expansion to cover acquired entity |
| **ISO 27001:2022 Cl.6.1** [VERIFY] | Risk and opportunity management: integration risks as organisational context change |
| **NIST CSF 2.0: Govern (GV)** [VERIFY] | Organisational governance for managing cybersecurity risk through material organisational change |
| **EU AI Act (Regulation 2024/1689)** [VERIFY] | Article 9 risk management obligation; integration charter establishes governance for conformity compliance |
| **GDPR (Regulation 2016/679)** [VERIFY] | Article 28 processor obligations; Article 5 data governance requirements applying to inherited data assets |

---

## M. Evidence of Compliance

### Evidence Index

| Evidence Type | System of Record | Owner | Retention Period |
|---|---|---|---|
| Integration Management Committee meeting minutes | Document Repository | CRO | 7 years |
| Policy acknowledgement records (Veridian AI staff) | HR System / GRC Platform | Human Resources | Employment + 3 years |
| Workstream completion records | GRC Platform | GRC Team | 7 years |
| Policy application notices | Document Repository | ISO | 7 years |
| AI Governance Committee classification decisions | GRC Platform | AI Governance Committee | Life of system + 7 years |
| Risk register integration records | GRC Platform | GRC Team | 7 years |
| Vendor contract novation records | Legal Repository | Legal Counsel | Contract + 7 years |
| Charter renewal decisions | Document Repository | CRO | 7 years |

---

## Approval History

| Date | Approver | Status | Comments |
|---|---|---|---|
| 2025-01-15 | Chief Executive Officer | Approved | "The acquisition of Veridian AI is a significant governance event. This charter provides the structure we need to manage the transition without creating compliance gaps. The policy hierarchy is clear and the workstream accountability is appropriate. Approved." |

---

## Document Control

- **Document ID:** INT-CHR-001
- **Version:** 1.0
- **Classification:** Internal Use
- **Last Updated:** 2025-01-15
- **Next Review Date:** 2026-01-15

---

*This document was developed as part of the Emyzer Nexus Phase 2 GRC programme and formatted for portfolio presentation.*

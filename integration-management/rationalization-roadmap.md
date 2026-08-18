# Policy Rationalization Roadmap

**Emyzer Nexus: Integration Management Programme**

---

## Document Information

| Attribute | Value |
|---|---|
| **Document ID** | INT-RR-001 |
| **Document Type** | Rationalization Planning Document |
| **Version** | 1.1 |
| **Effective Date** | 2025-02-01 |
| **Last Updated** | 2025-07-01 |
| **Owner** | GRC Team / Chief Risk Officer |
| **Classification** | Internal Use |
| **Governing Document** | [M&A GRC Integration Charter](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/integration-management/ma-grc-integration-charter.md) |

---

## 1. Purpose

This roadmap governs the scheduled review and update of all Phase 1 Emyzer Technology policies in light of the scope expansion created by the Veridian AI acquisition. It documents:

- The review schedule and priority for each Phase 1 policy
- Conflicts identified between existing policies and Veridian AI's operational model
- Domains where no existing policy addresses new obligations
- The status of each remediation item
- Update prioritisation criteria

This is a living document, updated at each Integration Management Committee meeting. It does not authorise policy changes: all policy updates require the approval process defined in the relevant policy's document control section.

---

## 2. Rationalization Methodology

Each Phase 1 policy was assessed across three dimensions:

### 2.1 Scope Expansion Check
Does Veridian AI's operational profile, specifically its AI-native operations, external LLM API usage, and B2B SaaS client base, create obligations not addressed in the current policy? If yes, the policy requires extension or update.

### 2.2 Conflict Check
Does Veridian AI's existing practice conflict with any requirement in the current policy? If yes, the conflict must be resolved by either remediating the Veridian AI practice (standard approach) or, where the policy was written for a scope that did not contemplate AI operations, updating the policy to address the new context.

### 2.3 Gap Check
Are there governance domains where neither an Emyzer Technology Phase 1 policy nor an Emyzer Nexus Phase 2 policy addresses an obligation created by the Veridian AI acquisition? If yes, this is a domain gap requiring new documentation.

### 2.4 Update Prioritisation Criteria

Policies are prioritised for rationalization using the following criteria:

| Criterion | Weight | Description |
|---|---|---|
| Regulatory risk | 40% | Likelihood and severity of regulatory enforcement if the gap is not addressed |
| Data sensitivity | 25% | Whether the gap involves personal data or confidential commercial data |
| Operational impact | 20% | Whether the gap creates current operational compliance failures (vs. future risk) |
| Implementation timeline | 15% | How quickly the remediation can realistically be delivered |

---

## 3. Phase 1 Policy Review Schedule

| Policy | Current Version | Rationalization Priority | Review Trigger | Target Review Date | Review Status | Outcome / Notes |
|---|---|---|---|---|---|---|
| [Information Security Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/information-security-policy.md) | 1.0 | **Medium** | 12-month scheduled review; AI system scope expansion | 2025-12-31 | Scheduled | Add reference to AI system governance obligations; update ISMS scope to include Veridian AI operations |
| [Access Control Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/access-control-policy.md) | 1.0 | **High** | Veridian AI had no formal IAM programme: immediate coverage gap | 2025-06-30 | **In Review** | Extend to explicitly cover AI system access; add AI operator access requirements; Veridian AI IAM remediation in progress |
| [Incident Management Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/incident-management-policy.md) | 1.0 | **High** | EU AI Act Article 73 [VERIFY] incident reporting obligations not addressed | 2025-09-30 | Scheduled | Add AI incident classification tier; incorporate EU AI Act Article 73 [VERIFY] notification requirements as policy obligation |
| [Risk Management Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/risk-management-policy.md) | 1.0 | **Medium** | AI-specific risk categories not in Phase 1 methodology | 2025-12-31 | Scheduled | Extend methodology to formally include AI risk categories; reference AI System Risk Assessments as a document type |
| [BC/DR Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/bcdr-policy.md) | 1.0 | **Low** | No material conflict; AI system outage scenarios not explicitly addressed | 2025-12-31 | Scheduled | Minor update: add AI system availability to BCP scope; reference AI system outage scenarios in BCP |
| [Change Management and Configuration Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/change-management-and-configuration-policy.md) | 1.0 | **High** | AI model retraining constitutes a material change; not covered by Phase 1 policy: operational gap exists today | 2025-06-30 | **In Review** | Add AI model retraining as a change type requiring CAB review; define criteria for "material change" to AI system; CAB process extended as interim measure pending policy update |
| [Acceptable Use Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/acceptable-use-policy.md) | 1.0 | **Medium** | Staff use of AI tools (including consumer AI) not addressed | 2025-09-30 | Scheduled | Add AI tool acceptable use provisions: approved AI tools register; prohibition on inputting confidential data into unapproved consumer AI tools |
| [Data Classification Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/data-classification-policy.md) | 1.0 | **Critical** | Training data and model outputs have no classification in Phase 1 scheme; immediate GDPR and EU AI Act [VERIFY] compliance gap | 2025-06-30 | **In Review** | Add new data classification categories for: AI training data, AI model artefacts, AI model outputs; apply retention and handling requirements |
| [Third-Party Risk Management Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/third-party-risk-management-policy.md) | 1.0 | **Critical** | AI vendor due diligence requirements not in Phase 1 policy; LLM API vendor without adequate controls | 2025-06-30 | **In Review** | AI Vendor Risk Due Diligence Addendum being developed; standard TPRM policy to be updated to reference addendum; immediate due diligence applied manually in interim |
| [Security Awareness and Training Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/security-awareness-and-training-policy.md) | 1.0 | **High** | AI governance training and High-Risk AI system operator training not in Phase 1 scope | 2025-03-31 | **Complete** | Superseded for Phase 2 AI training obligations by [Security Awareness and Training Policy Tier 2](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/enterprise-policies/security-awareness-and-training-policy.md); Phase 1 policy retained as subsidiary for Emyzer Technology general staff training |

---

## 4. Conflict Identification Log

The following conflicts were identified between existing policies / practices and Veridian AI's pre-acquisition operational model.

| Conflict ID | Policy | Nature of Conflict | Veridian AI Practice | Required Resolution | Priority | Status |
|---|---|---|---|---|---|---|
| CONF-001 | [Security Awareness and Training Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/security-awareness-and-training-policy.md) | Veridian AI employees had received no annual security awareness training | No formal training programme existed | Onboarding training completed for all 212 Veridian AI staff by 2025-03-31; ongoing training governed by Tier 2 policy | **Critical** | **Resolved: 2025-03-31** |
| CONF-002 | [Data Classification Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/data-classification-policy.md) + GDPR Art.28 [VERIFY] | CRT-001 was transmitting personal data to an external LLM API without a DPA | Standard vendor practice treated external API as a software tool, not a data processor | Use restriction implemented immediately; DPA negotiation in progress; target execution 2025-09-30 | **Critical** | In Progress: use restriction in effect |
| CONF-003 | [Change Management and Configuration Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/change-management-and-configuration-policy.md) | AI model retraining cycles were not governed as changes | PCM-001 was retrained quarterly on an engineering team schedule with no change approval | AI model retraining brought under CAB process from 2025-02-01 as interim measure; policy update in progress | **High** | In Progress: interim control in place |
| CONF-004 | [Third-Party Risk Management Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/third-party-risk-management-policy.md) | LLM API vendor had not been assessed under the TPRM programme | Vendor relationship was a technical dependency without security or governance assessment | AI-specific vendor due diligence initiated (SR-2025-001); approved with conditions | **Critical** | In Progress |
| CONF-005 | [Access Control Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/access-control-policy.md) | Veridian AI had no formal access review programme for its systems | System access managed informally by engineering leads; no quarterly review | Access Control Policy applied from 2025-01-15; quarterly review for PCM-001 and CRT-001 initiated; IAM remediation in progress | **High** | In Progress |
| CONF-006 | [Acceptable Use Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/acceptable-use-policy.md) | Veridian AI staff were using unapproved consumer AI tools for work tasks | Several engineers were using public ChatGPT for code assistance, potentially exposing confidential code | Interim guidance issued; approved AI tools register in development; AUP update pending | **Medium** | In Progress: interim guidance issued 2025-02-15 |

---

## 5. Domain Gap Analysis

Domains where no Phase 1 or Phase 2 policy fully addresses obligations created by the Veridian AI acquisition:

| Domain | Gap Description | Resolution | Owner | Target Date | Status |
|---|---|---|---|---|---|
| AI governance operational procedures | The AI Governance Policy establishes the framework; no detailed operational procedures exist for conformity assessment process, bias testing protocol, or AI system retirement | AI Governance Procedures Manual to be developed as Phase 2 operational document | CISO / GRC Team | 2025-12-31 | Planned |
| AI incident response runbook | Incident Management Policy extended for AI incidents in principle; no detailed runbook covering AI-specific failure modes, LLM hallucination incidents, or regulatory notification procedures | AI Incident Response Runbook to be developed | CISO / ISO | 2025-09-30 | In Progress |
| AI vendor due diligence addendum | Standard TPRM does not address AI-specific vendor obligations (model transparency, bias audit availability, LLM API governance) | AI Vendor Risk Due Diligence Addendum in development | Vendor Risk Manager / GRC Team | 2025-06-30 | In Progress |
| Training data lifecycle management | No policy governs the full lifecycle of ML training data: collection, retention, access, deletion, and consent documentation | Will be addressed in Data Classification Policy update plus new AI training data handling procedure | DPO | 2025-09-30 | Planned |

---

## 6. Veridian AI Documentation Remediation Priorities

The following items represent the specific remediation actions required to bring Veridian AI's operations into compliance with Emyzer Nexus governance requirements.

| Priority | Remediation Item | Description | Owner | Target Date | Status |
|---|---|---|---|---|---|
| P1 | DPA with LLM API vendor | Execute GDPR Article 28 [VERIFY] compliant DPA covering CRT-001 data processing; unblock full CRT-001 use | Legal Counsel | 2025-09-30 | In Progress |
| P1 | PCM-001 technical documentation | Complete Annex IV [VERIFY] technical documentation for PCM-001; required for conformity assessment and regulatory examination | VP Customer Success / CTO | 2025-09-30 | In Progress |
| P1 | PCM-001 and CRT-001 conformity assessments | Complete EU AI Act Article 9 [VERIFY] conformity assessments for both systems | AI Governance Committee | 2025-12-31 | In Progress |
| P1 | Training data audit: PCM-001 | DPO-led audit of training data provenance, legal basis, retention, and access controls | DPO | 2025-09-30 | In Progress |
| P2 | CRT-001 technical documentation | Obtain whatever technical documentation is available from LLM API vendor; document residual gap | General Counsel / Legal Counsel | 2025-12-31 | In Progress |
| P2 | Data classification for AI assets | Apply Data Classification Policy extended categories to PCM-001 training data, model artefacts, and CRT-001 contract processing data | DPO / GRC Team | 2025-06-30 | In Progress |
| P2 | AI model retraining change management | Formally document PCM-001 retraining as a change type requiring CAB approval; complete policy update | GRC Team / CTO | 2025-06-30 | In Progress |
| P3 | Acceptable use AI provisions | Update AUP to address approved AI tools register and prohibit unapproved consumer AI tool use for work tasks | ISO | 2025-09-30 | Planned |
| P3 | AI incident response runbook | Develop detailed runbook for AI-specific incidents including LLM failures, model drift detection, and EU AI Act Article 73 [VERIFY] notifications | CISO / ISO | 2025-09-30 | In Progress |
| P3 | Bias testing protocol | Develop formal bias testing protocol for PCM-001 quarterly bias audit; apply to CRT-001 via output quality sampling | AI Governance Committee | 2025-09-30 | Planned |

---

## 7. Update Prioritisation Criteria Applied

Rationalization priority was assigned using the criteria in Section 2.4. The resulting priority distribution is:

| Priority | Policies | Rationale |
|---|---|---|
| **Critical** | Data Classification Policy; Third-Party Risk Management Policy | Current compliance failures (GDPR exposure from CRT-001 data transmission; unclassified training data); regulatory enforcement risk |
| **High** | Access Control Policy; Change Management Policy; Incident Management Policy; Security Awareness and Training Policy | Operational gaps with regulatory and security risk; near-term remediation required |
| **Medium** | Information Security Policy; Risk Management Policy; Acceptable Use Policy | Scope expansion required but no current compliance failure; 12-month review horizon appropriate |
| **Low** | BC/DR Policy | No material conflict; minor scope extension only |

---

## 8. Document Control

| Version | Date | Author | Changes |
|---|---|---|---|
| 1.0 | 2025-02-01 | GRC Team | Initial publication |
| 1.1 | 2025-07-01 | GRC Team | Updated status for CONF-001 (resolved), W6 (complete); added P3 remediation items; reflected shadow AI discovery closure |

- **Document ID:** INT-RR-001
- **Classification:** Internal Use
- **Next Review:** IMC monthly review; formal version update quarterly

---

*This document was developed as part of the Emyzer Nexus Phase 2 GRC programme and formatted for portfolio presentation.*

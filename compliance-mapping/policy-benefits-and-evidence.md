# Policy Benefits and Compliance Evidence Mapping

**Emyzer Technology / Emyzer Nexus – GRC Programme**

---

## Document Metadata

| Attribute | Details |
|-----------|---------|
| **Document Title** | Policy Benefits and Compliance Evidence Mapping |
| **Document ID** | COMP-MAP-001 |
| **Version** | 2.0 |
| **Phase 1 Policies Effective** | 2024-07-01 (Emyzer Technology) |
| **Phase 2 Policies Added** | 2025-07-01 (Emyzer Nexus) |
| **Classification** | Internal |
| **Owner** | GRC Team |
| **Approved By** | Chief Information Security Officer |
| **Review Date** | 2026-07-01 |
| **Framework Alignment** | [ISO 27001:2022](https://www.iso.org/standard/82875.html), [ISO 22301:2019](https://www.iso.org/standard/75106.html), [ISO 31000:2018](https://www.iso.org/standard/65694.html), [EU AI Act (Regulation 2024/1689)](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32024R1689) [VERIFY], [NIST CSF 2.0](https://www.nist.gov/cyberframework), [NIST AI RMF 1.0](https://www.nist.gov/artificial-intelligence/ai-risk-management-framework), [GDPR (Regulation 2016/679)](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32016R0679), ITIL 4 |

---

## Table of Contents

1. [Purpose](#1-purpose)
2. [How to Use This Document](#2-how-to-use-this-document)
3. [Phase 1 Policy Mappings — Emyzer Technology](#3-phase-1-policy-mappings--emyzer-technology)
4. [Phase 2 Policy Mappings — Emyzer Nexus](#4-phase-2-policy-mappings--emyzer-nexus)
5. [Compliance Evidence Summary Matrix](#5-compliance-evidence-summary-matrix)
6. [Audit Readiness Notes](#6-audit-readiness-notes)
7. [Framework Coverage Summary](#7-framework-coverage-summary)
8. [Document Control](#8-document-control)

---

## 1. Purpose

This document maps each policy in the Emyzer Technology and Emyzer Nexus GRC programme to three dimensions of governance value:

1. **Organisational Benefits** — the concrete business, legal, and operational value delivered by the policy's implementation and enforcement.
2. **Compliance Evidence Required** — the specific types of evidence that must be collected, retained, and made accessible to demonstrate that the policy is being followed. Each evidence type includes its system of record, owner, retention period, and collection frequency.
3. **Framework Obligations Satisfied** — the specific clauses, controls, or requirements within external regulatory and standards frameworks that each policy addresses, and the mechanism by which compliance is achieved.

This document supports three primary use cases:

- **Audit readiness:** Enables GRC team members and internal auditors to rapidly identify what evidence to collect for any given policy and where that evidence lives.
- **GRC programme governance:** Provides the executive and board-level view of what value the GRC programme delivers and why each policy exists.
- **Regulatory horizon scanning:** As new obligations emerge (e.g., EU AI Act implementing acts, sector-specific regulations), this document identifies which existing policies partially or fully satisfy those obligations and where new policies or evidence types are needed.

The document covers **10 Phase 1 policies** (Emyzer Technology, effective 2024) and **4 Phase 2 policies** (Emyzer Nexus, added 2025).

---

## 2. How to Use This Document

**For internal auditors and GRC team members reviewing a single policy:**
Navigate to the relevant section in Sections 3 or 4. The evidence table for that policy identifies every evidence type required, where it lives, who owns it, and how often it must be collected. Use this to build an evidence collection checklist before an audit or assessment.

**For external auditors (ISO, regulatory):**
Use Section 7 (Framework Coverage Summary) to identify which policies address the framework you are auditing. Then use the individual policy sections to locate specific clause mappings and the evidence required to satisfy each clause.

**For the GRC team during programme reviews:**
Use Section 5 (Compliance Evidence Summary Matrix) for a programme-level view of evidence collection requirements. Use Section 6 (Audit Readiness Notes) for practical guidance on demonstrating completeness to an auditor.

**For executives and board members:**
The "Organisational Benefits" bullet points at the start of each policy section summarise the business value of that policy in non-technical terms. Section 7 summarises overall framework coverage.

**Caveat:** This document records the design intent of each policy. Ongoing evidence collection, quality, and completeness is the responsibility of the evidence owner identified in each table. The GRC Team reviews evidence completeness quarterly as part of the control effectiveness monitoring programme.

---

## 3. Phase 1 Policy Mappings — Emyzer Technology

---

### 3.1 Information Security Policy

**Document:** [Information Security Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/information-security-policy.md)

#### Organisational Benefits

- **Legal defensibility:** A formally approved and published Information Security Policy establishes that Emyzer Technology has taken reasonable steps to govern information security. In the event of a breach or regulatory investigation, the policy demonstrates governance intent and executive accountability.
- **ISMS scope definition:** The policy formally defines the scope of the Information Security Management System (ISMS), which is a prerequisite for ISO 27001 certification. Without a formally scoped ISMS, the entire certification is at risk.
- **Executive accountability documented:** CISO and CEO approval signatures on the policy record that information security has executive sponsorship, satisfying a key auditor expectation and enabling security investment decisions to be traced back to approved policy.
- **Baseline for all subsidiary policies:** The Information Security Policy is the parent policy to all others in this programme; its existence and currency validates the policy hierarchy and provides legal enforceability for all subordinate controls.

#### Compliance Evidence Required

| # | Evidence Type | System of Record | Owner | Retention Period | Collection Frequency |
|---|---------------|-----------------|-------|-----------------|----------------------|
| 1 | CISO and CEO approval records (signed version history) | GRC Document Repository | CISO | 7 years | Per version release |
| 2 | Staff acknowledgement records (all employees and contractors have read and accepted the policy) | LMS / HR System | HR Lead | Duration of employment + 3 years | Annual (at policy review) + on hire |
| 3 | Annual policy review records (documented review with sign-off that content remains current) | GRC Document Repository | CISO | 7 years | Annual |
| 4 | Policy exception log (any approved departures from policy requirements, with risk acceptance sign-off) | ServiceNow GRC | CISO | 7 years | Continuous; quarterly review report |
| 5 | ISMS scope statement (formal document defining what is in and out of scope) | GRC Document Repository | CISO | Current version + 2 prior versions | Annual / as changed |

#### Framework Obligations Satisfied

| Framework | Specific Clause / Control | How Satisfied |
|-----------|--------------------------|---------------|
| ISO 27001:2022 | Cl. 5.2 — Policy [VERIFY]: Top management shall establish an information security policy | Policy establishes ISMS purpose, objectives, and executive commitment; approved by CEO (top management) |
| ISO 27001:2022 | Cl. 5.1 — Leadership and commitment [VERIFY] | CEO and CISO approval records demonstrate top-management leadership and commitment to ISMS |
| NIST CSF 2.0 | GV.PO-01 — Organizational cybersecurity policy is established [VERIFY] | Policy constitutes the organisational cybersecurity policy required by this function |
| NIST CSF 2.0 | GV.OC — Organizational context [VERIFY] | Policy scope statement defines organisational context and ISMS boundaries |
| COBIT 2019 | APO01.01 — Define the organizational structures, roles, and responsibilities [VERIFY] | Policy assigns ISMS ownership and governance responsibilities |
| COBIT 2019 | APO01.08 — Manage policy lifecycle [VERIFY] | Annual review process and approval history satisfies policy lifecycle management |

---

### 3.2 Access Control Policy

**Document:** [Access Control Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/access-control-policy.md)

#### Organisational Benefits

- **Least privilege reduces breach surface:** By mandating that staff are granted only the access necessary for their role, the policy directly reduces the potential impact of a compromised account. Lateral movement by an attacker is constrained when least privilege is enforced.
- **MFA reduces credential-based attack success:** Multi-factor authentication requirement, particularly for privileged and remote access, significantly reduces the probability of unauthorised access resulting from credential theft, phishing, or brute-force attacks — the most common initial access vectors.
- **Access reviews support insider threat detection:** Mandatory periodic access reviews ensure that access rights are recertified by managers, creating a structured mechanism to identify and revoke inappropriate or orphaned access rights before they are exploited.
- **Audit trail for regulatory compliance:** Privileged access logging and joiners/movers/leavers (JML) records provide the evidence trail required by GDPR (data access controls), PCI DSS (separation of duties), and ISO 27001 auditors.

#### Compliance Evidence Required

| # | Evidence Type | System of Record | Owner | Retention Period | Collection Frequency |
|---|---------------|-----------------|-------|-----------------|----------------------|
| 1 | Access review reports (completed recertification of all user and privileged accounts by managers) | ServiceNow GRC / IAM platform | IT Operations | 7 years | Quarterly for privileged accounts; semi-annual for all users |
| 2 | MFA enrollment records (confirmation of MFA enrollment per user; MFA enforcement evidence from directory) | Azure Active Directory / IAM platform | IT Operations | Duration of employment + 3 years | Continuous; monthly compliance report |
| 3 | Privileged access logs (logs of all privileged account activity, PAM system vault check-outs, admin session recordings) | PAM system (e.g., CyberArk / BeyondTrust) | CISO | 7 years | Continuous; monthly review |
| 4 | Joiners/movers/leavers records (evidence of access provisioning on hire, changes on role change, and timely revocation on departure) | HR System + ServiceNow ITSM | HR Lead + IT Operations | Duration of employment + 3 years | Per JML event; quarterly completeness audit |
| 5 | Role-Based Access Control (RBAC) role definitions (current approved role definitions and access entitlements per role) | IAM platform | IT Operations | Current version + 2 prior versions | Annual review / as changed |
| 6 | Policy exception records (approved departures, e.g., temporary elevated access) | ServiceNow GRC | CISO | 7 years | Per exception; quarterly review |

#### Framework Obligations Satisfied

| Framework | Specific Clause / Control | How Satisfied |
|-----------|--------------------------|---------------|
| ISO 27001:2022 | A.5.15 — Access control [VERIFY] | Policy mandates need-to-know and least privilege access; RBAC framework defined |
| ISO 27001:2022 | A.5.16 — Identity management [VERIFY] | Policy governs identity lifecycle including JML process; unique IDs required |
| ISO 27001:2022 | A.5.17 — Authentication information [VERIFY] | MFA requirements and password policy defined in Access Control Policy |
| ISO 27001:2022 | A.5.18 — Access rights [VERIFY] | Periodic access review requirements; formal provisioning and revocation process |
| ISO 27001:2022 | A.8.2 — Privileged access rights [VERIFY] | Privileged access management, PAM system requirements, and logging obligations |
| NIST SP 800-53 Rev. 5 | AC-1 — Policy and procedures [VERIFY] | Policy constitutes the organisational access control policy |
| NIST SP 800-53 Rev. 5 | AC-2 — Account management [VERIFY] | JML process and access review programme address account management requirements |
| NIST SP 800-53 Rev. 5 | AC-3 — Access enforcement [VERIFY] | RBAC framework and least privilege mandate address access enforcement |
| NIST SP 800-53 Rev. 5 | AC-5 — Separation of duties [VERIFY] | Policy requires separation of duties for privileged operations; RBAC enforces this |
| NIST SP 800-53 Rev. 5 | AC-6 — Least privilege [VERIFY] | Explicit least privilege requirement with documented role definitions |
| PCI DSS v4.0 | Requirement 7 — Restrict access to system components and cardholder data [VERIFY] | Access control policy and RBAC framework restrict access to cardholder data environments |
| PCI DSS v4.0 | Requirement 8 — Identify users and authenticate access [VERIFY] | MFA requirements and unique user ID mandate satisfy this requirement |

---

### 3.3 Incident Management Policy

**Document:** [Incident Management Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/incident-management-policy.md)

#### Organisational Benefits

- **Reduces mean time to contain (MTTC):** A structured incident response process with defined roles, escalation paths, and playbooks reduces the time between incident detection and containment, directly limiting the blast radius of security incidents.
- **Ensures regulatory notification timelines are met:** GDPR Article 33's [VERIFY] 72-hour supervisory authority notification deadline is a hard legal obligation. A defined policy with explicit notification triggers prevents organisations from inadvertently breaching this deadline through disorganised response.
- **Post-incident reviews drive continuous improvement:** Mandatory post-incident review (PIR) processes capture lessons learned and drive improvements to preventive controls and response procedures, reducing the probability of recurrence.
- **Preserves legal admissibility of evidence:** Documented chain of custody and evidence handling procedures during incidents ensure that forensic evidence remains legally admissible, supporting potential civil or criminal proceedings.

#### Compliance Evidence Required

| # | Evidence Type | System of Record | Owner | Retention Period | Collection Frequency |
|---|---------------|-----------------|-------|-----------------|----------------------|
| 1 | Incident register (log of all security incidents including classification, timeline, affected systems, and resolution) | ServiceNow Security Incident Management | CISO | 7 years | Continuous; monthly summary report |
| 2 | Incident response timeline records (documented timestamps for: detection, triage, containment, eradication, recovery, and closure) | ServiceNow Security Incident Management | CISO | 7 years | Per incident |
| 3 | GDPR 72-hour notification records (evidence of supervisory authority notification, content, and timestamp; or documented rationale for non-notification) | Legal Management System | Legal Counsel + CISO | 7 years (or longer per regulatory requirement [VERIFY]) | Per qualifying incident |
| 4 | Post-incident review reports (written PIR for all P1 and P2 incidents; root cause analysis; lessons learned; action items with owners and due dates) | ServiceNow GRC | CISO | 7 years | Per qualifying incident (P1 mandatory; P2 mandatory; P3 at CISO discretion) |
| 5 | Playbook version history (evidence that incident response playbooks are reviewed and updated; change log) | GRC Document Repository | CISO | Current + 2 prior versions | Annual review / after each major incident |
| 6 | IR training and awareness records (evidence that response team members have been trained on current playbooks) | LMS | CISO | 3 years | Annual |

#### Framework Obligations Satisfied

| Framework | Specific Clause / Control | How Satisfied |
|-----------|--------------------------|---------------|
| ISO/IEC 27035-1:2016 — Information security incident management [VERIFY] | Part 1: Principles and process | Policy defines the full incident management lifecycle (detect, report, assess, respond, learn) aligned to ISO 27035 phases |
| ISO 27001:2022 | A.5.24 — Information security incident management planning and preparation [VERIFY] | Policy and playbooks constitute the required incident management plans |
| ISO 27001:2022 | A.5.26 — Response to information security incidents [VERIFY] | Structured response procedures, escalation paths, and PIR requirements |
| NIST SP 800-61 Rev. 2 — Computer Security Incident Handling Guide [VERIFY] | All phases (Preparation, Detection, Containment, Eradication, Recovery, Post-incident) | Policy phases map to NIST 800-61 phases; playbooks operationalise each phase |
| GDPR | Article 33 — Notification of a personal data breach to the supervisory authority [VERIFY] | Policy includes explicit 72-hour notification trigger, process, and evidence requirement |
| GDPR | Article 34 — Communication of a personal data breach to the data subject [VERIFY] | Policy includes data subject notification assessment process |
| NIST CSF 2.0 | RS.MA — Incident management [VERIFY] | Policy constitutes the incident response plan required by this function |

---

### 3.4 Risk Management Policy

**Document:** [Risk Management Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/risk-management-policy.md)

#### Organisational Benefits

- **Risk-informed decision making:** A formalised risk management process ensures that investment decisions, change approvals, and operational choices are made with an accurate understanding of associated risks, reducing the probability of costly surprises.
- **Executive accountability for risk acceptance:** The policy defines who has authority to accept risks at different severity levels, creating a clear and auditable record that risk acceptance decisions were made deliberately by appropriate stakeholders rather than by default.
- **Prioritises security investment:** A maintained risk register enables the GRC team and CISO to present prioritised, evidence-based investment proposals to the board, ensuring that security budget is directed to the highest-risk areas.
- **Demonstrates due diligence to insurers and clients:** Enterprise clients and cyber insurers increasingly require evidence of formal risk management processes. A functioning risk management programme with a maintained register and documented risk treatment plans is a differentiator in enterprise procurement and can reduce cyber insurance premiums.

#### Compliance Evidence Required

| # | Evidence Type | System of Record | Owner | Retention Period | Collection Frequency |
|---|---------------|-----------------|-------|-----------------|----------------------|
| 1 | Risk register (complete and current register of all identified information security risks, with likelihood, impact, risk score, owner, treatment status, and residual risk) | ServiceNow GRC | CISO | 7 years (per version) | Continuous; quarterly formal review |
| 2 | Risk acceptance records (formal sign-off for each risk accepted above the defined risk appetite, with accepting authority, date, and review date) | ServiceNow GRC | CISO + accepting authority | 7 years | Per risk acceptance decision |
| 3 | Quarterly risk committee minutes (documented output of risk committee meetings including risks discussed, decisions made, and actions assigned) | GRC Document Repository | CISO | 7 years | Quarterly |
| 4 | Annual risk appetite review records (evidence of board or executive review and reaffirmation of risk appetite statements) | GRC Document Repository | CISO + CEO | 7 years | Annual |
| 5 | Risk treatment plan records (documented risk treatment plans for all High and Critical risks, with treatment owner, timeline, and completion evidence) | ServiceNow GRC | Risk owners | 7 years | Per treatment plan; quarterly status review |
| 6 | Risk assessment methodology document (documented scoring methodology, likelihood/impact scales, and risk appetite thresholds — version controlled) | GRC Document Repository | CISO | Current + 2 prior versions | Annual review |

#### Framework Obligations Satisfied

| Framework | Specific Clause / Control | How Satisfied |
|-----------|--------------------------|---------------|
| ISO 31000:2018 — Risk management guidelines [VERIFY] | Clauses 6.3–6.6 (Risk assessment process: identification, analysis, evaluation, treatment) | Policy defines risk assessment methodology aligned to ISO 31000 principles; risk register and treatment plans operationalise the process |
| ISO 27001:2022 | Cl. 6.1.2 — Information security risk assessment [VERIFY] | Policy mandates risk identification, analysis, and evaluation; risk register is the output |
| ISO 27001:2022 | Cl. 6.1.3 — Information security risk treatment [VERIFY] | Risk treatment plans and risk acceptance process with defined authority levels |
| NIST CSF 2.0 | ID.RA — Risk assessment [VERIFY] | Risk identification and scoring methodology satisfies this function |
| NIST CSF 2.0 | GV.RM — Risk management strategy [VERIFY] | Risk appetite statements and executive risk governance satisfy this function |
| NIST SP 800-30 Rev. 1 [VERIFY] | Guide for conducting risk assessments | Risk assessment methodology references NIST 800-30 threat and vulnerability identification approach |
| COSO ERM (2017) [VERIFY] | Component 3: Performance — Assesses severity of risk | Risk scoring matrix and treatment prioritisation process align to COSO ERM performance component |

---

### 3.5 Business Continuity and Disaster Recovery Policy

**Document:** [BC/DR Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/bcdr-policy.md)

#### Organisational Benefits

- **Quantified RTOs and RPOs enable investment decisions:** By establishing maximum tolerable periods of disruption for each business function, the policy provides the business case for DR infrastructure investment. Without defined RTOs and RPOs, it is impossible to justify the cost of redundant infrastructure versus the cost of downtime.
- **Reduces prolonged outage impact:** A tested and maintained BCP reduces both the duration and impact of disruptions. The BIA quantifies daily financial exposure at $2.8M+ for complete Emyzer Technology outage; a 2-hour RTO for Tier 1 functions caps that exposure relative to an unmanaged recovery.
- **Demonstrates due diligence to enterprise clients:** Managed service and cloud service clients with their own compliance obligations frequently require evidence of their suppliers' BCPs. A mature, ISO 22301-aligned programme is a competitive differentiator in enterprise procurement and contract retention.
- **Satisfies contractual SLA obligations:** Emyzer Technology's 99.99% uptime SLA commitments to 340 cloud service clients require a tested technical recovery capability. The policy mandates and governs that capability, reducing SLA breach liability.

#### Compliance Evidence Required

| # | Evidence Type | System of Record | Owner | Retention Period | Collection Frequency |
|---|---------------|-----------------|-------|-----------------|----------------------|
| 1 | Business Impact Analysis report (documented BIA with process inventory, impact analysis, and RTO/RPO/MTPD outcomes) | GRC Document Repository | BC Manager | 7 years | Annual refresh; trigger-based update |
| 2 | Business Continuity Plan (current version of BC-PLAN-001 and all annexes) | GRC Document Repository | BC Manager | 7 years per version | Annual review; trigger-based update |
| 3 | DR test results (technical DR failover test reports including RTO/RPO measurement, pass/fail outcomes, and observations) | ServiceNow + AWS CloudWatch export | IT Recovery Lead | 7 years | Semi-annual |
| 4 | Tabletop exercise reports (written reports from CMT plan walkthroughs and scenario exercises) | GRC Document Repository | BC Manager | 7 years | Annual |
| 5 | Supplier BCP attestations (annual written confirmation from Tier 1 suppliers that their BCP is current and tested) | Vendor Risk Register (ServiceNow) | Vendor Risk Manager | 7 years | Annual |
| 6 | Plan activation records (for any real activations: log of trigger, CMT actions, recovery timeline, and deactivation confirmation) | ServiceNow | BC Manager | 7 years | Per activation |
| 7 | Recovery time validation records (timestamped evidence that stated RTOs were achieved in tests) | ServiceNow | IT Recovery Lead | 7 years | Per DR test |

#### Framework Obligations Satisfied

| Framework | Specific Clause / Control | How Satisfied |
|-----------|--------------------------|---------------|
| ISO 22301:2019 | Cl. 8.2 — Business impact analysis and risk assessment [VERIFY] | BIA requirement mandated by policy; BIA report is deliverable |
| ISO 22301:2019 | Cl. 8.3 — Business continuity strategy and solutions [VERIFY] | Policy defines BC strategy requirements; BCP documents strategies |
| ISO 22301:2019 | Cl. 8.4 — Business continuity plans and procedures [VERIFY] | BCP (BC-PLAN-001) is the primary deliverable required by this clause |
| ISO 22301:2019 | Cl. 8.5 — Exercise programme [VERIFY] | Policy mandates semi-annual DR testing and annual exercises |
| ISO 27001:2022 | A.5.29 — Information security during disruption [VERIFY] | Policy and BCP ensure information security controls operate during disruption |
| ISO 27001:2022 | A.5.30 — ICT readiness for business continuity [VERIFY] | DR infrastructure requirements and RTO/RPO mandates address ICT readiness |
| NIST SP 800-34 Rev. 1 [VERIFY] | Contingency planning guide for federal information systems (adopted as best practice) | Policy lifecycle maps to NIST 800-34's 7-phase contingency planning process |

---

### 3.6 Change Management and Configuration Policy

**Document:** [Change Management and Configuration Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/change-management-and-configuration-policy.md)

#### Organisational Benefits

- **Reduces risk of service outages from unauthorised changes:** Studies consistently show that 70–80% of unplanned IT outages are caused by changes. A formal change approval process with pre-implementation testing and rollback planning materially reduces this risk.
- **Provides comprehensive audit trail:** All changes to production systems are logged in ServiceNow with requester, approver, implementation window, and outcome. This audit trail is required for ISO 27001 and SOC 2 audits and supports forensic investigation of incidents.
- **AI model retraining governed:** The policy extends change governance to AI model retraining and updates — ensuring that changes to AI systems used in operations are subject to the same risk assessment and approval process as infrastructure changes, supporting EU AI Act compliance.
- **Enables rapid and safe emergency change:** A defined Emergency Change process allows critical fixes to be implemented quickly while maintaining appropriate documentation and retrospective review, balancing agility with control.

#### Compliance Evidence Required

| # | Evidence Type | System of Record | Owner | Retention Period | Collection Frequency |
|---|---------------|-----------------|-------|-----------------|----------------------|
| 1 | CAB meeting minutes (record of all Change Advisory Board meetings, changes reviewed, approvals and rejections, and rationale) | ServiceNow ITSM | IT Operations | 7 years | Per CAB meeting (typically weekly) |
| 2 | Change request records (all submitted RFCs including type, requester, risk assessment, test plan, rollback plan, approval status, and outcome) | ServiceNow ITSM | IT Operations | 7 years | Per change request |
| 3 | Post-implementation review records (completed PIRs for significant changes, confirming objectives met and no unintended side effects) | ServiceNow ITSM | Change owner | 7 years | Per significant change; all P1/Major changes |
| 4 | Emergency change log (register of all emergency changes with retrospective CAB approval and justification for bypassing standard process) | ServiceNow ITSM | IT Operations | 7 years | Per emergency change; monthly report |
| 5 | Configuration baseline records (documented approved configuration baselines for all critical systems, with version history) | CMDB (ServiceNow) | IT Operations | Current + 3 prior versions | Per change; quarterly audit |
| 6 | Unauthorised change detection records (evidence of configuration drift detection and investigation outcomes) | CMDB / configuration management tooling | IT Operations | 7 years | Continuous; monthly report |

#### Framework Obligations Satisfied

| Framework | Specific Clause / Control | How Satisfied |
|-----------|--------------------------|---------------|
| ITIL 4 | Change enablement practice [VERIFY] | Policy implements formal change enablement process aligned to ITIL 4 guidance, including RFC, CAB, and emergency change procedures |
| ISO 27001:2022 | A.8.32 — Change management [VERIFY] | Policy and ServiceNow process constitute the change management controls required by this annex control |
| ISO 27001:2022 | A.8.9 — Configuration management [VERIFY] | CMDB and configuration baseline requirements address configuration management |
| COBIT 2019 | BAI06 — Managed IT changes [VERIFY] | Policy governance and CAB process align to COBIT BAI06 management practice |
| COBIT 2019 | BAI10 — Managed configuration [VERIFY] | CMDB and configuration baseline management address BAI10 |
| NIST CSF 2.0 | PR.PS — Platform security [VERIFY] | Change and configuration controls are primary contributors to this category |

---

### 3.7 Acceptable Use Policy

**Document:** [Acceptable Use Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/acceptable-use-policy.md)

#### Organisational Benefits

- **Establishes the behavioural baseline for all staff:** The AUP defines what constitutes acceptable and unacceptable use of company systems, data, and assets. Without this baseline, it is difficult to take disciplinary action for misuse, as employees can claim they were unaware that a behaviour was prohibited.
- **Enables proportionate disciplinary action for violations:** By making policy requirements explicit and obtaining signed acknowledgements, the AUP creates the legal and HR foundation for disciplinary proceedings including dismissal for serious violations (e.g., data exfiltration, use of company systems for illegal activity).
- **Reduces shadow IT risk:** The AUP explicitly addresses the use of unsanctioned applications and cloud services. Combined with technical controls, it establishes that staff are not authorised to use unapproved tools for work data, reducing the organisation's exposure to data stored in uncontrolled third-party services.
- **Supports cyber insurance claims:** In the event of a cyber claim, insurers review whether the organisation had documented acceptable use requirements. The AUP and acknowledgement records demonstrate that users were informed of their obligations.

#### Compliance Evidence Required

| # | Evidence Type | System of Record | Owner | Retention Period | Collection Frequency |
|---|---------------|-----------------|-------|-----------------|----------------------|
| 1 | Staff acknowledgement records (evidence that all employees, contractors, and relevant third parties have read, understood, and agreed to the AUP) | LMS / HR System | HR Lead | Duration of employment + 3 years | Annual re-acknowledgement + on hire / on policy update |
| 2 | AUP policy violation records (documented record of all confirmed AUP violations, investigation outcomes, and disciplinary actions taken) | HR System (restricted) | HR Lead + CISO | Duration of employment + 7 years | Per violation |
| 3 | AUP training completion records (evidence that staff have completed AUP awareness training, including date and assessment score where applicable) | LMS | HR Lead | Duration of employment + 3 years | Annual |
| 4 | Shadow IT detection records (evidence from CASB or network monitoring tools identifying unsanctioned application usage and remediation actions) | CASB / network security tooling | CISO | 2 years | Monthly report |

#### Framework Obligations Satisfied

| Framework | Specific Clause / Control | How Satisfied |
|-----------|--------------------------|---------------|
| ISO 27001:2022 | A.5.10 — Acceptable use of information and other associated assets [VERIFY] | Policy constitutes the acceptable use policy required by this annex control |
| ISO 27001:2022 | A.6.2 — Terms and conditions of employment [VERIFY] | AUP acknowledgement as condition of employment addresses this requirement |
| NIST CSF 2.0 | PR.AT-01 — Awareness activities [VERIFY] | AUP training and acknowledgement programme is a component of the awareness activities required |
| NIST SP 800-53 Rev. 5 | PL-4 — Rules of behaviour [VERIFY] | AUP constitutes the rules of behaviour required for system users |

---

### 3.8 Data Classification Policy

**Document:** [Data Classification Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/data-classification-policy.md)

#### Organisational Benefits

- **Ensures PII is handled to GDPR standard:** Data classification is the foundation of GDPR compliance. Without knowing which data is personal data and how it is classified, it is impossible to apply appropriate handling controls (encryption, access restrictions, retention limits), creating systematic regulatory risk.
- **Prevents over-sharing of confidential data:** Classification labels and associated handling rules create a mechanism for preventing employees from inadvertently sharing confidential or restricted data via unsecured channels (email, personal cloud storage). DLP controls enforced on the basis of classification labels provide technical reinforcement.
- **Informs retention and deletion decisions:** Data classification levels are mapped to retention schedules. This ensures that high-classification data is not retained beyond its legal or business necessity period, reducing the volume of regulated data in scope during a breach.
- **Enables proportionate security investment:** Classification-based access controls, encryption requirements, and monitoring intensity allow security investment to be proportionate to data sensitivity rather than applying maximum controls uniformly, improving cost-efficiency.

#### Compliance Evidence Required

| # | Evidence Type | System of Record | Owner | Retention Period | Collection Frequency |
|---|---------------|-----------------|-------|-----------------|----------------------|
| 1 | Data classification audit reports (evidence that data assets have been classified per the policy; completeness of classification coverage) | GRC Document Repository | CISO | 7 years | Annual audit |
| 2 | Data inventory / information asset register (register of all significant data assets with classification, owner, storage location, and retention period) | ServiceNow GRC / CMDB | Data owners | Current version + 2 prior versions | Annual review; continuous for new assets |
| 3 | Data handling procedure acknowledgements (evidence that staff in roles with access to Confidential or Restricted data have been trained on handling requirements) | LMS | HR Lead + Data owners | Duration of employment + 3 years | Annual + on role change |
| 4 | Data Processing Agreement (DPA) records (evidence that DPAs are in place with all processors handling personal data) | Legal Management System | Legal Counsel | Duration of contract + 7 years | Per new processor; annual review of existing |
| 5 | DLP policy configuration records (evidence that DLP technical controls are configured to enforce classification-based handling rules) | CISO | CASB / DLP tooling | 3 years | Quarterly review |
| 6 | Data classification incident records (record of incidents involving mishandling or misclassification of data) | ServiceNow | CISO | 7 years | Per incident |

#### Framework Obligations Satisfied

| Framework | Specific Clause / Control | How Satisfied |
|-----------|--------------------------|---------------|
| NIST SP 800-60 Vol. 1 — Guide for mapping types of information and information systems to security categories [VERIFY] | Volume 1: categorisation process | Classification scheme and handling procedures reference NIST 800-60 categorisation approach |
| ISO 27001:2022 | A.5.12 — Classification of information [VERIFY] | Policy constitutes the information classification policy required by this annex control |
| ISO 27001:2022 | A.5.13 — Labelling of information [VERIFY] | Labelling requirements for classified assets are defined in the policy |
| ISO 27001:2022 | A.5.14 — Information transfer [VERIFY] | Transfer controls based on classification level address this requirement |
| GDPR | Article 5 — Principles relating to processing of personal data [VERIFY] (integrity and confidentiality principle) | Classification and handling controls for personal data demonstrate implementation of the integrity and confidentiality principle |
| GDPR | Article 32 — Security of processing [VERIFY] | Classification-based encryption and access controls satisfy the Article 32 obligation to implement appropriate technical measures |

---

### 3.9 Third-Party Risk Management Policy

**Document:** [Third-Party Risk Management Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/third-party-risk-management-policy.md)

#### Organisational Benefits

- **Identifies concentration risk:** The TPRM programme maps all critical third-party dependencies and identifies where single suppliers represent concentration risk (e.g., a single cloud provider hosting multiple Tier 1 systems). This analysis informs risk treatment and BCM decisions.
- **Ensures vendor security posture is verified before onboarding:** Pre-contract due diligence, including review of SOC 2 reports, penetration test results, and security questionnaire responses, prevents Emyzer Technology from inadvertently inheriting security weaknesses from its supply chain.
- **Contractual security obligations are enforceable:** The policy defines the minimum security requirements that must be included in supplier contracts (including breach notification timelines, audit rights, and BCP requirements). Without these contractual provisions, Emyzer Technology has no legal mechanism to compel suppliers to meet security standards.
- **Supports regulatory supply chain obligations:** DORA (where applicable to Emyzer Technology's financial technology services), GDPR (processor obligations), and the NIS2 Directive's supply chain requirements all mandate some form of third-party risk management. This policy provides the governance framework to satisfy those obligations.

#### Compliance Evidence Required

| # | Evidence Type | System of Record | Owner | Retention Period | Collection Frequency |
|---|---------------|-----------------|-------|-----------------|----------------------|
| 1 | Vendor risk assessments (completed risk assessments for all Tier 1 and Tier 2 suppliers, including security questionnaire responses and findings) | Vendor Risk Register (ServiceNow) | Vendor Risk Manager | Duration of contract + 7 years | On onboarding; annual reassessment for Tier 1 |
| 2 | Contract security addenda (evidence that applicable supplier contracts include required security provisions: breach notification, audit rights, BCP, data protection) | Legal Management System | Legal Counsel | Duration of contract + 7 years | Per contract; annual compliance review |
| 3 | SOC 2 / ISAE 3402 reports on file (current third-party assurance reports for all cloud-hosted Tier 1 and Tier 2 suppliers) | GRC Document Repository | Vendor Risk Manager | Current report + 1 prior year | Annual (upon supplier report issuance) |
| 4 | Continuous monitoring records (evidence of ongoing supplier risk monitoring, including alerts from risk intelligence platforms and response actions) | ServiceNow | Vendor Risk Manager | 3 years | Monthly summary report |
| 5 | Supplier offboarding records (evidence of data deletion/return, access revocation, and contract termination for departed suppliers) | ServiceNow + Legal Management System | Vendor Risk Manager + IT Operations | 7 years | Per offboarding event |
| 6 | Fourth-party risk assessments (evidence of review of material subprocessors used by Tier 1 suppliers) | Vendor Risk Register (ServiceNow) | Vendor Risk Manager | 7 years | Annual |

#### Framework Obligations Satisfied

| Framework | Specific Clause / Control | How Satisfied |
|-----------|--------------------------|---------------|
| ISO/IEC 27036-1 — Information security for supplier relationships [VERIFY] | Part 1: Overview and concepts | TPRM policy framework aligns to ISO 27036 supplier security governance principles |
| ISO 27001:2022 | A.5.19 — Information security in supplier relationships [VERIFY] | Policy establishes supplier security requirements and governance framework |
| ISO 27001:2022 | A.5.20 — Addressing information security within supplier agreements [VERIFY] | Contract security addenda requirements address this control |
| ISO 27001:2022 | A.5.21 — Managing information security in the ICT supply chain [VERIFY] | ICT supply chain risk management and fourth-party risk assessment address this control |
| NIST SP 800-161 Rev. 1 — Cybersecurity supply chain risk management [VERIFY] | Core practices for C-SCRM | Policy implements supplier risk tiering, assessment, and monitoring consistent with NIST 800-161 |
| NIST CSF 2.0 | ID.SC — Improvement [VERIFY] | Supplier risk identification and assessment satisfy this subcategory |
| GDPR | Article 28 — Processor [VERIFY] | DPA requirements and processor security obligations in contract addenda satisfy Article 28 |

---

### 3.10 Security Awareness and Training Policy (Phase 1 — Emyzer Technology)

**Document:** [Security Awareness and Training Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/security-awareness-and-training-policy.md)

#### Organisational Benefits

- **Reduces phishing click rates:** Regular phishing simulation programmes with follow-up training for users who click on simulated phishing emails demonstrate measurable reductions in susceptibility. A well-run programme typically achieves 30–50% reduction in click rates within 12 months.
- **Builds security culture:** Consistent security awareness communications, role-specific training, and visible management endorsement establish security as an organisational norm rather than an IT-imposed constraint, reducing shadow IT behaviours and improving voluntary incident reporting rates.
- **Satisfies regulator expectations for staff training:** Regulatory frameworks including GDPR, PCI DSS, and ISO 27001 explicitly require evidence that staff have been trained on their security obligations. In enforcement actions and audits, training records are among the first evidence requests.
- **Reduces insider risk from unintentional actions:** A significant proportion of data breaches involve unintentional insider actions — misaddressed emails, accidental public sharing of files, and misconfigured access. Training on correct data handling reduces this category of risk.

#### Compliance Evidence Required

| # | Evidence Type | System of Record | Owner | Retention Period | Collection Frequency |
|---|---------------|-----------------|-------|-----------------|----------------------|
| 1 | LMS training completion records (evidence that all staff have completed mandatory security awareness modules, including completion date, score, and any remediation training) | LMS | HR Lead | Duration of employment + 3 years | Annual completion; monthly compliance tracking |
| 2 | Phishing simulation results (metrics from simulated phishing campaigns: click rate, credential submission rate, report rate, trend over time) | Security awareness platform | CISO | 3 years | Quarterly campaigns; quarterly aggregate report |
| 3 | Role-specific training records (evidence of completion of role-specific training for high-risk roles: privileged users, finance staff, HR, executives) | LMS | HR Lead + CISO | Duration of employment + 3 years | Annual; upon role change |
| 4 | Security awareness programme schedule and content (documented annual training plan with topics, delivery methods, and target audiences) | GRC Document Repository | CISO | 3 years | Annual planning; quarterly review |
| 5 | Training effectiveness metrics (evidence of programme effectiveness: phishing click rate trends, incident rates correlated to training cycles, knowledge assessment scores) | LMS + SIEM data | CISO | 3 years | Annual effectiveness report |

#### Framework Obligations Satisfied

| Framework | Specific Clause / Control | How Satisfied |
|-----------|--------------------------|---------------|
| ISO 27001:2022 | A.6.3 — Information security awareness, education and training [VERIFY] | Policy mandates and governs the security awareness and training programme required by this annex control |
| ISO 27001:2022 | Cl. 7.2 — Competence [VERIFY] | Role-specific training requirements ensure staff are competent to perform security-relevant activities |
| NIST SP 800-50 — Building an information technology security awareness and training programme [VERIFY] | All sections | Policy and programme structure align to NIST 800-50 guidance on awareness and training programme design |
| NIST CSF 2.0 | PR.AT — Awareness and training [VERIFY] | Programme satisfies all subcategories within this function |
| PCI DSS v4.0 | Requirement 12.6 — Security awareness programme [VERIFY] | Annual training, phishing simulation, and completion record requirements satisfy PCI DSS Req. 12.6 |
| GDPR | Article 29 / Recital 74 [VERIFY] | Training on data protection obligations for staff processing personal data |

---

## 4. Phase 2 Policy Mappings — Emyzer Nexus

Phase 2 policies govern the expanded Emyzer Nexus entity following the Q4 2024 acquisition of Veridian AI. These policies extend the Phase 1 programme to address AI-specific risks, Veridian AI staff integration, and additional regulatory obligations applicable at the Nexus level.

---

### 4.1 AI Governance Policy

**Document:** [AI Governance Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/enterprise-policies/ai-governance-policy.md)

#### Organisational Benefits

- **EU AI Act compliance reduces penalty risk:** The EU AI Act (Regulation 2024/1689) [VERIFY] imposes penalties for non-compliance of up to €35 million or 7% of global annual turnover, whichever is higher, for providers of prohibited or non-compliant high-risk AI systems [VERIFY: confirm current penalty tier thresholds in force under implementing regulations]. The AI Governance Policy establishes the governance structure required to identify applicable obligations and achieve compliance before enforcement begins.
- **Demonstrates responsible AI to enterprise clients:** Enterprise clients — particularly those in regulated industries (financial services, healthcare, critical infrastructure) — increasingly require evidence of responsible AI governance from their technology suppliers. The AI Governance Policy and associated evidence package differentiates Emyzer Nexus in procurement processes.
- **Protects against inherited Veridian AI compliance gaps:** The Q4 2024 acquisition of Veridian AI introduced AI systems that may not have been designed with EU AI Act obligations in mind. The AI Governance Policy mandates a systematic inventory and conformity assessment of all AI systems, enabling identification and remediation of inherited compliance gaps before they become regulatory exposure.
- **Establishes human oversight for high-risk AI decisions:** The policy's human oversight and override requirements ensure that AI-generated outputs that affect material business or customer decisions are subject to human review, reducing legal liability and reputational risk from AI errors.

#### Compliance Evidence Required

| # | Evidence Type | System of Record | Owner | Retention Period | Collection Frequency |
|---|---------------|-----------------|-------|-----------------|----------------------|
| 1 | AI system inventory (register of all AI systems in use at Emyzer Nexus including Veridian AI systems, with risk classification, use case, and EU AI Act category) | AI Governance Register (ServiceNow) | AI Governance Committee | Lifecycle of system + 10 years [VERIFY] | Continuous; quarterly completeness audit |
| 2 | Conformity assessment records (for each high-risk AI system: technical documentation, conformity assessment procedure, and declaration of conformity where required) | GRC Document Repository | AI Governance Committee | Lifecycle of system + 10 years [VERIFY] | Per system classification; annual review for existing systems |
| 3 | AI Governance Committee minutes (records of committee meetings, decisions on AI system approvals, risk acceptances, and policy interpretations) | GRC Document Repository | AI Governance Committee | 7 years | Monthly meeting minutes |
| 4 | Human override logs (records of human review and override of AI-generated outputs for high-risk decisions; frequency and outcome trends) | AI system logs + ServiceNow | AI system owners | 5 years | Continuous; monthly aggregate report |
| 5 | Post-market monitoring reports (evidence of ongoing monitoring of high-risk AI system performance, drift, and real-world impact) | AI monitoring platform | AI system owners | Lifecycle of system + 5 years | Monthly monitoring reports; annual summary |
| 6 | Serious incident notification records (records of notifications made to national market surveillance authority per EU AI Act Article 73 [VERIFY]) | Legal Management System | Legal Counsel | 10 years [VERIFY] | Per qualifying serious incident |

#### Framework Obligations Satisfied

| Framework | Specific Clause / Control | How Satisfied |
|-----------|--------------------------|---------------|
| EU AI Act (Regulation 2024/1689) [VERIFY] | Article 9 — Risk management system for high-risk AI systems [VERIFY] | Policy mandates risk management system for all AI systems; AI Governance Committee implements and oversees |
| EU AI Act (Regulation 2024/1689) [VERIFY] | Article 10 — Data and data governance [VERIFY] | Policy addresses training data governance and data quality requirements for AI systems |
| EU AI Act (Regulation 2024/1689) [VERIFY] | Article 13 — Transparency and provision of information [VERIFY] | Policy requires transparency documentation for AI systems interacting with users |
| EU AI Act (Regulation 2024/1689) [VERIFY] | Article 14 — Human oversight [VERIFY] | Human oversight and override requirements operationalise this obligation |
| EU AI Act (Regulation 2024/1689) [VERIFY] | Article 17 — Quality management system [VERIFY] | AI Governance Committee and quality management requirements address this article |
| NIST AI RMF 1.0 | Govern — Establishing accountability [VERIFY] | AI Governance Committee structure and policy ownership address the Govern function |
| NIST AI RMF 1.0 | Map — Categorising risk context [VERIFY] | AI system inventory and risk classification operationalise the Map function |
| ISO/IEC 42001:2023 — AI management systems [VERIFY] | Cl. 6.1 — AI risk assessment [VERIFY] | Policy mandates AI-specific risk assessment aligned to ISO 42001 requirements |

---

### 4.2 Model Risk Policy

**Document:** [Model Risk Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/enterprise-policies/model-risk-policy.md)

#### Organisational Benefits

- **Prevents model failures from driving material business decisions on faulty outputs:** As Emyzer Nexus integrates Veridian AI models into cloud services and enterprise tooling, model failures (degraded accuracy, distributional shift, adversarial manipulation) could cause incorrect outputs to inform pricing, security triage, or customer recommendations with direct financial and reputational consequences. The Model Risk Policy defines the governance controls that catch failures before they propagate.
- **Defines bias testing cadence:** Algorithmic bias in AI models used for recruitment, credit, or resource allocation creates legal exposure (Equality Act, GDPR automated decision-making provisions). A defined bias testing schedule, documented methodology, and remediation process demonstrates proactive governance to regulators.
- **Provides human oversight framework for model outputs:** The policy defines when human review is mandatory before an AI output can be actioned, which AI outputs may be actioned automatically, and what the escalation process is when model confidence is below defined thresholds.
- **Enables evidence-based model lifecycle decisions:** Model performance monitoring data provides the objective basis for retraining, deprecation, and replacement decisions, preventing continued operation of degraded models beyond their useful life.

#### Compliance Evidence Required

| # | Evidence Type | System of Record | Owner | Retention Period | Collection Frequency |
|---|---------------|-----------------|-------|-----------------|----------------------|
| 1 | Model performance reports (regular metrics reports for each production model: accuracy, precision/recall, latency, confidence distribution, comparison against baseline) | AI monitoring platform | Model owners | Lifecycle of model + 5 years | Monthly |
| 2 | Bias audit reports (documented results of bias testing against protected characteristics and fairness metrics, per model and per test cycle) | GRC Document Repository | AI Governance Committee | Lifecycle of model + 7 years | Quarterly for high-risk models; annual for others |
| 3 | Retraining records (evidence of each model retraining cycle: trigger (scheduled or drift-detected), training data provenance, training parameters, validation metrics, and approval for production deployment) | AI Governance Register | Model owners | Lifecycle of model + 5 years | Per retraining event |
| 4 | Drift detection alerts and responses (log of all model drift alerts triggered by monitoring systems and documented response actions taken) | AI monitoring platform | Model owners | Lifecycle of model + 3 years | Continuous monitoring; monthly alert summary |
| 5 | Model validation records (independent validation of models prior to production deployment, including challenger model comparison where applicable) | GRC Document Repository | AI Governance Committee | Lifecycle of model + 7 years | Per new model; per major retraining |
| 6 | Model inventory (register of all production models with version, owner, risk classification, deployment date, and retirement status) | AI Governance Register | AI Governance Committee | 10 years | Continuous; quarterly audit |

#### Framework Obligations Satisfied

| Framework | Specific Clause / Control | How Satisfied |
|-----------|--------------------------|---------------|
| SR 11-7 (Federal Reserve / OCC model risk management guidance) [VERIFY] | Sections on model validation, governance, and ongoing monitoring | Policy implements SR 11-7's three-component model risk framework: development/implementation, validation, and ongoing monitoring — adapted for technology company context |
| NIST AI RMF 1.0 | Measure — Analysing and monitoring AI risk [VERIFY] | Model performance monitoring, bias testing, and drift detection operationalise the Measure function |
| NIST AI RMF 1.0 | Manage — Prioritising and acting on AI risk [VERIFY] | Retraining triggers, retirement process, and human oversight requirements operationalise the Manage function |
| EU AI Act (Regulation 2024/1689) [VERIFY] | Article 15 — Accuracy, robustness and cybersecurity [VERIFY] | Model performance requirements, drift detection, and adversarial robustness testing address this article |
| EU AI Act (Regulation 2024/1689) [VERIFY] | Article 72 — Post-market monitoring by providers [VERIFY] | Post-market monitoring programme for high-risk AI systems |
| ISO/IEC 42001:2023 [VERIFY] | Cl. 9.1 — Monitoring, measurement, analysis and evaluation [VERIFY] | Model performance monitoring programme satisfies this clause |

---

### 4.3 Privacy and Data Protection Policy

**Document:** [Privacy and Data Protection Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/enterprise-policies/privacy-and-data-protection-policy.md)

#### Organisational Benefits

- **GDPR compliance enables EU operations:** Processing personal data of EU data subjects without a compliant legal basis and appropriate technical/organisational measures is unlawful. The Privacy and Data Protection Policy establishes the governance framework that enables Emyzer Nexus to lawfully process EU personal data, which is essential for its European cloud and enterprise service operations.
- **Reduces financial penalties:** GDPR provides for administrative fines of up to €20 million or 4% of global annual turnover for the most serious infringements [VERIFY]. A documented and enforced data protection programme directly reduces the probability and potential severity of penalties.
- **Protects against data subject complaints and litigation:** Data subject rights under GDPR (access, erasure, portability, restriction, objection) must be honoured within defined timeframes. A managed data subject request process prevents complaints to supervisory authorities and class action litigation.
- **Builds client trust:** Enterprise clients whose own GDPR compliance depends on Emyzer Nexus as a processor will review data protection governance as a condition of procurement. This policy and its associated evidence package are directly relevant to client due diligence.

#### Compliance Evidence Required

| # | Evidence Type | System of Record | Owner | Retention Period | Collection Frequency |
|---|---------------|-----------------|-------|-----------------|----------------------|
| 1 | Data Protection Impact Assessment (DPIA) records (completed DPIAs for all high-risk processing activities, with outcomes and mitigations) | GRC Document Repository | DPO / Legal Counsel | Duration of processing + 5 years | Per new high-risk processing activity; annual review for ongoing activities |
| 2 | Data subject request records (log of all received DSARs and other data subject rights requests, with response timeline and outcome) | Legal Management System | DPO / Legal Counsel | 3 years post-resolution | Per request |
| 3 | Data Processing Agreement (DPA) register (evidence that DPAs are in place with all processors and sub-processors handling personal data) | Legal Management System | Legal Counsel | Duration of contract + 7 years | Per new processor; annual review |
| 4 | Personal data breach notification records (evidence of breach notifications to supervisory authority and data subjects, including content, timestamp, and outcome) | Legal Management System | DPO / Legal Counsel + CISO | 7 years (or longer per regulatory requirement [VERIFY]) | Per breach |
| 5 | Records of Processing Activities (RoPA) (Article 30 [VERIFY] register of all processing activities, including purposes, categories of data, recipients, and retention periods) | GRC Document Repository / Privacy management tool | DPO | Current version continuously maintained | Continuous; annual completeness audit |
| 6 | Lawful basis records (documented identification of lawful basis for each processing activity in the RoPA) | GRC Document Repository | DPO | Duration of processing + 5 years | Per new processing activity |
| 7 | Consent records (for consent-based processing: evidence of granular, informed, freely given consent and withdrawal mechanism) | Consent management platform | DPO | Duration of consent + 3 years | Per consent capture |

#### Framework Obligations Satisfied

| Framework | Specific Clause / Control | How Satisfied |
|-----------|--------------------------|---------------|
| GDPR (Regulation 2016/679) [VERIFY] | Article 5 — Principles relating to processing [VERIFY] | Policy operationalises lawfulness, fairness, transparency, purpose limitation, data minimisation, accuracy, storage limitation, and integrity/confidentiality principles |
| GDPR (Regulation 2016/679) [VERIFY] | Article 24 — Responsibility of the controller [VERIFY] | Policy establishes controller accountability with documented governance structure |
| GDPR (Regulation 2016/679) [VERIFY] | Article 25 — Data protection by design and by default [VERIFY] | Privacy-by-design requirements for new systems and processes |
| GDPR (Regulation 2016/679) [VERIFY] | Article 30 — Records of processing activities [VERIFY] | RoPA requirement directly satisfies this article |
| GDPR (Regulation 2016/679) [VERIFY] | Article 32 — Security of processing [VERIFY] | Technical and organisational measures requirements |
| UK GDPR (UK Data Protection Act 2018) [VERIFY] | Equivalent provisions to EU GDPR | Policy applies to both EU and UK data subject rights; dual compliance approach documented |
| ISO/IEC 27701:2019 — Privacy information management [VERIFY] | Clause 6 (Requirements specific to controllers) and Clause 7 (Requirements specific to processors) | Policy and PIMS extend the ISMS (ISO 27001) to privacy information management as required by ISO 27701 |

---

### 4.4 Security Awareness and Training Policy — Tier 2 (Emyzer Nexus)

**Document:** [Security Awareness and Training Policy (Emyzer Nexus)](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/enterprise-policies/security-awareness-and-training-policy.md)

#### Organisational Benefits

- **Extends AI-specific training to Veridian AI staff:** Following the Q4 2024 acquisition, Veridian AI staff joined the Emyzer Nexus workforce. Many of these individuals develop, operate, or maintain high-risk AI systems and have specific training obligations under the EU AI Act. The Phase 2 training policy ensures these obligations are met and evidenced.
- **High-risk AI system operator training compliance:** EU AI Act Article 14 [VERIFY] requires that operators of high-risk AI systems have sufficient AI literacy and training to understand and correctly interpret AI outputs, manage overrides, and report concerns. The Phase 2 training programme delivers and evidences this requirement.
- **Reduces risk from AI misuse by operators:** Operators who do not understand the limitations, failure modes, and appropriate use of AI systems are more likely to act uncritically on incorrect outputs. Structured training reduces this category of operational risk.
- **Demonstrates integrated governance post-acquisition:** A combined and extended training programme that covers both baseline security awareness and AI-specific obligations demonstrates to regulators and clients that Veridian AI has been fully integrated into Emyzer Nexus governance, not siloed as an ungoverned acquisition.

#### Compliance Evidence Required

| # | Evidence Type | System of Record | Owner | Retention Period | Collection Frequency |
|---|---------------|-----------------|-------|-----------------|----------------------|
| 1 | Role-specific AI training records (evidence of completion of AI-specific training modules for all staff in roles that involve developing, operating, or maintaining AI systems, including Veridian AI staff) | LMS | HR Lead + AI Governance Committee | Duration of employment + 3 years | Annual; upon role change; upon new AI system deployment |
| 2 | Operator competency assessments (results of formal competency assessments for operators of high-risk AI systems confirming adequate AI literacy and system-specific understanding) | LMS | HR Lead + AI Governance Committee | Duration of employment + 3 years | Annual; upon assignment to high-risk AI system role |
| 3 | AI awareness training completion records (evidence that all Emyzer Nexus staff (not only AI specialists) have completed the AI awareness training module covering AI risks, responsible AI principles, and reporting obligations) | LMS | HR Lead | Duration of employment + 3 years | Annual |
| 4 | Veridian AI staff integration training records (evidence of completion of Emyzer Nexus security baseline training by all staff joining via the Veridian AI acquisition, including the date of completion relative to integration milestones) | LMS | HR Lead | Duration of employment + 3 years | Per integration cohort; ongoing for new joiners |
| 5 | Training content review records (evidence that AI training content is reviewed and updated when AI systems are significantly changed, retrained, or when regulatory guidance is updated) | GRC Document Repository | CISO + AI Governance Committee | 3 years | Annual; trigger-based |

#### Framework Obligations Satisfied

| Framework | Specific Clause / Control | How Satisfied |
|-----------|--------------------------|---------------|
| EU AI Act (Regulation 2024/1689) [VERIFY] | Article 14 — Human oversight [VERIFY]: Operators shall take appropriate technical and organisational measures to ensure that the natural persons to whom human oversight is assigned have the necessary competence, training, and authority | Operator competency assessments and role-specific AI training programme directly satisfy this requirement |
| EU AI Act (Regulation 2024/1689) [VERIFY] | Article 4 — AI literacy [VERIFY] | AI awareness training programme satisfies the AI literacy obligation for all staff |
| ISO 27001:2022 | A.6.3 — Information security awareness, education and training [VERIFY] | Phase 2 training policy extends Phase 1 obligations to Veridian AI staff |
| ISO/IEC 42001:2023 [VERIFY] | Cl. 7.2 — Competence [VERIFY] | Competency assessment and training records satisfy ISO 42001 competence requirements |
| NIST AI RMF 1.0 | Govern 5.1 — Organisational teams are committed to a culture that considers and communicates AI risk [VERIFY] | AI literacy and awareness training programme operationalises this subcategory |

---

## 5. Compliance Evidence Summary Matrix

This matrix provides a programme-level view of evidence requirements across all 14 policies.

| # | Policy | Total Evidence Types | Primary Systems of Record | Max Retention Period | Annual Evidence Collection Required? |
|---|--------|----------------------|--------------------------|---------------------|--------------------------------------|
| 1 | Information Security Policy | 5 | GRC Repository, LMS, ServiceNow | 7 years | Yes (annual review, annual acknowledgements) |
| 2 | Access Control Policy | 6 | ServiceNow, IAM platform, PAM system, HR System | 7 years | Yes (quarterly access reviews, monthly MFA compliance) |
| 3 | Incident Management Policy | 6 | ServiceNow, Legal Management System, LMS | 7 years | Yes (incident register continuous; annual training) |
| 4 | Risk Management Policy | 6 | ServiceNow, GRC Repository | 7 years | Yes (quarterly risk committee; annual appetite review) |
| 5 | BC/DR Policy | 7 | GRC Repository, ServiceNow, AWS CloudWatch | 7 years | Yes (annual tabletop; semi-annual DR test; annual supplier attestations) |
| 6 | Change Management Policy | 6 | ServiceNow ITSM, CMDB | 7 years | Yes (CAB minutes weekly; change records continuous; emergency change monthly report) |
| 7 | Acceptable Use Policy | 4 | LMS, HR System, CASB | 7 years | Yes (annual acknowledgements; quarterly shadow IT report) |
| 8 | Data Classification Policy | 6 | GRC Repository, ServiceNow, Legal System | 7 years | Yes (annual classification audit; annual data inventory review) |
| 9 | Third-Party Risk Management Policy | 6 | ServiceNow, Legal System, GRC Repository | 7 years | Yes (annual reassessment for Tier 1 suppliers; annual SOC 2 collection) |
| 10 | Security Awareness and Training Policy (Phase 1) | 5 | LMS, SIEM | 3 years | Yes (annual training completion; quarterly phishing simulations) |
| 11 | AI Governance Policy | 6 | ServiceNow, GRC Repository, Legal System | 10 years | Yes (quarterly AI inventory audit; monthly committee meetings; annual conformity review) |
| 12 | Model Risk Policy | 6 | AI monitoring platform, GRC Repository | 7 years | Yes (monthly performance reports; quarterly bias audits for high-risk models) |
| 13 | Privacy and Data Protection Policy | 7 | Legal System, GRC Repository, Consent platform | 7 years | Yes (annual DPIA review; annual RoPA audit; annual DPA review) |
| 14 | Security Awareness and Training Policy (Phase 2 — Nexus) | 5 | LMS, GRC Repository | 3 years | Yes (annual AI training completion; annual competency assessments) |
| **Total** | **14 policies** | **81 evidence types** | **ServiceNow, LMS, GRC Repository, Legal System, IAM/PAM, AI monitoring** | **10 years (AI systems)** | **Yes — all policies require annual evidence collection** |

---

## 6. Audit Readiness Notes

### 6.1 How to Use This Document During an Audit

1. **Identify the framework being audited** (e.g., ISO 27001:2022, GDPR, EU AI Act).
2. **Use Section 7 (Framework Coverage Summary)** to identify which policies address that framework.
3. **Navigate to the relevant policy section** in Sections 3 or 4.
4. **Use the Framework Obligations Satisfied table** to identify the specific clause/control being assessed and the mechanism by which it is satisfied.
5. **Use the Compliance Evidence Required table** to identify the evidence type, its system of record, and its owner. Contact the owner to retrieve current evidence.

### 6.2 Where Evidence Lives

| Evidence Category | Primary Location | Access Contact |
|------------------|-----------------|----------------|
| Policy documents (current versions) | GRC Document Repository | GRC Team |
| Training and acknowledgement records | LMS (Learning Management System) | HR Lead |
| Incident and change records | ServiceNow | IT Operations / CISO |
| Risk register and risk acceptance records | ServiceNow GRC | CISO |
| Legal and regulatory records (DPAs, notifications, contracts) | Legal Management System | Legal Counsel |
| Vendor risk assessments and SOC 2 reports | ServiceNow Vendor Risk Register | Vendor Risk Manager |
| AI governance records (AI inventory, conformity assessments, committee minutes) | ServiceNow GRC + GRC Repository | AI Governance Committee |
| Audit and exercise reports | GRC Document Repository | GRC Team / BC Manager |
| Access and privileged access logs | IAM platform / PAM system | IT Operations |

### 6.3 Demonstrating Completeness to an Auditor

The GRC team maintains an **Evidence Completeness Dashboard** in ServiceNow that tracks:

- Which evidence types are due for collection (based on collection frequency schedules)
- Whether the most recent evidence is within its expected collection window
- Any overdue evidence collections with responsible owner and escalation status

Auditors may request an export of this dashboard as evidence of ongoing compliance monitoring. The dashboard does not replace individual evidence artefacts — it demonstrates the management system's oversight of evidence collection.

### 6.4 Handling Gaps

If an evidence gap is identified during an audit (i.e., required evidence is not available or is outdated):

1. Document the gap in the GRC team's audit log with a timestamp and description.
2. Identify the root cause (missed collection cycle, system failure, ownership gap).
3. Assess the risk impact of the gap (does it represent a control failure or an administrative omission?).
4. Raise a corrective action in ServiceNow with an owner and due date.
5. If the gap relates to a regulatory obligation (e.g., GDPR breach notification records), escalate to Legal Counsel immediately.

---

## 7. Framework Coverage Summary

This table shows which frameworks are addressed by the Emyzer Technology / Emyzer Nexus GRC programme and which policies contribute to each framework.

| Framework | Version | Policies That Address It | Coverage Assessment |
|-----------|---------|--------------------------|---------------------|
| ISO 27001 — Information security management systems | 2022 | All 10 Phase 1 policies (as primary ISMS controls) + Privacy policy (ISO 27701 extension) + Phase 2 policies where applicable | Comprehensive: policy set constitutes the ISMS control framework; certification-ready subject to implementation evidence |
| ISO 22301 — Business continuity management systems | 2019 | BC/DR Policy (primary); Information Security Policy (ISMS scope); Incident Management Policy (incident response interface) | Comprehensive: BIA, BCP, exercise programme, and maintenance requirements fully addressed |
| ISO 31000 — Risk management | 2018 | Risk Management Policy (primary); Information Security Policy (ISMS risk context); Third-Party Risk Management Policy | Substantial: enterprise risk management principles applied to information security and third-party domains |
| ISO/IEC 27701 — Privacy information management | 2019 | Privacy and Data Protection Policy (primary); Data Classification Policy; Third-Party Risk Management Policy | Substantial: controller and processor obligations addressed; extends ISO 27001 ISMS to PIMS |
| ISO/IEC 42001 — AI management systems | 2023 | AI Governance Policy (primary); Model Risk Policy; Security Awareness and Training Policy (Phase 2) | Developing: governance structure and risk management aligned; full certification scope to be confirmed as AI programme matures |
| EU AI Act (Regulation 2024/1689) | 2024 [VERIFY] | AI Governance Policy (primary); Model Risk Policy; Privacy and Data Protection Policy; Security Awareness and Training Policy (Phase 2) | Developing: governance obligations addressed; technical conformity of specific AI systems requires ongoing assessment per system classification |
| NIST Cybersecurity Framework | 2.0 | Information Security Policy; Risk Management Policy; Access Control Policy; Incident Management Policy; BC/DR Policy; Change Management Policy; Security Awareness and Training Policy | Comprehensive: Govern, Identify, Protect, Detect, Respond, and Recover functions addressed across the policy set |
| NIST AI Risk Management Framework | 1.0 | AI Governance Policy (primary); Model Risk Policy; Security Awareness and Training Policy (Phase 2) | Substantial: Govern, Map, Measure, and Manage functions addressed; ongoing maturation as AI programme develops |
| GDPR (EU) | 2016/679 [VERIFY] | Privacy and Data Protection Policy (primary); Data Classification Policy; Incident Management Policy; Access Control Policy; Third-Party Risk Management Policy; Security Awareness and Training Policy | Comprehensive: controller obligations, processing principles, data subject rights, breach notification, and processor management addressed |
| UK GDPR | UK Data Protection Act 2018 [VERIFY] | Privacy and Data Protection Policy (dual-scope); Data Classification Policy; Incident Management Policy | Substantial: dual EU/UK compliance approach documented in Privacy Policy; ICO as lead supervisory authority for UK operations |
| ITIL 4 | Current | Change Management and Configuration Policy (primary); Incident Management Policy (incident management practice interface) | Partial: change enablement practice fully aligned; service management practices referenced where relevant |
| PCI DSS | v4.0 | Access Control Policy; Security Awareness and Training Policy; Data Classification Policy | Partial: cardholder data environment controls in scope; full PCI DSS compliance requires additional payment-specific controls outside this policy set |
| NIST SP 800-53 | Rev. 5 | Access Control Policy; Incident Management Policy; Risk Management Policy; Security Awareness and Training Policy; Change Management Policy | Substantial: core security control families addressed; full 800-53 baseline requires control-by-control mapping beyond this policy set |

---

## 8. Document Control

| Attribute | Value |
|-----------|-------|
| **Document ID** | COMP-MAP-001 |
| **Version** | 2.0 |
| **Status** | Active |
| **Classification** | Internal |
| **Owner** | GRC Team |
| **Approved By** | Chief Information Security Officer |
| **Phase 1 Effective Date** | 2024-07-01 |
| **Phase 2 Additions Effective** | 2025-07-01 |
| **Next Review** | 2026-07-01 |
| **Storage Location** | GRC Document Repository |

### Approval History

| Version | Date | Author | Changes | Approved By | Approval Date |
|---------|------|--------|---------|-------------|---------------|
| 1.0 | 2024-07-01 | GRC Team | Initial version — Phase 1 policies (10 policies; Emyzer Technology) | CISO | 2024-07-01 |
| 2.0 | 2025-07-01 | GRC Team | Phase 2 additions — 4 Emyzer Nexus policies; updated Evidence Summary Matrix and Framework Coverage Summary | CISO | 2025-07-01 |

---

*COMP-MAP-001 v2.0 | Emyzer Technology / Emyzer Nexus | GRC Programme | 2025-07-01*

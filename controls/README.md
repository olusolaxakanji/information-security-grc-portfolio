# Controls Library

**Emyzer Technology: Phase 1 | Fictional case study.**

> All entities, systems, and control records are invented for professional demonstration purposes. Framework references are accurate as of the document dates.

---

## What the Controls Layer Does

Policies define requirements. Controls are what you test to prove those requirements are being met.

A policy can say "access to systems shall be reviewed quarterly." That requirement is unverifiable without a control that defines who performs the review, what evidence is produced, when it runs, what a pass looks like, and what happens when the test fails. The controls library is that layer: the operational bridge between governance requirements and audit evidence.

Every control in this library links to its governing policy, names its owner, defines its testing procedure, specifies its cadence, and records its current status. Together they form the testable evidence layer beneath the policy framework.

---

## Control Index

| Control ID | Control | Governing Policy | Cadence |
|---|---|---|---|
| [ET-CTRL-001](et-ctrl-001-access-control-review.md) | Access Control Review and Certification | [Access Control Policy](../policies/access-control-policy.md) | Quarterly |
| [ET-CTRL-002](et-ctrl-002-incident-detection-response.md) | Incident Detection and Response | [Incident Management Policy](../policies/incident-management-policy.md) | Continuous / Event-driven |
| [ET-CTRL-003](et-ctrl-003-change-advisory-board-review.md) | Change Advisory Board Review | [Change Management and Configuration Policy](../policies/change-management-and-configuration-policy.md) | Per change request |
| [ET-CTRL-004](et-ctrl-004-third-party-vendor-risk-assessment.md) | Third-Party Vendor Risk Assessment | [Third-Party Risk Management Policy](../policies/third-party-risk-management-policy.md) | Annual / At onboarding |
| [ET-CTRL-005](et-ctrl-005-data-classification-audit.md) | Data Classification Audit | [Data Classification Policy](../policies/data-classification-policy.md) | Annual |
| [ET-CTRL-006](et-ctrl-006-security-awareness-training-completion.md) | Security Awareness Training Completion | [Security Awareness and Training Policy](../policies/security-awareness-and-training-policy.md) | Annual |
| [ET-CTRL-007](et-ctrl-007-business-continuity-dr-testing.md) | Business Continuity and DR Testing | [BC/DR Policy](../policies/bcdr-policy.md) | Annual |
| [ET-CTRL-008](et-ctrl-008-ai-system-inventory-classification-review.md) | AI System Inventory and Risk Classification Review | [AI Governance Policy](../enterprise-policies/ai-governance-policy.md) | Quarterly |

**ET-CTRL-008** is a Nexus-level control covering both Phase 1 and Phase 2 scope. It operationalises the AI Governance Committee's quarterly review obligation for AI system classification status and risk posture. It retains the ET-CTRL prefix for portfolio consistency.

---

## Control ID Convention

All Emyzer Technology controls use the format `ET-CTRL-NNN`:
- `ET`: Emyzer Technology entity identifier
- `CTRL`: document type indicator
- `NNN`: sequential three-digit number

---

## What Each Control Record Contains

Each control document specifies:

- **Control objective:** The specific policy requirement this control tests
- **Control type:** Preventive, Detective, or Corrective
- **Testing procedure:** Step-by-step instructions for performing the test
- **Evidence required:** What records must be produced to demonstrate the control operated
- **Pass/fail criteria:** The specific condition that determines whether the control is effective
- **Cadence and owner:** When the test runs and who is accountable for results
- **Remediation path:** What happens if the test fails

---

## Framework Alignment

| Framework | Controls |
|---|---|
| ISO 27001:2022 | ET-CTRL-001 through ET-CTRL-007 |
| NIST CSF 2.0 | ET-CTRL-001, ET-CTRL-002, ET-CTRL-004, ET-CTRL-006 |
| NIST SP 800-53 Rev. 5 | ET-CTRL-001, ET-CTRL-002, ET-CTRL-003, ET-CTRL-004 |
| ISO 22301:2019 | ET-CTRL-007 |
| EU AI Act (Regulation 2024/1689) | ET-CTRL-008 |
| NIST AI RMF 1.0 | ET-CTRL-008 |
| ISO/IEC 42001:2023 | ET-CTRL-008 |
| GDPR | ET-CTRL-002, ET-CTRL-005 |

---

## Related Documentation

| Document | Description |
|---|---|
| [Emyzer Technology Overview](../emyzer-technology/README.md) | Phase 1 programme context |
| [Policies](../policies/README.md) | The 10 Phase 1 policies these controls operationalise |
| [ServiceNow Evidence](../servicenow-evidence/README.md) | Platform exports showing policies in the GRC system these controls run against |
| [Portfolio Overview](../README.md) | Top-level narrative and 60-second review path |

---

*All content in this portfolio is a fictional case study. Framework and regulatory references are accurate as of the document publication dates.*

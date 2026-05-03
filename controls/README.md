# Controls

This directory contains the Emyzer Technology information security control framework. Each control operationalises one or more published policies and defines the specific procedure used to demonstrate compliance.

---

## Document Index

| Document | Description |
|---|---|
| [control-index.md](control-index.md) | Master list of all controls — authoritative reference for IDs, owners, types, frequencies, and status |
| [et-ctrl-001-access-control-review.md](et-ctrl-001-access-control-review.md) | Access Control Review and Certification |
| [et-ctrl-002-incident-detection-response.md](et-ctrl-002-incident-detection-response.md) | Incident Detection and Response |
| [et-ctrl-003-change-advisory-board-review.md](et-ctrl-003-change-advisory-board-review.md) | Change Advisory Board (CAB) Review |
| [et-ctrl-004-third-party-vendor-risk-assessment.md](et-ctrl-004-third-party-vendor-risk-assessment.md) | Third-Party Vendor Risk Assessment |
| [et-ctrl-005-data-classification-audit.md](et-ctrl-005-data-classification-audit.md) | Data Classification Audit |
| [et-ctrl-006-security-awareness-training-completion.md](et-ctrl-006-security-awareness-training-completion.md) | Security Awareness Training Completion |
| [et-ctrl-007-business-continuity-dr-testing.md](et-ctrl-007-business-continuity-dr-testing.md) | Business Continuity and DR Testing |
| [et-ctrl-008-ai-system-inventory-classification-review.md](et-ctrl-008-ai-system-inventory-classification-review.md) | AI System Inventory and Risk Classification Review |

---

## Control ID Convention

All Emyzer Technology controls use the format `ET-CTRL-NNN`:

- `ET` — Emyzer Technology entity identifier
- `CTRL` — document type: control record
- `NNN` — sequential three-digit number

Controls scoped to Emyzer Nexus as the parent entity (e.g., ET-CTRL-008) retain the `ET-CTRL` prefix for this portfolio but are noted as Nexus-level in their entity field.

---

## Policy Mapping

| Control | Governing Policy |
|---|---|
| ET-CTRL-001 | [Access Control Policy](../policies/access-control-policy.md) |
| ET-CTRL-002 | [Incident Management Policy](../policies/incident-management-policy.md) |
| ET-CTRL-003 | [Change Management and Configuration Policy](../policies/change-management-and-configuration-policy.md) |
| ET-CTRL-004 | [Third-Party Risk Management Policy](../policies/third-party-risk-management-policy.md) |
| ET-CTRL-005 | [Data Classification Policy](../policies/data-classification-policy.md) |
| ET-CTRL-006 | [Security Awareness and Training Policy](../policies/security-awareness-and-training-policy.md) |
| ET-CTRL-007 | [Business Continuity and DR Policy](../policies/bcdr-policy.md) |
| ET-CTRL-008 | [AI Governance Policy](../enterprise-policies/ai-governance-policy.md) |

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

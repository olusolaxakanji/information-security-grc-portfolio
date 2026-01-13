# Information Security Policies

**Enterprise security policies for Emyzer Technology, developed in ServiceNow GRC and aligned with NIST, ISO 27001, COBIT, and COSO ERM frameworks.**

---

## Quick Navigation

| Priority | Policy | Why Start Here |
|----------|--------|----------------|
| ⭐ Start Here | [Information Security Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/information-security-policy.md) | Parent policy with full evidence index, exception handling, and control cadence |

---

## Policy Index

### Flagship Policy

| Policy | Description | Framework Alignment | Status |
|--------|-------------|---------------------|--------|
| ⭐ [Information Security Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/information-security-policy.md) | Defines security program structure, governance roles, responsibilities, exception handling, and strategic direction | NIST CSF GV, ISO 27001 A.5, COBIT EDM, ITIL | **Flagship-Ready** |
| ⭐ [Access Control Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/access-control-policy.md) | Governs user authentication, authorization, and access management based on least privilege and role-based access principles | NIST CSF PR.AC, ISO 27001 A.5.15-A.5.18, COBIT DSS05 | **Flagship-Ready** |

### Completed Policies (Upgrades In Progress)

These policies are complete and functional. Quality upgrades are underway to add evidence indexes, exception-handling sections, and control-cadence documentation, consistent with the flagship policy.

| Policy | Description | Framework Alignment | Status |
|--------|-------------|---------------------|--------|
| ✅ [Incident Management Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/incident-management-policy.md) | Defines procedures for detecting, responding to, and recovering from security incidents with GDPR breach notification compliance | NIST CSF RS, ISO/IEC 27035, NIST SP 800-61, GDPR Art. 33-34 | Upgrade Pending |
| ✅ [Risk Management Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/risk-management-policy.md) | Establishes framework for identifying, assessing, and mitigating organizational risks across all business functions | NIST SP 800-37 RMF, COSO ERM, CIS RAM, ISO 31000 | Upgrade Pending |
| ✅ [Business Continuity and Disaster Recovery Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/bcdr-policy.md) | Ensures organizational preparedness to respond to and recover from disruptions through defined recovery objectives | ISO 22301, ISO/IEC 27031, BCI GPG, NIST SP 800-34 | Upgrade Pending |

### Planned Policies

| Policy | Description | Framework Alignment | Status |
|--------|-------------|---------------------|--------|
| 📋 Change Management & Configuration Policy | Controls modifications to systems and configurations to maintain security and operational stability | ITIL, ISO 20000, COBIT BAI06, NIST SP 800-128 | Planned |
| 📋 Acceptable Use Policy | Establishes appropriate use of organizational systems, networks, and resources by all personnel | NIST CSF PR.AT, ISO 27001 A.5.10, SANS AUP | Planned |
| 📋 Data Classification Policy | Defines data sensitivity levels, labeling requirements, and handling procedures throughout the data lifecycle | NIST CSF PR.DS, ISO 27001 A.5.12-A.5.13, NIST SP 800-60 | Planned |
| 📋 Third-Party/Vendor Risk Management Policy | Manages third-party risk through security requirements, assessments, and ongoing monitoring | NIST SP 800-161, ISO 27036, NIST CSF ID.SC | Planned |
| 📋 Security Awareness & Training Policy | Establishes requirements for security education, training, and awareness programs | NIST CSF PR.AT, ISO 27001 A.6.3, NIST SP 800-50 | Planned |

---

## Policy Structure

All policies follow a consistent structure aligned with GRC best practices and audit expectations:

| Section | Purpose |
|---------|---------|
| **Document Control** | Ownership, versioning, classification, review schedules |
| **Purpose and Scope** | Policy intent, applicability, and boundaries |
| **Policy Statement** | Core requirements and enforceable provisions |
| **Roles and Responsibilities** | Accountability assignments and separation of duties |
| **Procedures** | Implementation guidance and operational workflows |
| **Compliance and Enforcement** | Monitoring mechanisms and consequences for non-compliance |
| **Framework Alignment** | Mapping to recognized security standards |
| **Organizational Benefits** | Business value and risk reduction articulation |
| **Evidence of Compliance** | Audit trail requirements and documentation cadence |

### Flagship Policy Additions

The Information Security Policy (flagship) includes additional governance sections being rolled out to other policies:

- **Policy Snapshot** — Executive-level summary of scope, governance, and evidence
- **Evidence Index** — System of record, owner, and retention for each evidence type
- **Policy Exceptions** — Approval workflow, duration limits, and quarterly review process
- **Control Cadence** — Frequency of reviews, audits, and attestations

---

## Framework Coverage

These policies collectively address requirements from:

### NIST Cybersecurity Framework v1.1

| Function | Coverage |
|----------|----------|
| **Identify (ID)** | Asset management, risk assessment, governance |
| **Protect (PR)** | Access control, data security, protective technology |
| **Detect (DE)** | Security monitoring and event detection |
| **Respond (RS)** | Incident response planning and communications |
| **Recover (RC)** | Recovery planning and improvements |

### ISO/IEC 27001:2022

| Control Category | Coverage |
|------------------|----------|
| **Organizational controls (A.5)** | Information security policies, roles, asset management |
| **People controls (A.6)** | Screening, awareness, disciplinary process |
| **Physical controls (A.7)** | Physical security and environmental controls |
| **Technological controls (A.8)** | Access control, cryptography, logging |

### Additional Frameworks

| Framework | Application |
|-----------|-------------|
| **NIST RMF** | Prepare, Categorize, Select, Implement, Assess, Authorize, Monitor |
| **COSO ERM** | Governance, Strategy, Performance, Review |
| **ISO 22301** | Business impact analysis, continuity planning, testing |

---

## ServiceNow GRC Implementation

All policies were created and managed within the ServiceNow GRC platform:

| Capability | Demonstration |
|------------|---------------|
| Policy lifecycle management | Draft → Review → Approval → Publication |
| Version control | Change tracking with documented history |
| Approval workflows | Documented approvers and reviewers |
| Knowledge base integration | Organizational accessibility |
| Compliance scoring | Audit readiness capabilities |

See [`servicenow-evidence/`](https://github.com/olusolaxakanji/information-security-grc-portfolio/tree/main/servicenow-evidence) for platform screenshots and implementation artifacts.

---

## Related Documentation

| Resource | Description |
|----------|-------------|
| [`compliance-mapping/`](https://github.com/olusolaxakanji/information-security-grc-portfolio/tree/main/compliance-mapping) | Framework control mappings and gap analyses |
| [`business-continuity/`](https://github.com/olusolaxakanji/information-security-grc-portfolio/tree/main/business-continuity) | ISO 22301 BCMS documentation |
| [`risk-assessments/`](https://github.com/olusolaxakanji/information-security-grc-portfolio/tree/main/risk-assessments) | Risk registers and treatment plans |
| [`servicenow-evidence/`](https://github.com/olusolaxakanji/information-security-grc-portfolio/tree/main/servicenow-evidence) | Platform implementation artifacts |

---

## Policy Maintenance

| Process | Details |
|---------|---------|
| **Review Cycle** | Annual, or when significant organizational changes occur |
| **Change Process** | Risk assessment → Stakeholder review → Approval → Communication → Training |
| **Version Control** | Document history table in each policy |

---

## Contact

| Role | Contact |
|------|---------|
| Information Security Officer | security@emyzertech.com |
| Chief Risk Officer | risk@emyzertech.com |
| GRC Program Manager | grc@emyzertech.com |

---

*Last Updated: January 2025*

# GRC Document Templates

**Emyzer Technology – ServiceNow GRC Portfolio**

---

## Overview

This folder contains reusable templates for governance, risk, and compliance documentation. Each template mirrors the structure of documents generated from ServiceNow GRC and aligns with industry frameworks, including NIST, ISO 27001, SOC 2, and COBIT.

These templates represent the three core pillars of GRC work:

| Template | GRC Function | Purpose |
|----------|--------------|---------|
| **Policy Template** | Governance | Establish organizational requirements and standards |
| **Risk Assessment Template** | Risk | Identify, evaluate, and treat information security risks |
| **Control Testing Template** | Compliance | Verify controls are designed and operating effectively |

---

## Templates Included

### 1. Policy Template ([policy-template.md](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/templates/policy-template.md))

A comprehensive framework for creating information security policies that includes:

- Metadata fields compatible with ServiceNow GRC
- Standardized sections (Purpose, Scope, Definitions, Policy Statement, Roles, Procedures)
- Compliance and monitoring requirements
- Framework alignment mapping (NIST, ISO 27001, COBIT, CSF)
- Organizational benefits documentation
- Evidence of compliance matrix

**Use for:** Access Control, Incident Response, Risk Management, Data Classification, Acceptable Use, and other security policies.

---

### 2. Risk Assessment Template ([risk-assessment-template.md](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/templates/risk-assessment-template.md))

A structured approach to risk identification and treatment that includes:

- 5x5 risk matrix with likelihood and impact scales
- Asset inventory and threat/vulnerability identification
- Risk register with inherent and residual risk scoring
- Treatment plan with strategy definitions (Mitigate, Transfer, Accept, Avoid)
- Risk summary dashboard
- Framework alignment (NIST 800-30, ISO 31000, FAIR)

**Use for:** Annual risk assessments, project-based assessments, third-party risk evaluations, and compliance-driven risk analysis.

---

### 3. Control Testing Template ([control-testing-template.md](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/templates/control-testing-template.md))

A detailed workbook for testing control design and operating effectiveness that includes:

- Control testing summary matrix
- Detailed workpaper structure for each control
- Evidence inventory with traceability
- Findings and remediation tracker
- Severity definitions and remediation timelines
- Framework mapping (SOC 2, ISO 27001, NIST 800-53, PCI DSS)

**Use for:** Internal control testing, audit preparation, SOC 2 readiness, ISO 27001 certification support, and continuous compliance monitoring.

---

## How to Use These Templates

1. **Copy the template** to your working directory
2. **Rename the file** following your naming convention (e.g., `access-control-policy.md`)
3. **Replace all bracketed placeholders** `[text]` with your specific content
4. **Customize sections** as needed for your organization's requirements
5. **Remove the "Template Usage Notes" section** at the bottom before publishing
6. **Update framework mappings** to reflect your compliance scope

---

## Naming Conventions

| Document Type | Format | Example |
|---------------|--------|---------|
| Policies | `[policy-name]-policy.md` | `access-control-policy.md` |
| Risk Assessments | `[scope]-risk-assessment-[YYYY].md` | `enterprise-risk-assessment-2024.md` |
| Control Testing | `[framework]-control-testing-[period].md` | `soc2-control-testing-q4-2024.md` |

---

## Framework Coverage

These templates support alignment with:

| Framework | Templates |
|-----------|-----------|
| **NIST SP 800-53 Rev. 5** | Policy, Risk Assessment, Control Testing |
| **NIST Cybersecurity Framework** | Policy, Risk Assessment, Control Testing |
| **NIST SP 800-30** | Risk Assessment |
| **ISO/IEC 27001:2022** | Policy, Control Testing |
| **ISO/IEC 27005:2022** | Risk Assessment |
| **ISO 31000:2018** | Risk Assessment |
| **SOC 2 (AICPA TSC)** | Policy, Control Testing |
| **COBIT 2019** | Policy, Risk Assessment, Control Testing |
| **PCI DSS 4.0** | Control Testing |
| **FAIR** | Risk Assessment |

---

## ServiceNow GRC Integration

These templates are designed for compatibility with ServiceNow GRC modules:

| Template | ServiceNow Module | Key Tables |
|----------|-------------------|------------|
| Policy | Policy & Compliance | `sn_compliance_policy`, `sn_compliance_control` |
| Risk Assessment | Risk Management | `sn_risk_risk`, `sn_risk_assessment`, `sn_risk_response_task` |
| Control Testing | Audit Management | `sn_audit_test_plan`, `sn_audit_test_result`, `sn_audit_finding` |

---

## Related Documentation

- [Main README](../README.md) – Project overview and repository structure
- [Access Control Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/access-control-policy.md) – Example policy using this template

---

## Version History

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 1.0 | [YYYY-MM-DD] | [Your Name] | Initial template release |

---

*These templates were developed as part of a ServiceNow GRC portfolio project demonstrating governance, risk, and compliance capabilities aligned with industry frameworks.*

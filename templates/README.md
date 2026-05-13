# GRC Document Templates

**Emyzer Technology: Phase 1 | Fictional case study.**

---

## Why Templates Exist in a GRC Programme

Consistency is the foundation of audit readiness. If every risk assessment uses a different structure, different field names, and different scoring criteria, it is impossible to compare risk entries, aggregate findings, or demonstrate that the programme operates systematically. Templates solve that problem by establishing the structure before the work begins.

These three templates produce the three core document types used across the Emyzer Technology programme: governance policies, risk assessments, and control testing workpapers. Every substantive document in the portfolio was produced from one of them.

---

## Templates

### [Policy Template](policy-template.md)

The structure every Phase 1 and Phase 2 policy was built from. Using a common template ensures consistent metadata fields, accountability structures, and evidence indexes across all 14 policies in the programme.

**What it includes:** Policy metadata (owner, version, validity dates, approver, knowledge base reference), purpose and scope, definitions, policy statement with "shall" language and defined SLAs, roles and responsibilities with named accountability, minimum security requirements, compliance and monitoring provisions, exception handling workflow, cross-policy references, evidence index with system of record and retention periods, framework alignment table, and approval history.

**The evidence index section is the most important part.** It specifies, for every evidence type the policy requires, which system holds the record, who owns it, and how long it must be retained. Without this section, compliance is asserted but not demonstrable.

**Compatible with ServiceNow GRC:** Metadata fields map directly to ServiceNow Policy and Compliance module fields.

### [Risk Assessment Template](risk-assessment-template.md)

The structure every risk assessment in the programme was built from, including the Phase 2 AI system risk assessments which extend it with AI-specific categories.

**What it includes:** Asset inventory and scope definition, threat and vulnerability identification, 5x5 risk matrix with likelihood and impact scales, inherent and residual risk scoring, treatment plan with strategy definitions (Mitigate, Transfer, Accept, Avoid), risk register fields, and framework alignment section.

**The inherent/residual distinction matters.** Documenting both ratings is what allows the programme to show what controls are doing: the gap between inherent and residual is the demonstrated value of each control. Documenting only one rating produces a register that cannot answer "what would happen without these controls."

**Frameworks:** NIST SP 800-30 Rev. 1, ISO 27005, ISO 31000:2018, FAIR

### [Control Testing Template](control-testing-template.md)

The workpaper structure for testing whether controls are designed and operating effectively. Used in internal control testing, audit preparation, and continuous compliance monitoring.

**What it includes:** Control testing summary matrix, individual workpaper structure (control objective, test procedure, evidence inspected, results, findings), evidence inventory with traceability, findings and remediation tracker with severity definitions and remediation timelines, and framework mapping.

**The evidence traceability section is what connects testing to audit.** Each evidence item is linked to the control it supports and the test result it contributed to. An auditor can follow the chain from a control objective to the specific evidence examined to the conclusion reached.

**Frameworks:** SOC 2 (AICPA TSC), ISO 27001:2022, NIST SP 800-53 Rev. 5, PCI DSS

---

## ServiceNow Compatibility

Each template maps to the corresponding ServiceNow GRC module:

| Template | ServiceNow Module | Primary Tables |
|---|---|---|
| Policy Template | Policy and Compliance | `sn_compliance_policy`, `sn_compliance_control` |
| Risk Assessment Template | Risk Management | `sn_risk_risk`, `sn_risk_assessment`, `sn_risk_response_task` |
| Control Testing Template | Audit Management | `sn_audit_test_plan`, `sn_audit_test_result`, `sn_audit_finding` |

---

## How to Use

Copy the relevant template, rename it following the programme naming convention, replace all bracketed placeholders with content specific to the document's scope, and remove the template usage notes section before publishing. Framework alignment sections should be updated to reflect the compliance scope of the specific document.

---

## Related Documentation

| Document | Description |
|---|---|
| [Controls Library](../controls/README.md) | Control records produced using the control testing template structure |
| [Risk Assessments](../risk-assessments/README.md) | Risk documents produced using the risk assessment template |
| [Policies](../policies/README.md) | Policies produced using the policy template |
| [Portfolio Overview](../README.md) | Top-level narrative and 60-second review path |

---

*All content in this portfolio is a fictional case study. Framework references are accurate as of the document publication dates.*

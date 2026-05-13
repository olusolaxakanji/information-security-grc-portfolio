# Information Security Policies

**Emyzer Technology: Phase 1 | Fictional case study.**

> All entities, systems, personnel, and scenarios are invented for professional demonstration purposes. Framework references are accurate as of the document dates.

---

## What This Directory Contains

Ten core information security policies developed for Emyzer Technology and implemented in ServiceNow GRC. These are the Phase 1 foundation that Phase 2 depends on. When Emyzer Technology acquired Veridian AI, these policies applied to the acquired entity from Day 0 and were extended, not replaced, by the four Phase 2 enterprise policies.

---

## Policy Index

| Policy | Key design decision | Frameworks |
|---|---|---|
| [Information Security Policy](information-security-policy.md) | ISMS parent policy. Establishes the Security Steering Committee as the exception escalation authority and defines the review cadence all other policies inherit. The scope explicitly includes Emyzer Technology subsidiaries and acquired entities: governance obligations travel with acquisitions from Day 0. | ISO 27001:2022, NIST CSF 2.0, COBIT |
| [Access Control Policy](access-control-policy.md) | Role-based access with privileged access controls and quarterly review for high-privilege accounts. At Phase 2, the AI Governance Committee is added as an access authority for AI system records, and model operator access provisioning is linked to training completion under the Tier 2 Training Policy. | NIST SP 800-53 Rev. 5, ISO 27001:2022 A.5.15-A.5.18, COBIT DSS05 |
| [Incident Management Policy](incident-management-policy.md) | IRT activation criteria are defined at incident classification, not at escalation. This design prevents the assessment delay that causes organizations to miss the 72-hour GDPR notification window. A 4-hour initial assessment SLA reinforces the timeline. At Phase 2, the AI Governance Policy extends this policy with AI-specific failure modes and EU AI Act Article 73 serious incident reporting obligations. | NIST SP 800-61, ISO 27035, GDPR Art. 33-34 |
| [Risk Management Policy](risk-management-policy.md) | Establishes the 5x5 hybrid scoring matrix applied across all Phase 1 and Phase 2 risk assessments. Defines the materiality threshold above which Risk Management Committee formal acceptance is required. AI-specific risk categories (model drift, training data bias, third-party model dependency) are defined as distinct register entries, not subsets of operational risk. | ISO 31000:2018, NIST CSF 2.0, COSO ERM |
| [BC/DR Policy](bcdr-policy.md) | Recovery objectives are derived from a 42-stakeholder BIA with financial exposure quantification across 12 critical processes, not estimated. RTO and RPO targets are tiered by process class. At Phase 2, AI system availability is treated as a distinct continuity risk with documented fallback procedures for PCM-001 and CRT-001. | ISO 22301:2019, NIST SP 800-34 |
| [Change Management and Configuration Policy](change-management-and-configuration-policy.md) | Three-tier change classification with defined CAB authority limits. Emergency change provisions include AI-specific guidance for rapid model suspension decisions. At Phase 2, AI system material changes escalate to the AI Governance Committee rather than standard CAB review, using the material change definition consistent across both policies. | ITIL 4, ISO 27001:2022, COBIT BAI06 |
| [Acceptable Use Policy](acceptable-use-policy.md) | Covers personal device use, shadow IT, and staff use of AI tools. Generative AI use provisions prohibit inputting Confidential or Restricted data into external LLM APIs without AI Governance Committee-approved data handling controls. Shadow AI reporting obligations align with the AI Governance Policy's annual inventory audit. | ISO 27001:2022 A.5.10, NIST CSF |
| [Data Classification Policy](data-classification-policy.md) | Four-tier classification (Public, Internal, Confidential, Restricted) with handling, labeling, and disposal requirements per tier. At Phase 2, AI training data is classified under this scheme with additional GDPR controls applied via the Privacy and Data Protection Policy. Model artefacts and AI system outputs are classified at minimum as Confidential. | NIST SP 800-60, ISO 27001:2022 A.5.12-A.5.13, GDPR |
| [Third-Party Risk Management Policy](third-party-risk-management-policy.md) | Risk tiering criteria for vendors with review cadences by tier. At Phase 2, extended by the AI Vendor Risk Due Diligence Addendum, a subordinate document rather than a policy amendment, covering model transparency, training data provenance, bias audit availability, and contractual liability for model errors. Structured as a subordinate document so it can be updated as EU AI Act implementing acts develop without a full policy revision cycle. | ISO 27036, NIST SP 800-161, NIST CSF ID.SC |
| [Security Awareness and Training Policy](security-awareness-and-training-policy.md) | Completion tracking and role-based curriculum requirements. At Phase 2, a Tier 2 policy adds EU AI Act Article 14 human oversight training obligations for staff interacting with High-Risk AI systems. Training completion is a prerequisite for model operator access provisioning under the Access Control Policy. | ISO 27001:2022 A.6.3, NIST SP 800-50 |

---

## Policy Structure

Every policy in this directory follows a consistent structure derived from the policy template:

| Section | Purpose |
|---|---|
| Policy metadata | Owner, version, validity dates, knowledge base reference, approval chain |
| Purpose and scope | Policy intent, applicability, third-party requirements |
| Definitions | Key terminology defined consistently across the framework |
| Policy statement | Core requirements with "shall" language and defined SLAs |
| Roles and responsibilities | Named accountability assignments |
| Minimum security requirements | Operational controls and implementation specifications |
| Compliance and monitoring | Monitoring mechanisms and non-compliance consequences |
| Policy exceptions | Approval workflow, duration limits, compensating controls |
| Evidence index | System of record, owner, and retention period for every evidence type required |
| Framework alignment | Control mapping to relevant standards |

The evidence index is the most operationally important section. It specifies exactly what records must exist, where they live, and how long they must be retained. Without this section, compliance is asserted but not demonstrable.

---

## ServiceNow Implementation

All 10 policies were built and managed in ServiceNow GRC. Platform exports for five policies are in [/servicenow-evidence/](../servicenow-evidence/): raw PDFs showing ownership, approval workflows, and compliance mappings as generated by the platform.

---

## Related Documentation

| Document | Description |
|---|---|
| [Emyzer Technology Overview](../emyzer-technology/README.md) | Phase 1 programme context |
| [Enterprise Policies](../enterprise-policies/readme.md) | Phase 2 policies extending this Phase 1 foundation |
| [Controls Library](../controls/README.md) | The operational controls that test these policy requirements |
| [ServiceNow Evidence](../servicenow-evidence/README.md) | Platform exports for 5 of these policies |
| [Portfolio Overview](../README.md) | Top-level narrative and 60-second review path |

---

*All content in this portfolio is a fictional case study. Framework and regulatory references are accurate as of the document publication dates.*

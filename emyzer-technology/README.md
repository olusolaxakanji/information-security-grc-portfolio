# Emyzer Technology — GRC Programme Overview

**Phase 1 Entity | Information Security GRC Portfolio**

---

> **Simulated Environment**
>
> Emyzer Technology is a fictional organisation created for this GRC portfolio. All entities, personnel, systems, policies, risk entries, and regulatory scenarios are invented. Framework references (ISO 27001:2022, NIST CSF, EU AI Act, GDPR, and others) are accurate as of the document dates; their application to Emyzer Technology is illustrative. No real organisation, individual, or incident is represented.

---

## About Emyzer Technology

Emyzer Technology is a fictional multinational technology company operating across Asia, the Americas, Africa, and parts of Europe and the Middle East, with a workforce of approximately 5,000 staff. The organisation's business lines span four functional areas:

| Business Function | Description |
|---|---|
| **Hardware and device production** | Consumer and enterprise laptop manufacturing for regional markets |
| **Cloud service management** | Managed cloud infrastructure and platform services for enterprise clients |
| **Enterprise technical support** | Tier 1–3 support services covering hardware, software, and systems |
| **Global security implementation** | Security programme delivery and managed security services for client environments |

**GRC maturity stage at Phase 1:** Foundational. 10 core information security policies, a structured risk assessment programme, business continuity documentation, and full ServiceNow GRC implementation, all established before the Veridian AI acquisition.

---

## Position in the Corporate Structure

Emyzer Technology is a subsidiary of Emyzer Nexus, the post-acquisition parent entity formed following the acquisition of Veridian AI in 2024. All Phase 1 documentation developed for Emyzer Technology remains in effect as subsidiary governance under the policy hierarchy to be established in the M&A GRC Integration Charter.

```
Emyzer Nexus  (parent — Phase 2)
├── Emyzer Technology  (subsidiary — Phase 1 GRC programme, this folder)
└── Veridian AI  (acquired — AI systems under governance integration)
```

**Phase 1** covers the period before acquisition: the GRC programme built for Emyzer Technology as a standalone entity.

**Phase 2** covers the post-acquisition period: the expanded governance obligations of Emyzer Nexus as parent, including AI governance under the EU AI Act and M&A integration management.

For parent-level governance documentation, see [`emyzer-nexus/README.md`](../emyzer-nexus/readme.md). For Veridian AI inherited AI system governance, see the [AI Governance Programme](#ai-governance-programme--phase-2) section below.

---

## Governance Bodies and Accountable Roles

The following roles and governance bodies are referenced across Emyzer Technology's GRC documentation. All named individuals are fictional.

| Role / Body | Function | Referenced In |
|---|---|---|
| **Chief Information Security Officer (CISO)** | Executive sponsor of the ISMS; final approver on all security policies; chairs the AI Governance Committee at Nexus level | All Phase 1 and Phase 2 security policies |
| **Information Security Officer (ISO)** | ISMS operational ownership; responsible for policy drafting, exception approval, and day-to-day compliance monitoring. *Named: Susan Orwell* | Information Security Policy, Access Control Policy, Incident Management Policy, Change Management Policy, Acceptable Use Policy, Data Classification Policy, Third-Party Risk Management Policy, Security Awareness and Training Policy |
| **Chief Risk Officer (CRO)** | Enterprise risk register owner; risk appetite governance; business continuity oversight. *Named: Susan Orwell* | Risk Management Policy, Business Continuity and DR Policy, Third-Party Risk Management Policy, Model Risk Policy |
| **Data Protection Officer (DPO)** | Privacy programme ownership; GDPR and UK GDPR obligations; Data Protection Impact Assessment governance | Privacy and Data Protection Policy |
| **Chief Technology Officer (CTO)** | IT governance authority; change management programme ownership; vulnerability management oversight | Change Management and Configuration Policy |
| **Business Continuity Manager** | BC/DR programme ownership; Business Impact Analysis oversight; tabletop exercise coordination. *Named: Susan Orwell* | Business Continuity and DR Policy, Business Impact Analysis Report |
| **GRC Analyst** | Policy document reviewer; framework alignment verification; evidence register maintenance and spot-checks | All policies (reviewer role) |
| **Security Steering Committee** | Cross-functional ISMS governance body; exception escalation authority; programme performance oversight | Information Security Policy |
| **Risk Management Committee** | Risk escalation and formal acceptance authority; approves treatment decisions above defined materiality thresholds; receives budget-blocked risk escalations | Risk Management Policy, Asset Risk Register |
| **Change Advisory Board (CAB)** | Change request governance; authorises standard, normal, and emergency changes; reviews AI system material change requests | Change Management and Configuration Policy |
| **Incident Response Team (IRT)** | Incident identification, classification, containment, eradication, and recovery operations; owns the post-incident review process | Incident Management Policy |
| **AI Governance Committee** | AI system risk classification authority; EU AI Act conformity assessment governance; high-risk system oversight. Quarterly cadence. Phase 2 body. | AI Governance Policy, Model Risk Policy |
| **Legal Counsel** | Regulatory notification obligations under GDPR Articles 33–34 and EU AI Act Article 73; privilege review for incident communications | Incident Management Policy, Privacy and Data Protection Policy |
| **HR** | Training completion records; security onboarding obligations; disciplinary process for policy violations | Security Awareness and Training Policy, Acceptable Use Policy |

---

## Document Index

All artefacts are listed below, organised by programme area. Links are relative to this file.

**Status key:** ✓ Published | ✓ Complete | ⧖ In Development | ☐ Planned

---

### Security Policies — Phase 1

Ten core information security policies developed for Emyzer Technology and implemented in ServiceNow GRC. All policies are published and in effect. Each contains a full evidence index specifying the system of record, owner, and retention period for every required evidence type.

| Policy | Owner | Status | Frameworks |
|---|---|---|---|
| [Information Security Policy](../policies/information-security-policy.md) | CISO | ✓ Published | ISO 27001:2022, NIST CSF 2.0, COBIT |
| [Access Control Policy](../policies/access-control-policy.md) | ISO | ✓ Published | ISO 27001:2022, NIST SP 800-53 Rev. 5, COBIT DSS05 |
| [Incident Management Policy](../policies/incident-management-policy.md) | ISO | ✓ Published | ISO 27035, NIST SP 800-61 Rev. 2, GDPR Art. 33–34 |
| [Risk Management Policy](../policies/risk-management-policy.md) | CRO | ✓ Published | ISO 31000:2018, NIST CSF 2.0, COSO ERM |
| [Business Continuity and DR Policy](../policies/bcdr-policy.md) | CRO | ✓ Published | ISO 22301:2019, NIST SP 800-34 |
| [Change Management and Configuration Policy](../policies/change-management-and-configuration-policy.md) | ISO | ✓ Published | ITIL 4, ISO 27001:2022, COBIT BAI06 |
| [Acceptable Use Policy](../policies/acceptable-use-policy.md) | ISO | ✓ Published | ISO 27001:2022, NIST CSF, SANS AUP |
| [Data Classification Policy](../policies/data-classification-policy.md) | ISO | ✓ Published | NIST SP 800-60, ISO 27001:2022, GDPR |
| [Third-Party Risk Management Policy](../policies/third-party-risk-management-policy.md) | ISO | ✓ Published | ISO 27036, NIST SP 800-161, NIST CSF ID.SC |
| [Security Awareness and Training Policy](../policies/security-awareness-and-training-policy.md) | ISO | ✓ Published | ISO 27001 A.6.3, NIST SP 800-50, PCI DSS |

---

### Risk Assessment Programme

| Document | Description | Status | Frameworks |
|---|---|---|---|
| [Risk Assessment Methodology](../risk-assessments/risk-assessment-methodology.md) | Six-step hybrid qualitative/quantitative methodology with 5×5 scoring matrix and tiered monitoring cadences | ✓ Complete | NIST SP 800-30, ISO 27005, COBIT, FAIR |
| [Asset Risk Register](../risk-assessments/asset-risk-register.md) | 15-entry operational register across four risk categories; includes treatment tracking and a formally documented budget-blocked Critical risk | ✓ Complete | NIST SP 800-30, ISO 27005, NIST CSF ID.RA |
| [Risk Appetite Statement](../risk-assessments/risk-appetite-statement.md) | Domain-specific tolerance thresholds with escalation governance, unacceptable risk conditions, and current posture assessment | ✓ Complete | ISO 31000:2018, COSO ERM |

---

### Business Continuity

| Document | Description | Status | Frameworks |
|---|---|---|---|
| [Business Impact Analysis Report](../business-continuity/business-impact-analysis-report.md) | 42-stakeholder-interview BIA; 4-tier process prioritisation; RTO/RPO analysis; financial exposure quantification across 12 critical processes | ✓ Complete | ISO 22301 Cl. 8.2.2, NIST SP 800-34 |

---

### Compliance Mapping

| Document | Description | Status |
|---|---|---|
| [Compliance Mapping README](../compliance-mapping/README.md) | Folder scope and framework references | ✓ Complete |
| `compliance-mapping/policy-benefits-and-evidence.md` | Maps each policy to compliance evidence requirements and organisational benefits | ☐ Planned |

---

### Templates

| Document | Purpose | Status |
|---|---|---|
| [Policy Template](../templates/policy-template.md) | Standardised framework for drafting new governance policies | ✓ Complete |
| [Risk Assessment Template](../templates/risk-assessment-template.md) | Risk identification, scoring, and treatment documentation | ✓ Complete |
| [Control Testing Template](../templates/control-testing-template.md) | Audit workbook structure for control testing and evidence collection | ✓ Complete |

---

### ServiceNow Evidence Exports

Raw policy exports from ServiceNow GRC. These PDFs show ownership, approval workflows, validity periods, and compliance mappings as generated by the platform.

| Document | Linked Policy | Status |
|---|---|---|
| [Evidence Exports README](../servicenow-evidence/README.md) | Index and guidance for reading raw ServiceNow exports | ✓ Complete |
| `Access Control Policy.pdf` | [Access Control Policy](../policies/access-control-policy.md) | ✓ Exported |
| `Business Continuity and Disaster Recovery Policy.pdf` | [BC/DR Policy](../policies/bcdr-policy.md) | ✓ Exported |
| `Incident Management Policy.pdf` | [Incident Management Policy](../policies/incident-management-policy.md) | ✓ Exported |
| `Information Security Policy.pdf` | [Information Security Policy](../policies/information-security-policy.md) | ✓ Exported |
| `Risk Management Policy.pdf` | [Risk Management Policy](../policies/risk-management-policy.md) | ✓ Exported |

---

### Enterprise Policies — Phase 2 (Emyzer Nexus)

These policies govern Emyzer Nexus as the post-acquisition parent entity. They address AI governance under the EU AI Act and the expanded privacy and training obligations arising from the Veridian AI acquisition. Phase 1 policies remain in effect as subsidiary documentation.

| Policy | Owner | Status | Frameworks |
|---|---|---|---|
| [AI Governance Policy](../enterprise-policies/ai-governance-policy.md) | CISO | ✓ Published | EU AI Act (Regulation 2024/1689), NIST AI RMF 1.0, ISO/IEC 42001:2023 |
| [Model Risk Policy](../enterprise-policies/model-risk-policy.md) | CRO | ✓ Published | SR 11-7, NIST AI RMF 1.0, EU AI Act |
| [Privacy and Data Protection Policy](../enterprise-policies/privacy-and-data-protection-policy.md) | DPO | ✓ Published | GDPR, UK GDPR, ISO 27701:2019 |
| [Security Awareness and Training Policy (Tier 2)](../enterprise-policies/security-awareness-and-training-policy.md) | CISO | ✓ Published | ISO 27001:2022, NIST SP 800-50, PCI DSS |

---

### AI Governance Programme — Phase 2

Supporting documents for the EU AI Act compliance programme: system inventory, article-by-article control mapping, and risk assessments for the two inherited Veridian AI systems.

| Document | Description | Status |
|---|---|---|
| `ai-governance/README.md` | AI governance programme overview and document index | ☐ Planned |
| `ai-governance/ai-system-inventory.md` | Formal EU AI Act risk tier classification of the Predictive Customer Churn Model and AI-Assisted Contract Review Tool | ☐ Planned |
| `ai-governance/eu-ai-act-mapping.md` | Control mapping of Emyzer Nexus AI systems to EU AI Act obligations (Articles 9, 10, 11, 13, 14, 15, 72, 73) with gap identification | ☐ Planned |
| `ai-governance/risk-assessments.md` | AI system risk assessments applying the Phase 1 methodology extended with AI-specific risk categories | ☐ Planned |

---

### M&A Integration Management — Phase 2

Documents covering the GRC integration of Veridian AI into the Emyzer Nexus structure: which policies apply to the acquired entity, what documentation requires remediation, and in what order.

| Document | Description | Status |
|---|---|---|
| `integration-management/README.md` | M&A integration governance scope and approach | ☐ Planned |
| `integration-management/m&a-grc-integration-charter.md` | Post-acquisition policy hierarchy; subsidiary governance arrangements; conditions triggering policy update or retirement | ☐ Planned |
| `integration-management/rationalization-roadmap.md` | Scheduled review timeline for all Phase 1 documentation; conflict identification log; Veridian AI documentation remediation priorities | ☐ Planned |

---

## Related Documentation

| Document | Description |
|---|---|
| [Portfolio Overview](../README.md) | Top-level programme narrative, 60-second review path, and skills demonstrated |
| [Enterprise Policies README](../enterprise-policies/readme.md) | Phase 2 policy architecture, design principles, and framework coverage matrix |
| [Emyzer Nexus Overview](../emyzer-nexus/readme.md) | Parent entity documentation *(forthcoming)* |
| [CONTRIBUTING.md](../CONTRIBUTING.md) | How changes are proposed, reviewed, approved, and merged across the portfolio |

---

*All content in this portfolio is a fictional case study developed for professional demonstration purposes. Framework and regulatory references are accurate as of the document publication dates.*

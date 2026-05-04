# Information Security GRC Portfolio

[![ServiceNow GRC](https://img.shields.io/badge/Platform-ServiceNow%20GRC-00C7B7?style=flat-square)](https://www.servicenow.com/products/governance-risk-and-compliance.html)
[![NIST CSF](https://img.shields.io/badge/Framework-NIST%20CSF-003366?style=flat-square)](https://www.nist.gov/cyberframework)
[![NIST AI RMF](https://img.shields.io/badge/Framework-NIST%20AI%20RMF-003366?style=flat-square)](https://www.nist.gov/itl/ai-risk-management-framework)
[![ISO 27001](https://img.shields.io/badge/Standard-ISO%2027001-1A73E8?style=flat-square)](https://www.iso.org/standard/27001)
[![ISO 22301](https://img.shields.io/badge/Standard-ISO%2022301-1A73E8?style=flat-square)](https://www.iso.org/standard/75106.html)
[![EU AI Act](https://img.shields.io/badge/Regulation-EU%20AI%20Act-FF6B35?style=flat-square)](https://artificialintelligenceact.eu/)
[![GDPR](https://img.shields.io/badge/Regulation-GDPR-FF6B35?style=flat-square)](https://gdpr.eu/)

**ServiceNow GRC Project: Emyzer Nexus (Fictionalized Case Study)**  
*AI governance, M&A integration, security policy development, and risk programme design. Built end-to-end in ServiceNow GRC.*

---

## Start Here (60-Second Review Path)

Begin with the flagship artifact, then follow the path most relevant to your evaluation focus.

✅ **Flagship Artifact:** [AI Governance Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/emyzer-nexus/enterprise-policies/ai-governance-policy.md). Parent-level policy governing AI/ML system development, acquisition, validation, monitoring, and retirement across Emyzer Nexus. Aligned to the EU AI Act and NIST AI RMF.

| If you want to evaluate... | Start here |
|----------------------------|------------|
| **AI governance and EU AI Act** | AI Governance Policy → EU AI Act Control Mapping → AI System Inventory |
| **M&A and policy integration** | M&A GRC Integration Charter → Policy Rationalization Roadmap |
| **Risk program design** | Risk Assessment Methodology → Asset Risk Register → Risk Appetite Statement |
| **Security policy depth** | Information Security Policy → Access Control Policy → evidence exports |
| **Audit readiness** | Any policy Evidence Index → ServiceNow evidence exports |

---

## Overview

This portfolio covers two phases of GRC work, both built in ServiceNow GRC and documented to audit-ready standards. Phase 1 is the foundational programme for Emyzer Technology: 10 security policies, a risk assessment programme, and ISO 22301 business continuity. Phase 2 is the post-acquisition programme for Emyzer Nexus: M&A governance integration, EU AI Act compliance for two inherited AI systems, and four enterprise-level policies.

The case study is built around a real governance problem. When a company acquires an AI-native startup, it inherits the startup's compliance gaps. Phase 2 shows how those gaps get assessed, documented, and addressed.

---

## Program Timeline

| Phase | Entity | Core Work |
|-------|--------|-----------|
| **Phase 1** | Emyzer Technology | Foundational GRC build: 10 enterprise security policies, business continuity documentation (ISO 22301), risk assessment methodology, asset risk register, and risk appetite statement. All implemented in ServiceNow. |
| **Phase 2** | Emyzer Nexus | Post-acquisition governance: M&A GRC Integration Charter, AI governance program (EU AI Act + NIST AI RMF), AI system risk classifications for inherited Veridian AI systems, and a policy rationalization roadmap governing legacy documentation |

---

## Organizational Context

**Emyzer Technology (Phase 1)** was a fictional multinational technology company with four business lines (laptop production, cloud service management, enterprise technical support, and global security implementation) operating across Asia, the Americas, Africa, and parts of Europe and the Middle East, with over 5,000 staff.

**Veridian AI (Acquired)** was a fictional AI-native startup with two enterprise products: a predictive customer churn model and an AI-assisted contract review tool built on a third-party LLM API. Both systems required formal risk classification and compliance assessment under the EU AI Act following acquisition.

**Emyzer Nexus (Phase 2)** is the post-acquisition parent entity. All Phase 1 documentation remains in effect as subsidiary documentation under the policy hierarchy established in the M&A GRC Integration Charter.

---

## Phase 2: Emyzer Nexus

### M&A Integration Governance

| Artifact | Description | Frameworks |
|----------|-------------|------------|
| [M&A GRC Integration Charter](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/emyzer-nexus/integration-management/ma-grc-integration-charter.md) | Establishes the post-acquisition policy hierarchy, defines subsidiary documentation governance, and sets the conditions that trigger policy review or retirement | ISO 31000, NIST CSF |
| [Policy Rationalization Roadmap](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/emyzer-nexus/integration-management/policy-rationalization-roadmap.md) | Scheduled review timeline for all Phase 1 documentation, conflict identification log, and update prioritization criteria | ISO 27001 |

### AI Governance Program

| Artifact | Description | Frameworks |
|----------|-------------|------------|
| [AI Governance Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/emyzer-nexus/enterprise-policies/ai-governance-policy.md) ⭐ | Parent-level policy governing the development, acquisition, validation, monitoring, and retirement of AI/ML systems across Emyzer Nexus | EU AI Act, NIST AI RMF |
| [Model Risk Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/emyzer-nexus/enterprise-policies/model-risk-policy.md) | Operational policy covering model lifecycle management, bias testing cadence, human oversight requirements, explainability standards, and incident response for model failures | NIST AI RMF, ISO/IEC 42001 |
| [AI System Inventory and Classification](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/emyzer-nexus/ai-governance/ai-system-inventory.md) | Formal classification of the Veridian AI churn model and contract review tool under EU AI Act risk tiers, including Article 9 risk management system requirements for high-risk systems | EU AI Act, NIST AI RMF |
| [EU AI Act Control Mapping](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/emyzer-nexus/ai-governance/eu-ai-act-control-mapping.md) | Control mapping of Emyzer Nexus AI systems to EU AI Act obligations, with compliance gap identification and remediation priorities | EU AI Act |

### Veridian AI Integration

| Artifact | Description | Frameworks |
|----------|-------------|------------|
| [Veridian AI Risk Assessment](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/veridian-ai/ai-risk-assessments/veridian-ai-risk-assessment.md) | Risk assessments for inherited AI systems using the Phase 1 methodology, extended with AI-specific risk categories: model drift, training data bias, explainability gaps, and third-party model dependency | NIST AI RMF, ISO 31000, NIST SP 800-30 |
| [AI Vendor Risk Due Diligence Addendum](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/veridian-ai/vendor-risk-addendum/ai-vendor-risk-addendum.md) | Extension of the Phase 1 Third-Party Risk Management Policy covering AI-specific vendor evaluation: model transparency, data retention practices, bias audit availability, and contractual liability for model errors | ISO 27001 A.15, NIST AI RMF, EU AI Act |

---

## Phase 1 Foundation: Emyzer Technology

Phase 1 established the governance baseline that Phase 2 builds on. All artifacts remain in effect as subsidiary documentation under Emyzer Nexus.

### Security Policies

| Policy | Frameworks |
|--------|------------|
| [Information Security Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/information-security-policy.md) | NIST CSF, ISO 27001, COBIT |
| [Access Control Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/access-control-policy.md) | NIST AC, ISO 27001 A.5.15–A.5.18, COBIT DSS05 |
| [Incident Management Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/incident-management-policy.md) | NIST IR, ISO 27035, GDPR Art. 33–34 |
| [Risk Management Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/risk-management-policy.md) | COSO ERM, ISO 31000 |
| [BC/DR Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/bcdr-policy.md) | ISO 22301, NIST SP 800-34 |
| [Change Management and Configuration Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/change-management-and-configuration-policy.md) | ITIL, COBIT BAI06, NIST SP 800-128 |
| [Acceptable Use Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/acceptable-use-policy.md) | NIST CSF, ISO 27001 A.5.10, SANS AUP |
| [Data Classification Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/data-classification-policy.md) | NIST SP 800-60, ISO 27001 A.5.12–A.5.13, GDPR |
| [Third-Party/Vendor Risk Management Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/third-party-risk-management-policy.md) | NIST SP 800-161, ISO 27036, NIST CSF ID.SC |
| [Security Awareness and Training Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/security-awareness-and-training-policy.md) | NIST CSF PR.AT, ISO 27001 A.6.3, NIST SP 800-50 |

### Risk Assessment Program

| Artifact | Description |
|----------|-------------|
| [Risk Assessment Methodology](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/risk-assessments/risk-assessment-methodology.md) | Six-step hybrid qualitative/quantitative methodology with 5×5 scoring matrix, tiered monitoring cadences, and multi-framework alignment |
| [Asset Risk Register](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/risk-assessments/asset-risk-register.md) | 15-entry operational risk register across information security, privacy, operational, and third-party risk categories. Includes full treatment tracking and a budget-blocked Critical risk documented at actual status. |
| [Risk Appetite Statement](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/risk-assessments/risk-appetite-statement.md) | Domain-specific tolerance thresholds with escalation governance, unacceptable risk conditions, and current posture assessment against defined appetite |

### Business Continuity

| Artifact | Frameworks |
|----------|------------|
| [Business Impact Analysis](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/business-continuity/business-impact-analysis-report.md) | ISO 22301 Cl. 8.2.2, NIST SP 800-34 |
| BCDR Tabletop Exercise Summary | ISO 22301 Cl. 8.5, BCI PP6 |

---

## Skills Demonstrated

| Competency | What the Work Shows |
|------------|---------------------|
| **AI Risk Management** | Classified two inherited AI systems under EU AI Act Annex III. Built article-by-article control mappings for Articles 9–15, 72, and 73. Designed controls targeting specific failure modes: model drift, LLM hallucination, training data bias, and prompt injection. |
| **M&A GRC Integration** | Structured a post-acquisition policy hierarchy governing the acquired entity from Day 0. Defined conditions for policy review and retirement. Documented 15 integration risks with owners and target dates. |
| **Policy Development** | Each policy includes a full Evidence Index specifying system of record, owner, and retention period for every evidence type required. Implemented in ServiceNow GRC. |
| **Risk Assessment Program Design** | Built a hybrid 5×5 methodology applied to a 15-entry asset register. One entry documents a budget-blocked Critical risk at its actual status, with the block identified as the root cause. |
| **Framework Translation** | Mapped EU AI Act, ISO 22301, and NIST AI RMF obligations to operational controls with traceable linkages. Each mapping includes gap identification and remediation priorities. |
| **GRC Platform Proficiency** | Built and managed policies, risk registers, and compliance workflows in ServiceNow GRC. PDF platform exports in `/servicenow-evidence/` are direct evidence of module-level work. |
| **Vendor Risk Management** | Extended the Phase 1 TPRM Policy with an AI-specific due diligence addendum covering model transparency, training data provenance, bias testing, EU AI Act compliance assessment, and contractual liability for model errors. |
| **Evidence Management** | Each artefact specifies a system of record, a responsible owner, and a retention period. Evidence requirements are defined in the document, not left to interpretation. |

---

## Frameworks and Standards Referenced

| Framework | Application |
|-----------|-------------|
| **EU AI Act** | AI system risk classification, High-Risk system obligations (Articles 9–15), and post-market monitoring requirements. Applied to inherited Veridian AI systems. |
| **NIST AI RMF** | AI governance program structure: Govern, Map, Measure, Manage functions |
| **ISO/IEC 42001:2023** | AI management system standard. Applied in the Model Risk Policy and AI Governance Programme. |
| **NIST Cybersecurity Framework (CSF)** | Security policy structure and control categories |
| **NIST SP 800-30 Rev. 1** | Risk assessment process guidance |
| **NIST SP 800-34 Rev. 1** | Contingency planning guidance |
| **ISO/IEC 27001:2022** | Information security management system alignment |
| **ISO/IEC 27005** | Information security risk management |
| **ISO 22301:2019** | Business continuity management system |
| **ISO 31000:2018** | Enterprise risk management principles |
| **COSO ERM** | Enterprise risk management integration |
| **COBIT 2019** | IT governance and management objectives |
| **FAIR** | Quantitative risk assessment methodology |
| **GDPR** | Data protection and privacy compliance |
| **PCI DSS** | Payment card data security standards |
| **SOC 2** | Trust services criteria mapping |
| **ITIL** | IT service management and change control |

---

## Tools and Technologies

- **ServiceNow GRC**: Policy management, risk register, compliance tracking, workflow automation
- **ServiceNow IRM**: Integrated risk management workflows
- **GitHub**: Version control and portfolio presentation
- **Markdown**: Documentation format

---

## Repository Structure

```
information-security-grc-portfolio/
│
├── emyzer-nexus/                        # Phase 2: Parent entity documentation
│   ├── integration-management/          # M&A GRC Integration Charter, rationalization roadmap
│   ├── enterprise-policies/             # AI Governance Policy, Model Risk Policy
│   └── ai-governance/                   # AI system inventory, risk assessments, EU AI Act mapping
│
├── emyzer-technology/                   # Phase 1: Subsidiary documentation (in effect)
│   ├── policies/                        # 10 enterprise security policies
│   ├── business-continuity/             # BC/DR documentation (ISO 22301)
│   ├── risk-assessments/                # Risk methodology, registers, risk appetite statement
│   └── compliance-mapping/              # Framework alignment matrices
│
├── veridian-ai/                         # Acquired entity documentation
│   ├── ai-risk-assessments/             # Risk assessments for inherited AI systems
│   └── vendor-risk-addendum/            # AI-specific vendor due diligence addendum
│
├── servicenow-evidence/                 # Raw platform exports: policy proof, not just documentation
├── templates/                           # Reusable GRC templates
└── README.md
```

---

## Intended Audience

- **GRC and Information Security hiring managers** evaluating practical, platform-demonstrated experience
- **AI governance professionals** reviewing EU AI Act compliance approaches and model risk frameworks
- **Risk and Compliance analysts** seeking documentation examples grounded in real governance trade-offs
- **Security auditors** reviewing policy structure, evidence indexes, and framework alignment
- **ServiceNow practitioners** exploring GRC module implementation at the policy and risk register level

---

## Portfolio Note

All content was developed independently using published frameworks and standards. The fictional company context allows real governance problems to be documented in a public-facing format.

Phase 1 covers Emyzer Technology's GRC programme before the acquisition. Phase 2 covers Emyzer Nexus after it. Phase 1 artefacts remain in effect as subsidiary documentation under the policy hierarchy in the M&A GRC Integration Charter.

---

## Author

**Olusola B. Akanji**  
Information Security and GRC Professional. Focus areas: AI governance, risk programme design, and multi-framework regulatory compliance. Open to GRC analyst, AI governance, and information security risk roles.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat-square&logo=linkedin)](https://www.linkedin.com/in/olusola-b-akanji/)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-181717?style=flat-square&logo=github)](https://github.com/olusolaxakanji)
[![GRC Writing](https://img.shields.io/badge/Blog-GRC%20Writing%20%26%20Analysis-21759B?style=flat-square&logo=wordpress)](https://cleanlikesoapblog.wordpress.com/category/grc/)

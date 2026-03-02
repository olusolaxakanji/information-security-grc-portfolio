# Information Security GRC Portfolio

[![ServiceNow GRC](https://img.shields.io/badge/Platform-ServiceNow%20GRC-00C7B7?style=flat-square)](https://www.servicenow.com/products/governance-risk-and-compliance.html)
[![NIST CSF](https://img.shields.io/badge/Framework-NIST%20CSF-003366?style=flat-square)](https://www.nist.gov/cyberframework)
[![NIST AI RMF](https://img.shields.io/badge/Framework-NIST%20AI%20RMF-003366?style=flat-square)](https://www.nist.gov/itl/ai-risk-management-framework)
[![ISO 27001](https://img.shields.io/badge/Standard-ISO%2027001-1A73E8?style=flat-square)](https://www.iso.org/standard/27001)
[![ISO 22301](https://img.shields.io/badge/Standard-ISO%2022301-1A73E8?style=flat-square)](https://www.iso.org/standard/75106.html)
[![EU AI Act](https://img.shields.io/badge/Regulation-EU%20AI%20Act-FF6B35?style=flat-square)](https://artificialintelligenceact.eu/)
[![GDPR](https://img.shields.io/badge/Regulation-GDPR-FF6B35?style=flat-square)](https://gdpr.eu/)

**ServiceNow GRC Project – Emyzer Nexus (Fictionalized Case Study)**  
*A living GRC portfolio of production-style security policies, risk assessments, AI governance artifacts, and M&A integration documentation.*

---

## Start Here (60-Second Review Path)

If you only have a minute, start with the **Information Security Policy** and review in this order:

1. **Policy Snapshot** → executive view (scope, governance, exceptions, evidence)
2. **Evidence Index** → audit readiness view (system of record, owner, retention)
3. **Policy Exceptions** → real-world governance (approval, duration, quarterly review)
4. **M&A Integration Charter** → how legacy documentation remains in effect under the new parent entity

✅ **Flagship Artifact:** [Information Security Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/information-security-policy.md)

---

## Overview

This repository demonstrates hands-on GRC work implemented in ServiceNow GRC and translated into clear, audit-oriented documentation. It includes enforceable policy language, defined governance roles, exception handling, evidence-of-compliance artifacts, framework alignment, and a structured M&A integration program showing how a GRC program absorbs an acquired entity without creating compliance gaps.

The portfolio is organized into two program phases that reflect how GRC governance actually evolves in an organization: a foundational build followed by a material organizational change that required new parent-level documentation, an AI governance program, and a formal policy rationalization roadmap.

**Note on maturity:** This portfolio is actively maintained and updated as new artifacts are completed.

---

## Program Timeline

| Phase | Period | Entity | Description |
|-------|--------|--------|-------------|
| **Phase 1** | 2024 | Emyzer Technology | Foundational GRC program build: 10 enterprise security policies, business continuity documentation, risk assessment methodology, asset risk register, and risk appetite statement |
| **Phase 2** | 2025 | Emyzer Nexus | Post-acquisition integration: Emyzer Technology acquires Veridian AI and rebrands as Emyzer Nexus. GRC program expands to cover inherited AI systems, triggering development of an AI governance program aligned to the EU AI Act and NIST AI RMF |

---

## Organizational Context (Fictionalized Case Study)

### Emyzer Technology (Phase 1 Entity)

Emyzer Technology was a fictional multinational technology company operating across Asia, the Americas, Africa, and parts of Europe and the Middle East. The organization provided:

- Laptop production and global distribution
- Cloud service management
- Enterprise technical support
- Global security implementation for businesses

The organization employed over 5,000 staff worldwide and operated in a complex, distributed IT and security environment requiring structured governance and resilience planning.

### Veridian AI (Acquired Entity)

Veridian AI was a fictional AI-native startup specializing in machine learning solutions for enterprise clients. Its product suite included:

- A predictive customer churn model used by B2B SaaS clients
- An AI-assisted contract review tool built on a third-party large language model API

Veridian AI was acquired by Emyzer Technology in Q1 2025. The acquisition introduced two AI systems into the combined organization's technology environment, both requiring formal risk classification, governance documentation, and compliance assessment under the EU AI Act.

### Emyzer Nexus (Phase 2 Parent Entity)

Following the acquisition of Veridian AI, Emyzer Technology rebranded as Emyzer Nexus. The combined organization retained all existing Emyzer Technology governance documentation under a formal policy hierarchy established in the M&A GRC Integration Charter. Legacy documentation from Phase 1 remains in effect as subsidiary documentation until a scheduled review or a material change triggers a formal update.

*This case study was designed to simulate realistic enterprise conditions for practicing GRC methodology, M&A integration governance, AI risk management, and ServiceNow platform workflows.*

---

## Project Scope and Objectives

This project was completed using **ServiceNow** and covers two phases of GRC program development.

**Phase 1 objectives:**

1. Development of 10 enterprise information security policies aligned to recognized frameworks
2. Documentation of organizational benefits for each policy
3. Identification of evidence of compliance and retention expectations
4. Design of a Business Continuity Management System (BCMS) aligned to ISO/IEC 22301
5. Development of a risk assessment methodology, asset risk register, and risk appetite statement

**Phase 2 objectives:**

1. Establishment of a policy hierarchy and governance structure for the post-acquisition entity
2. Classification of inherited AI systems under the EU AI Act risk framework
3. Development of an AI governance program aligned to NIST AI RMF and EU AI Act requirements
4. Extension of the vendor risk framework to cover AI-specific third-party due diligence
5. Documentation of a policy rationalization roadmap governing the lifecycle of legacy subsidiary documentation

All policies, procedures, and plans were created and managed within the **ServiceNow platform** in accordance with project requirements.

---

## Repository Structure

```
information-security-grc-portfolio/
│
├── emyzer-nexus/                        # Phase 2: Parent entity documentation
│   ├── integration-management/          # M&A GRC Integration Charter, rationalization roadmap
│   ├── enterprise-policies/             # Parent-level AI governance and model risk policies
│   └── ai-governance/                   # AI system inventory, risk assessments, EU AI Act mapping
│
├── emyzer-technology/                   # Phase 1: Subsidiary documentation (in effect)
│   ├── policies/                        # Enterprise security policies (10 completed)
│   ├── business-continuity/             # BC/DR documentation (ISO 22301)
│   ├── risk-assessments/                # Risk methodology, registers, risk appetite statement
│   └── compliance-mapping/              # Framework alignment matrices
│
├── veridian-ai/                         # Acquired entity documentation
│   ├── ai-risk-assessments/             # Risk assessments for inherited AI systems
│   └── vendor-risk-addendum/            # AI-specific vendor due diligence addendum
│
├── servicenow-evidence/                 # Platform implementation artifacts
├── templates/                           # Reusable GRC templates
└── README.md
```

| Folder | Contents |
|--------|----------|
| [`emyzer-nexus/integration-management/`] | M&A GRC Integration Charter, Policy Rationalization Roadmap |
| [`emyzer-nexus/enterprise-policies/`] | AI Governance Policy, Model Risk Policy |
| [`emyzer-nexus/ai-governance/`] | AI System Inventory and Classification, EU AI Act Control Mapping |
| [`emyzer-technology/policies/`] | 10 enterprise security policies (Access Control, Incident Management, Risk Management, Information Security, BC/DR, Change Management, Acceptable Use, Data Classification, Third-Party Risk, Security Awareness) |
| [`emyzer-technology/business-continuity/`] | ISO 22301 BCMS documentation, BIA, tabletop exercises, framework alignment |
| [`emyzer-technology/risk-assessments/`] | Risk methodology, asset risk register, risk appetite statement |
| [`emyzer-technology/compliance-mapping/`] | Framework alignment matrices, gap analysis, evidence guides |
| [`veridian-ai/ai-risk-assessments/`] | Risk assessments for acquired churn model and contract review AI systems |
| [`veridian-ai/vendor-risk-addendum/`] | AI-specific vendor due diligence addendum extending the Phase 1 third-party risk framework |
| [`servicenow-evidence/`] | Platform screenshots, workflow documentation, implementation artifacts |
| [`templates/`] | Reusable policy, risk assessment, and control testing templates |

---

## Current Portfolio Status

### Phase 1 Artifacts: Emyzer Technology (Completed)

#### Policies

| Policy | Description | Frameworks | Status |
|--------|-------------|------------|--------|
| [Information Security Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/information-security-policy.md) | Parent policy establishing security governance structure with full evidence index, exception handling, and control cadence | NIST CSF, ISO 27001, COBIT | ✅ Complete |
| [Access Control Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/access-control-policy.md) | RBAC/ABAC implementation, least privilege, authentication requirements | COBIT DSS05, NIST AC | ✅ Complete |
| [Incident Management Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/incident-management-policy.md) | Detection, response, escalation, and recovery procedures | NIST IR, ISO 27035 | ✅ Complete |
| [Risk Management Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/risk-management-policy.md) | Risk identification, assessment, and treatment methodology | COSO ERM, ISO 31000 | ✅ Complete |
| [BC/DR Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/bcdr-policy.md) | Business continuity and disaster recovery governance | ISO 22301, NIST SP 800-34 | ✅ Complete |
| [Change Management and Configuration Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/change-management-policy.md) | Change control processes, configuration baseline management, and CAB governance | ITIL, COBIT BAI06, NIST SP 800-128 | ✅ Complete |
| [Acceptable Use Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/acceptable-use-policy.md) | Authorized use of organizational IT resources, user responsibilities, and prohibited activities | SANS AUP, ISO 27001 A.8, NIST CSF | ✅ Complete |
| [Data Classification Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/data-classification-policy.md) | Data categorization framework, labeling requirements, and handling procedures by classification level | ISO 27001 A.8.2, NIST SP 800-60, GDPR | ✅ Complete |
| [Third-Party/Vendor Risk Management Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/third-party-risk-management-policy.md) | Vendor security assessment, contract security requirements, and ongoing monitoring | ISO 27001 A.15, NIST CSF ID.SC, GDPR | ✅ Complete |
| [Security Awareness and Training Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/security-awareness-training-policy.md) | Security education program, role-based training requirements, and phishing simulation protocols | NIST CSF PR.AT, ISO 27001 A.7.2, COBIT APO07 | ✅ Complete |

#### Risk Assessment Program

| Artifact | Description | Frameworks | Status |
|----------|-------------|------------|--------|
| [Risk Assessment Methodology](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/risk-assessments/risk-assessment-methodology.md) | Six-step hybrid qualitative/quantitative methodology with 5x5 scoring matrix, tiered monitoring cadences, and framework alignment | ISO 31000, NIST SP 800-30, NIST CSF, ISO 27005, COBIT 2019, FAIR | ✅ Complete |
| [Asset Risk Register](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/risk-assessments/asset-risk-register.md) | 15-entry operational risk register covering information security, privacy, operational, and third-party risk categories with full treatment tracking | NIST CSF, ISO 27001, SOC 2, GDPR | ✅ Complete |
| [Risk Appetite Statement](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/risk-assessments/risk-appetite-statement.md) | Domain-specific tolerance thresholds with escalation governance, unacceptable risk conditions, and current posture assessment against defined appetite | ISO 31000, NIST CSF, ISO 27001 | ✅ Complete |

#### Business Continuity

| Artifact | Description | Status |
|----------|-------------|--------|
| Business Impact Analysis | Critical process identification, RTO/RPO targets, and recovery prioritization | 🔄 Draft |
| BCDR Tabletop Exercise Summary | Documented exercise scenarios, findings, and remediation actions | 🔄 Draft |

#### Compliance Mapping

| Artifact | Description | Status |
|----------|-------------|--------|
| Framework Alignment Matrix | Cross-framework control mapping across NIST CSF, ISO 27001, SOC 2, and GDPR | 🔄 Draft |
| NIST CSF Control Mapping | Detailed control mapping to NIST CSF subcategories | 🔄 Draft |
| SOC 2 Gap Analysis | Trust services criteria gap assessment and remediation roadmap | 📋 Planned |

---

### Phase 2 Artifacts: Emyzer Nexus (In Development)

#### M&A Integration Governance

| Artifact | Description | Frameworks | Status |
|----------|-------------|------------|--------|
| M&A GRC Integration Charter | Establishes the policy hierarchy, defines subsidiary documentation governance, and sets the conditions that trigger policy review or retirement | ISO 31000, NIST CSF | 🔄 In Development |
| Policy Rationalization Roadmap | Scheduled review timeline for all Phase 1 documentation, conflict identification log, and update prioritization criteria | ISO 27001 | 🔄 In Development |

#### AI Governance Program

| Artifact | Description | Frameworks | Status |
|----------|-------------|------------|--------|
| AI System Inventory and Classification | Formal classification of the Veridian AI churn model and contract review tool under EU AI Act risk tiers, including Article 9 risk management system requirements for high-risk systems | EU AI Act, NIST AI RMF | 🔄 In Development |
| AI Governance Policy | Parent-level policy governing the development, acquisition, validation, monitoring, and retirement of AI/ML systems across Emyzer Nexus | EU AI Act, NIST AI RMF | 🔄 In Development |
| Model Risk Policy | Operational policy covering model lifecycle management, bias testing cadence, human oversight requirements, explainability standards, and incident response for model failures | NIST AI RMF, ISO/IEC 42001 | 🔄 In Development |
| EU AI Act Control Mapping | Control mapping of Emyzer Nexus AI systems to EU AI Act obligations, with compliance gap identification and remediation priorities | EU AI Act | 📋 Planned |

#### Veridian AI Integration Artifacts

| Artifact | Description | Frameworks | Status |
|----------|-------------|------------|--------|
| Veridian AI Risk Assessment | Risk assessments for inherited AI systems using the Phase 1 methodology, extended with AI-specific risk categories: model drift, training data bias, explainability gaps, and third-party model dependency | NIST AI RMF, ISO 31000, NIST SP 800-30 | 🔄 In Development |
| AI Vendor Risk Due Diligence Addendum | Extension of the Phase 1 Third-Party Risk Management Policy covering AI-specific vendor evaluation criteria: model transparency, data retention practices, bias audit availability, and contractual liability for model errors | ISO 27001 A.15, NIST AI RMF, EU AI Act | 📋 Planned |

---

## Skills Demonstrated

| Competency | Application |
|------------|-------------|
| **Policy Development** | Created enforceable security policies with clear scope, roles, evidence requirements, and exception handling |
| **M&A GRC Integration** | Designed a post-acquisition governance structure with a formal policy hierarchy, subsidiary documentation continuity, and a rationalization roadmap |
| **AI Risk Management** | Applied EU AI Act risk classification tiers and NIST AI RMF governance functions to inherited AI systems |
| **Risk Assessment Program Design** | Built a complete risk assessment methodology, 15-entry risk register, and risk appetite statement with escalation governance |
| **Framework Application** | Translated abstract standards (NIST, ISO 22301, EU AI Act) into operational documentation with traceable control linkages |
| **GRC Platform Proficiency** | Built and managed policies within ServiceNow's governance module |
| **Business Continuity Planning** | Designed resilience strategies aligned to ISO/IEC 22301 requirements |
| **Evidence Management** | Documented systems of record, retention periods, and audit-ready evidence indexes |
| **Vendor Risk Management** | Designed third-party risk controls covering SOC 2 assurance, continuous monitoring, contractual security requirements, and AI-specific due diligence |
| **Cross-Functional Thinking** | Addressed security, operations, business continuity, and AI governance as integrated organizational concerns |

---

## Frameworks and Standards Referenced

| Framework | Application |
|-----------|-------------|
| **NIST Cybersecurity Framework (CSF)** | Security policy structure and control categories |
| **NIST AI Risk Management Framework (AI RMF)** | AI governance program structure and model risk management |
| **NIST SP 800-30 Rev. 1** | Risk assessment process guidance |
| **NIST SP 800-34 Rev. 1** | Contingency planning guidance |
| **NIST SP 800-60** | Data classification guidance |
| **NIST SP 800-128** | Configuration management guidance |
| **ISO/IEC 27001:2022** | Information security management system alignment |
| **ISO/IEC 27005** | Information security risk management |
| **ISO 22301:2019** | Business continuity management system |
| **ISO/IEC 27031:2011** | ICT readiness for business continuity |
| **ISO/IEC 42001:2023** | AI management system standard |
| **EU AI Act** | AI system risk classification, high-risk system obligations, and governance requirements |
| **COBIT 2019** | IT governance and management objectives |
| **COSO ERM** | Enterprise risk management integration |
| **FAIR** | Factor Analysis of Information Risk for quantitative assessment |
| **ISO 31000:2018** | Enterprise risk management principles |
| **BCI Good Practice Guidelines** | Business continuity planning methodology |
| **ITIL** | IT service management and change control |
| **SANS** | Acceptable use policy framework |
| **SOC 2** | Trust services criteria mapping |
| **GDPR** | Data protection and privacy compliance for EU operations |
| **PCI DSS** | Payment card data security standards |

---

## Tools and Technologies

- **ServiceNow GRC** — Policy management, risk register, compliance tracking
- **ServiceNow IRM** — Integrated risk management workflows
- **GitHub** — Version control and portfolio presentation
- **Markdown** — Documentation format

---

## Intended Audience

This repository is intended for:

- **GRC and Information Security hiring managers** evaluating practical experience
- **Risk and Compliance analysts** seeking documentation examples
- **Security auditors** reviewing policy structure and framework alignment
- **AI governance professionals** reviewing model risk and EU AI Act compliance approaches
- **Students and professionals** studying security governance frameworks
- **ServiceNow practitioners** exploring GRC module implementation

---

## Portfolio Note

This repository represents applied learning through structured case study work. All content has been developed independently using recognized frameworks and tools. The fictionalized organizational context was designed to simulate realistic enterprise conditions, including M&A integration governance and AI system risk management, while maintaining a professional, non-proprietary example suitable for public portfolio demonstration.

Phase 1 documentation reflects the Emyzer Technology GRC program as it existed prior to the acquisition. Phase 2 documentation reflects the expanded governance responsibilities of Emyzer Nexus as the post-acquisition parent entity. All Phase 1 artifacts remain in effect as subsidiary documentation under the policy hierarchy established in the M&A GRC Integration Charter.

---

## Author

**Olusola B. Akanji**  
Information Security and GRC Professional

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat-square&logo=linkedin)](https://www.linkedin.com/in/olusola-b-akanji/)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-181717?style=flat-square&logo=github)](https://github.com/olusolaxakanji)

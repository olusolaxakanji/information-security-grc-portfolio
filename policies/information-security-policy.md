# Information Security Policy

**Emyzer Technology – Governance, Risk, and Compliance**

---

## Policy Metadata

| Attribute | Value |
|-----------|-------|
| **Policy Name** | Information Security Policy |
| **Type** | Policy |
| **Owner** | Information Security Officer (Susan Orwell) |
| **Owning Group** | App Engine Admins |
| **State** | Published |
| **Valid From** | 2026-01-13 |
| **Valid To** | 2027-01-13 |
| **Approvers** | Chief Information Security Officer |
| **Reviewers** | GRC Analyst |
| **Knowledge Base** | Governance, Risk, and Compliance |
| **Published Policy** | KB-PORTFOLIO-0003 |

---

## Description

This policy aims to protect the confidentiality, integrity, and availability of information.

**Impact:** Ensures data security for cloud services, customer data protection, and cybersecurity resilience.

**Relevant Standards:** ISO/IEC 27001, ISO/IEC 27017, ISO/IEC 27018, ISO/IEC 27032

---

## Policy Snapshot

| Dimension | Summary |
|-----------|---------|
| **Applies to** | All workforce members (employees, contractors, consultants, temporary staff) and third parties |
| **Covers** | All information assets: data, systems, networks, applications, and related resources |
| **Review Cadence** | Annual review or upon major organizational/regulatory changes |
| **Key Governance** | CISO provides executive oversight; ISO owns ISMS operations; department leaders enforce compliance; IT implements technical controls |
| **Exceptions Process** | ServiceNow workflow with ISO/CISO approval; maximum 90-day duration; quarterly review of active exceptions |
| **Evidence Maintained** | Access reviews, training records, incident tickets, audit reports, risk register (all with defined retention periods) |

---

## A. Purpose

To establish a framework for managing and protecting the confidentiality, integrity, and availability of information assets within Emyzer Technology. This policy aims to safeguard data against unauthorized access, disclosure, alteration, and destruction, ensuring the security of cloud services and customer data, and enhancing cybersecurity resilience.

---

## B. Scope

This policy applies to all employees, contractors, consultants, temporary staff, and other workers at Emyzer Technology, including all personnel affiliated with third parties. It encompasses all information assets, systems, networks, applications, and data owned or managed by Emyzer Technology.

**Third-party applicability:** Third parties handling organizational data or systems **shall** meet equivalent security controls via contractual requirements and periodic security reviews.

---

## C. Definitions

1. **Confidentiality:** Ensuring that information is accessible only to authorized users.

2. **Integrity:** Safeguarding the accuracy and completeness of information and processing methods.

3. **Availability:** Ensuring authorized users can access information and associated assets when required.

4. **Information Assets:** Data, systems, networks, applications, and other resources that manage information.

---

## D. Policy Statement

Emyzer Technology is committed to protecting its information assets from all threats, whether internal or external, deliberate or accidental. To achieve this, the organization **shall**:

1. Implement an Information Security Management System (ISMS) following ISO/IEC 27001 standards.

2. Use ISO/IEC 27017 and ISO/IEC 27018 guidelines for cloud service security and personal data protection.

3. Adopt ISO/IEC 27032 standards to enhance cybersecurity measures.

4. Assess and manage risks to information security **quarterly**, with critical risks reviewed **monthly** for status, treatment progress, and risk acceptance decisions.

5. Ensure all employees comply with this policy and related procedures through documented acknowledgement and annual attestation.

6. Respond to security incidents within defined timeframes (critical: 1 hour; high: 4 hours; medium: 24 hours) to minimize impact. **Response timeframes refer to initial triage and assignment; containment and eradication timelines are defined in the Incident Response Plan. Severity definitions are maintained in the Incident Management Policy.**

7. Review and audit the ISMS **annually** with continuous improvement through management review meetings held **quarterly**.

---

## E. Roles and Responsibilities

### E.1 Chief Information Security Officer (CISO)
Provides executive oversight of the information security program. **Shall** approve strategic policy exceptions, significant risk acceptance decisions, and annual ISMS management reviews. **Shall** serve as the escalation point for critical security incidents and reportable breaches.

### E.2 Information Security Officer (ISO)
**Shall** develop, implement, and maintain the ISMS under CISO direction. **Shall** ensure compliance with relevant standards and regulations through documented evidence and periodic assessments. Acts as the delegated security executive for day-to-day program operations.

### E.3 Department Heads
**Shall** ensure their teams comply with the information security policy and related procedures through **quarterly attestation for departmental compliance**. **Shall** identify and report security risks within 24 hours of discovery.

### E.4 IT Department
**Shall** implement technical controls and monitor information systems **on an ongoing basis** to protect against security threats. **Shall** maintain security audit logs for a minimum of 1 year (3 years for privileged access).

### E.5 All Employees
**Shall** comply with the information security policy, complete **annual** security awareness training, and report any security incidents, suspected incidents, or vulnerabilities within 1 hour of discovery.

---

## F. Minimum Security Requirements

The following requirements establish baseline security controls. Detailed implementation procedures are maintained in the **IT Security Procedures Manual** and related operational documentation.

### F.1 Risk Assessment
- **Shall** conduct risk assessments **quarterly** to identify and evaluate security risks.
- **Shall** implement controls aligned to risk severity: critical risks require mitigation within 30 days; high risks within 60 days; moderate risks within 90 days.
- **Shall** document all risk assessments with identified threats, vulnerabilities, likelihood, impact, and treatment decisions in the enterprise risk register.

### F.2 Access Control
- **Shall** implement role-based access controls (RBAC) to ensure only personnel with job-aligned authorization can access information assets.
- **Shall** review standard user access rights **quarterly** and privileged access rights **monthly**, with documented manager approval retained for 3 years.
- **Shall** provision new access within 24 hours of approved request and deprovision access within 4 hours of termination or role change.

### F.3 Data Protection
- **Shall** encrypt sensitive data at rest (AES-256 minimum) and in transit (TLS 1.2 minimum).
- **Shall** classify data according to sensitivity levels (Public, Internal, Confidential, Restricted) with handling requirements documented per classification.
- **Shall** ensure compliance with data protection regulations including GDPR, CCPA, and applicable industry standards **where applicable based on data residency, customer contracts, and processing activities**.

### F.4 Incident Management
- **Shall** establish and maintain procedures for detecting, reporting, and responding to security incidents within defined response timeframes.
- **Shall** conduct root cause analysis for all high and critical incidents within 5 business days of resolution.
- **Shall** implement corrective actions with documented verification of effectiveness within 30 days.

### F.5 Training and Awareness
- **Shall** provide information security awareness training to all employees **annually** and during onboarding (within 7 days of start date).
- **Shall** provide role-specific training for personnel handling sensitive data or performing security functions within 30 days of role assignment.
- **Shall** maintain training completion records for 3 years.

### F.6 Audits and Reviews
- **Shall** conduct internal ISMS audits **annually** with independent auditors reviewing compliance with policy requirements.
- **Shall** perform management reviews of the ISMS **quarterly** to assess effectiveness and identify improvement opportunities.
- **Shall** maintain audit findings, management review minutes, and corrective action plans for 3 years.

---

## G. Compliance and Monitoring

Compliance with this policy **shall** be monitored through **quarterly security reviews and control assessments** combined with **annual internal ISMS audits**. Non-compliance **shall** be addressed through documented corrective actions within 30 days. Violations may result in access revocation, mandatory corrective training, and disciplinary actions up to and including termination.

---

## H. Policy Exceptions

### H.1 Exception Request Process
Employees requiring temporary deviation from this policy **shall**:
1. Submit exception requests via the **ServiceNow GRC/ITSM ticketing workflow (or equivalent ticketing system)** with detailed business justification, risk assessment, and proposed compensating controls.
2. Obtain approval from the Information Security Officer for tactical exceptions (≤30 days) or CISO for strategic exceptions (>30 days).
3. Accept exceptions valid for a maximum of **90 days** unless formally renewed.
4. Document compensating controls implemented during the exception period.

### H.2 Exception Governance
- All active exceptions **shall** be reviewed **quarterly** by the Information Security Officer to confirm continued necessity.
- Exception renewals **shall** require updated business justification and CISO approval.
- Each exception **shall** include a remediation plan with target closure date not to exceed 180 days from initial approval.
- Exception tracking **shall** be maintained in the GRC platform with status updates provided to executive leadership **monthly**.

---

## I. Related Policies

This policy is supported by the following subordinate policies and procedures:

1. [**Access Control Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/access-control-policy.md) – Defines authentication mechanisms, authorization models (RBAC/ABAC), account lifecycle management (provisioning/deprovisioning), privileged access requirements, and access review procedures.

2. **Incident Management Policy** – Defines incident detection methods, classification criteria, response procedures, escalation paths, communication protocols, containment strategies, eradication steps, recovery processes, and post-incident review requirements.

3. **Risk Management Policy** – Defines risk assessment methodology, risk scoring criteria (likelihood × impact), risk appetite thresholds, treatment options (accept/mitigate/transfer/avoid), ownership assignment, and reporting cadence to executive leadership.

4. **Business Continuity and Disaster Recovery Policy** – Defines Recovery Time Objectives (RTO), Recovery Point Objectives (RPO), business impact analysis (BIA) methodology, continuity strategies, disaster recovery procedures, and testing requirements.

5. **Data Protection and Privacy Policy** – Defines data classification standards, handling requirements per classification level, retention schedules, disposal methods, privacy controls for PII/PHI, and regulatory compliance requirements.

---

## J. Related Documents

1. IT Security Procedures Manual
2. Incident Response Plan
3. Business Continuity Plan
4. Disaster Recovery Plan
5. Acceptable Use Policy

---

## K. Review and Revision

This policy **shall** be reviewed **annually** or when significant changes occur (regulatory updates, major security incidents, organizational restructuring, technology changes) to ensure its continued relevance and effectiveness. Revisions **shall** be made to address emerging threats, regulatory changes, and improvements in best practices. All revisions require CISO approval and executive leadership notification.

---

## L. Framework Alignment

| Framework | Alignment |
|-----------|-----------|
| **ISO/IEC 27001** | Information Security Management System (ISMS) implementation and certification requirements |
| **ISO/IEC 27017** | Security controls for cloud services, addressing cloud-specific threats and shared responsibility models |
| **ISO/IEC 27018** | Protection of personally identifiable information (PII) in public cloud environments |
| **ISO/IEC 27032** | Cybersecurity guidelines for improving security posture and resilience against cyber threats |
| **NIST Cybersecurity Framework** | Aligns with Identify, Protect, Detect, Respond, and Recover functions |

**Note:** This policy aligns to these standards; certification and compliance scope are defined in the ISMS Statement of Applicability (SoA).

---

## M. Organizational Benefit

| Benefit Area | Description |
|--------------|-------------|
| **Data Security** | Protects sensitive information from unauthorized access, disclosure, and modification through structured controls |
| **Cloud Service Security** | Establishes secure practices for cloud operations, ensuring safe delivery of services to global customers |
| **Customer Data Protection** | Builds trust with clients by demonstrating commitment to safeguarding their data through internationally recognized standards |
| **Cybersecurity Resilience** | Strengthens organizational defenses against evolving cyber threats through proactive risk management |
| **Regulatory Compliance** | Reduces legal and financial risk by aligning with global data protection regulations |
| **Operational Continuity** | Minimizes disruption from security incidents through defined response and recovery procedures |
| **Stakeholder Confidence** | Enhances reputation with customers, partners, and regulators through demonstrated security governance |

---

## N. Evidence of Compliance

The organization **shall** maintain the following compliance evidence with defined retention periods:

### Evidence Index

| Evidence Type | System of Record | Owner | Retention Period |
|---------------|------------------|-------|------------------|
| User Access Reviews | Identity Management System | IT Department | 3 years |
| Privileged Access Reviews | Identity Management System | IT Department | 3 years |
| Training Completion Records | Learning Management System (LMS) | Human Resources | 3 years |
| Policy Acknowledgements | GRC Platform / HR System | Human Resources | 3 years |
| Incident Tickets | ServiceNow ITSM | Information Security Team | 7 years |
| Incident Response Reports | ServiceNow / Document Repository | Information Security Team | 7 years |
| Risk Register | GRC Platform | Information Security Officer | Indefinite |
| Risk Assessment Reports | GRC Platform / Document Repository | Information Security Officer | 5 years |
| Business Impact Analysis (BIA) | GRC Platform / Document Repository | Business Continuity Manager | 5 years |
| BC/DR Test Results | Document Repository | Business Continuity Manager | 5 years |
| ISMS Certification | Document Repository | Information Security Officer | 7 years |
| Internal Audit Reports | GRC Platform / Document Repository | Internal Audit / ISO | 7 years |
| Penetration Test Reports | Document Repository | Information Security Officer | 5 years |
| Vendor Security Assessments | Vendor Management System | Procurement / IT | Contract + 3 years |

---

### N.1 Access Control Evidence
- **User Access Reviews:** Quarterly access certification reports exported from identity management system, showing account name, role, manager approval, and review date. Retained for 3 years.
- **Privileged Access Reviews:** Monthly privileged account audits with documented justification for continued access. Retained for 3 years.
- **Provisioning/Deprovisioning Records:** Service desk tickets showing access request, approval, implementation date, and system confirmations. Retained for 3 years.
- **Authentication Logs:** Multi-factor authentication (MFA) logs demonstrating successful and failed login attempts. Retained for 1 year.

### N.2 Training and Awareness Evidence
- **Training Completion Records:** Learning management system (LMS) reports showing employee name, course title, completion date, and pass/fail status. Retained for 3 years.
- **Onboarding Training Records:** New hire security awareness training completed within 7 days of start date. Retained for 3 years.
- **Role-Specific Training Records:** Evidence of specialized training for security personnel, administrators, and data handlers. Retained for 3 years.
- **Policy Acknowledgements:** Signed attestations (digital or physical) confirming employees have read, understood, and agree to comply with security policies. Retained for 3 years.

### N.3 Incident Management Evidence
- **Incident Tickets:** ServiceNow incident records showing detection timestamp, classification, severity, assigned owner, containment actions, resolution timestamp, and status. Retained for 7 years.
- **Incident Response Reports:** Detailed reports for high/critical incidents including timeline, root cause analysis, impact assessment, and lessons learned. Retained for 7 years.
- **Post-Incident Reviews:** Documentation of corrective actions implemented, effectiveness validation, and preventive measures. Retained for 7 years.
- **Security Event Logs:** SIEM (Security Information and Event Management) logs showing detection of suspicious activities and automated responses. Retained for 1 year.

### N.4 Risk Management Evidence
- **Risk Register:** Enterprise risk register maintained in GRC platform, updated quarterly, showing risk ID, description, owner, likelihood, impact, risk score, treatment decision, and status. Retained indefinitely.
- **Risk Assessments:** Quarterly risk assessment reports identifying new/changed threats, vulnerabilities, and corresponding controls. Retained for 5 years.
- **Risk Treatment Plans:** Documented mitigation strategies with assigned owners, target completion dates, and implementation evidence. Retained for 5 years.
- **Executive Risk Reports:** Monthly risk dashboard presented to leadership showing top risks, trending, and treatment progress. Retained for 5 years.

### N.5 Business Continuity Evidence
- **Business Impact Analysis (BIA):** Annual BIA reports identifying critical business processes, dependencies, RTO/RPO requirements, and resource needs. Retained for 5 years.
- **BC/DR Test Results:** Documentation of annual disaster recovery tests including test scenarios, participant lists, results, gaps identified, and remediation plans. Retained for 5 years.
- **Tabletop Exercise Records:** Sign-in sheets, scenario descriptions, participant responses, and improvement recommendations from annual BC exercises. Retained for 5 years.
- **Recovery Procedure Documentation:** Step-by-step recovery runbooks for critical systems with version control and approval history. Retained indefinitely (current version).

### N.6 Audit and Certification Evidence
- **ISMS Certification:** ISO/IEC 27001 certification documentation including certificate, audit reports, and corrective action responses. Retained for 7 years.
- **Internal Audit Reports:** Annual internal ISMS audit findings, severity classifications, remediation plans, and closure evidence. Retained for 7 years.
- **Management Review Minutes:** Quarterly ISMS management review meeting minutes documenting decisions, action items, and performance metrics. Retained for 7 years.
- **Penetration Test Reports:** Annual third-party penetration testing results showing vulnerabilities discovered, severity ratings, remediation recommendations, and closure status. Retained for 5 years.
- **Vulnerability Scan Results:** Monthly vulnerability scanning reports from automated tools with risk ratings and patch status. Retained for 1 year.

### N.7 Third-Party Management Evidence
- **Vendor Security Assessments:** Due diligence questionnaires, security reviews, and audit reports for vendors handling sensitive data. Retained for duration of contract + 3 years.
- **Vendor Contracts:** Executed agreements with security and compliance requirements, SLA terms, and data handling provisions. Retained for duration of contract + 7 years.
- **Vendor Performance Reviews:** Annual reviews of vendor security posture and compliance with contractual obligations. Retained for 5 years.

---

## Approval History

| Date | Approver | Status | Comments |
|------|----------|--------|----------|
| 2026-01-13 | Chief Information Security Officer | Approved | "Looks great. Approved." |

---

## Document Control

- **Document ID:** KB-PORTFOLIO-0003
- **Version:** 1.0
- **Classification:** Internal
- **Last Updated:** 2026-01-13
- **Next Review Date:** 2027-01-13

---

*This policy document was generated from ServiceNow GRC and formatted for portfolio presentation.*

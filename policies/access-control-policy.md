# Access Control Policy

**Emyzer Technology – Governance, Risk, and Compliance**

---

## Policy Metadata

| Attribute | Value |
|-----------|-------|
| **Policy Name** | Access Control Policy |
| **Type** | Policy |
| **Version** | 2.0 |
| **Parent Policy** | Information Security Policy |
| **Owner** | Information Security Officer (Susan Orwell) |
| **Owning Group** | App Engine Studio Users |
| **State** | Published |
| **Valid From** | 2026-01-13 |
| **Valid To** | 2027-01-13 |
| **Approvers** | Chief Information Security Officer |
| **Reviewers** | GRC Analyst |
| **Knowledge Base** | Governance, Risk, and Compliance |
| **Published Policy** | KB-PORTFOLIO-0004 |

---

> **Start here:** Policy Snapshot → Minimum Requirements (F) → Evidence Index (N)

---

## Description

**Purpose:** Establishes guidelines for managing access to information systems and data based on business and security requirements.

**Impact:** Ensures only authorized personnel have access to sensitive information, reducing unauthorized access and data breaches while supporting regulatory compliance (SOC 2, ISO 27001, GDPR, HIPAA, PCI-DSS, where applicable based on data residency, contracts, and processing activities).

**Relevant Models/Frameworks:** COBIT; RBAC/ABAC access models

---

## Policy Snapshot

| Dimension | Summary |
|-----------|---------|
| **Applies to** | All workforce members (employees, contractors, consultants, temporary staff) and third parties |
| **Covers** | All information systems, applications, networks, data repositories, and cloud platforms |
| **Review Cadence** | Quarterly access reviews for standard users; monthly reviews for privileged access |
| **Key Governance** | IT Security Team implements technical controls; Department Managers approve access; Employees safeguard credentials |
| **Exceptions Process** | ServiceNow workflow with ISO approval (≤30 days) or CISO approval (>30 days); maximum 60-day duration; monthly review of active exceptions |
| **Evidence Maintained** | Access request forms, role definitions, MFA records, authentication logs, access reviews, revocation records (all with defined retention periods) |

---

## A. Purpose

To establish guidelines and requirements for managing access to information systems and data within Emyzer Technology. This policy ensures confidentiality, integrity, and availability of information through effective access control measures aligned with COBIT, RBAC, and ABAC frameworks.

---

## B. Scope

This policy applies to all departments and activities within Emyzer Technology, including but not limited to:

- IT Security
- Human Resources
- Operations
- Finance
- Legal
- All third-party vendors and contractors

It encompasses all information systems, applications, networks, data repositories, cloud platforms, and physical access controls used by Emyzer Technology in its business.

**Third-party applicability:** Third parties accessing organizational systems or data shall meet equivalent access control requirements via contractual obligations and periodic security assessments.

---

## C. Definitions

| Term | Definition |
|------|------------|
| **COBIT (Control Objectives for Information and Related Technologies)** | A framework for developing, implementing, monitoring, and improving IT governance and management practices. |
| **RBAC (Role-Based Access Control)** | A method of regulating access to computer or network resources based on the roles of individual users within an enterprise. |
| **ABAC (Attribute-Based Access Control)** | An access control method granting rights through combined attribute policies, including user attributes, resource attributes, and environmental conditions. |
| **MFA (Multi-Factor Authentication)** | Identity verification requiring two or more distinct factors: something you know (password), something you have (device), or something you are (biometric). |
| **Least Privilege** | The principle of granting users only the minimum access necessary to perform their job functions. |
| **Need-to-Know** | Access is granted only when there is an active, legitimate business reason for the information. |
| **Privileged Access** | Elevated permissions granting administrative or system-level control over critical infrastructure, applications, or data. |
| **Access Certification** | Periodic review and validation of user access rights by authorized managers to ensure appropriateness. |
| **Separation of Duties** | Division of critical functions among multiple individuals to prevent fraud and error. |

---

## D. Policy Statement

Emyzer Technology adheres to structured access control measures to protect information assets. The organization shall:

1. **Grant access based on least privilege and need-to-know** principles to minimize exposure, with access rights assigned only for active business requirements.

2. **Implement role-based access control (RBAC)** to assign permissions based on documented job functions, with role definitions reviewed annually.

3. **Apply attribute-based access control (ABAC)** for dynamic, context-aware security decisions incorporating user location, device security posture, data sensitivity, and time-based restrictions.

4. **Require multi-factor authentication (MFA)** for all system and data access, with mandatory MFA enrollment completed within 7 days of account provisioning.

5. **Conduct regular access reviews** with standard user access reviewed quarterly and privileged access reviewed monthly to ensure appropriate access levels are maintained.

6. **Provision new access within 24 hours of approved request** and **deprovision access within 4 hours of HR/manager notification** of termination, role change, or access no longer required.

---

## E. Roles and Responsibilities

### E.1 Chief Information Security Officer (CISO)
Provides executive oversight of access control governance. Shall approve strategic access control exceptions, review access control metrics quarterly, and serve as the escalation point for access-related security incidents.

### E.2 Information Security Officer (ISO)
Shall oversee the access control program, ensure compliance with policy requirements through documented evidence and periodic assessments, and approve tactical access exceptions (≤30 days).

### E.3 IT Security Team
Shall implement and manage access control measures, including identity management systems, authentication mechanisms, and authorization frameworks. Shall conduct access reviews according to defined schedules, monitor access logs continuously, and enforce compliance with this policy.

### E.4 Department Managers
Shall identify role requirements for their teams through documented job-function analyses. Shall approve access requests within 24 hours based on business justification and job functions. Shall ensure team compliance with access control policies through quarterly attestation for departmental access appropriateness.

### E.5 Employees and Users
Shall adhere to access control policies, safeguard authentication credentials (passwords, MFA devices, biometric data), and report suspicious access activities or credential compromise immediately (within 1 hour of discovery).

---

## F. Minimum Access Control Requirements

The following requirements establish baseline access control standards. Detailed implementation procedures are maintained in the **IT Security Procedures Manual** and related operational documentation.

### F.1 Access Request and Approval
- Shall submit access requests via the ServiceNow ticketing workflow with documented business justification and manager approval.
- Department Managers shall review and approve requests within 24 hours based on role requirements and business need.
- IT Security Team shall configure access according to approved requests within 24 hours of approval.
- Shall maintain access request forms with approval signatures for 3 years.

### F.2 Role-Based Access Control (RBAC)
- Access rights shall be assigned based on predefined roles corresponding to job functions within the organization.
- Role definitions shall be documented with associated permissions, systems, data classifications, and business justification.
- Role definitions shall be reviewed annually with updates approved by Department Managers and the IT Security Team.
- Shall implement separation of duties controls for critical functions (financial transactions, code deployment, security administration).

### F.3 Attribute-Based Access Control (ABAC)
- Access decisions shall incorporate user attributes (role, department, clearance level), resource attributes (data classification, sensitivity), and environmental attributes (location, device security posture, time of access).
- Dynamic, context-aware controls shall adjust access based on risk factors, including geographic location (geo-fencing), device compliance status, network security zone, and resource sensitivity.
- Shall document ABAC policies with technical configurations reviewed annually.

### F.4 User Authentication
- All users shall authenticate using multi-factor authentication (MFA) combining at least two of the following factors: knowledge (password/PIN), possession (hardware token/authenticator app/SMS), or inherence (biometric).
- MFA shall be enforced for: all VPN connections, all cloud application access (Office 365, AWS, Azure, SaaS), all privileged access, all remote access to internal systems, and all access to systems processing sensitive data (Confidential or Restricted classification).
- Password policies shall require: minimum 12 characters, complexity (uppercase, lowercase, numbers, special characters), no reuse of last 24 passwords, and password changes upon suspected compromise, credential exposure in breach databases, or risk-triggered events. Password rotation is event-driven unless system constraints or regulatory obligations require a fixed cadence. Privileged credentials may be subject to tighter rotation requirements (such as 60-day expiration) based on system criticality and risk assessment.
- Shall provision MFA enrollment within 7 days of account creation,n with enrollment verification retained for 3 years.
- Failed authentication attempts shall trigger account lockout after 5 consecutive failures within 15 minutes, with automatic unlock after 30 minutes, or manual unlock by the IT Security Team.

### F.5 Privileged Access Management
- Privileged access shall be granted only when required for specific administrative functions with documented business justification.
- Privileged accounts shall be separate from standard user accounts with distinct credentials and elevated logging.
- Shall review privileged access monthly with manager attestation and access justification retained for 3 years.
- Privileged sessions shall be monitored and recorded with session logs retained for 3 years.
- Shall implement just-in-time (JIT) privileged access for temporary administrative needs with automatic de-escalation after defined time periods.

### F.6 Access Review and Certification
- Shall conduct quarterly access reviews for standard user access with manager certification of appropriateness.
- Shall conduct monthly access reviews for privileged access with enhanced scrutiny and justification.
- Access review reports shall document account name, role, systems accessed, manager approval, review date, and certification status.
- Shall remediate access review findings within 30 days for standard access and 15 days for privileged access.
- Shall retain access review documentation for 3 years.

### F.7 Access Revocation
- Shall revoke access within 4 hours of HR/manager notification of termination, role change, or access no longer required.
- Shall conduct periodic checks monthly to ensure timely revocation of unnecessary access and identify dormant accounts.
- Dormant accounts (inactive >90 days) shall be disabled automatically, with re-enablement requiring manager approval.
- Shall maintain access revocation records tied to termination or role change dates for 3 years.

### F.8 Account Lifecycle Management
- Shall provision new accounts within 24 hours of approved access request with documented confirmation to the requesting manager.
- Shall modify access within 24 hours of approved role change request with an audit trail of changes.
- Shall disable accounts within 4 hours upon notification of termination, extended leave (>30 days), or security incident involving the account.
- Shall delete disabled accounts after 90 days of retention unless required for legal hold, regulatory retention, or active investigation.
- Shall maintain account lifecycle documentation (creation, modifications, disablement, deletion) for 3 years.

### F.9 Service Account Management
- Service accounts (non-human accounts used by applications, scripts, or automated processes) shall have documented owners, business purpose, systems accessed, and a credential rotation schedule.
- Service account credentials shall be rotated every 90 days or immediately upon personnel changes affecting account ownership.
- Service accounts shall not be used for interactive login or personal access; violations trigger immediate investigation.
- Service account activity shall be logged with quarterly reviews of usage patterns and access appropriateness.
- Shall maintain service account inventory with quarterly validation of continued business need.

### F.10 Break-Glass Access
- Break-glass accounts (emergency access for crisis situations when normal authentication is unavailable) shall be established for critical systems with controlled, time-bound access.
- Break-glass account credentials shall be stored in secured physical/electronic safes with dual-custody access (two authorized individuals required).
- All break-glass account usage shall be logged, monitored in real-time, and reviewed within 24 hours of activation with mandatory incident ticket documentation.
- Break-glass accounts shall be tested quarterly to verify functionality with test activities documented.
- Credentials shall be rotated after each use and annually, even if unused.

### F.11 Remote Access Controls
- Remote access shall require a VPN connection with MFA before accessing internal systems or data.
- Remote access sessions shall time out after 30 minutes of inactivity, with re-authentication required.
- Remote access from high-risk countries or suspicious IP addresses shall trigger enhanced monitoring and may be blocked based on risk assessment.
- Personal devices accessing organizational resources shall meet minimum security baselines (OS patching, antivirus, encryption, screen lock) verified through endpoint management tools.

### F.12 Access Logging and Monitoring
- All access to information systems, applications, and data shall be logged with centralized log aggregation in SIEM.
- Access logs shall include: timestamp, username, source IP address, resource accessed, action performed (read/write/delete/modify), and success/failure status.
- Logs shall be retained for 1 year minimum (standard user access) and 3 years (privileged access, financial systems, regulated data).
- Access logs shall be monitored continuously with automated alerts for: failed authentication patterns, privilege escalation attempts, off-hours access to sensitive systems, geographic anomalies, and concurrent sessions from different locations.
- Log review findings shall be documented with investigation results and remediation actions retained for 3 years.

---

## G. Compliance and Monitoring

### G.1 Continuous Monitoring
Access logs and activities shall be monitored continuously to detect unauthorized access, anomalies, privilege escalation attempts, and suspicious authentication patterns in real time. SIEM (Security Information and Event Management) systems shall generate automated alerts for high-risk access events.

### G.2 Internal Audits
Shall conduct regular audits annually to ensure adherence to the access control policy and identify areas for improvement. Audit findings shall be documented with remediation plans and target closure dates.

### G.3 Performance Metrics
Key performance indicators (KPIs) shall track access control effectiveness, including:
- Percentage of accounts with MFA enabled (target: 100%)
- Average time to provision new access (target: <24 hours)
- Average time to deprovision access (target: <4 hours)
- Access review completion rate (target: 100% quarterly for standard, 100% monthly for privileged)
- Number of dormant accounts disabled (target: 100% >90 days inactive)
- Access control policy violations (target: trending downward)

### G.4 Enforcement
Non-compliance with this policy may result in access revocation, mandatory corrective training, and disciplinary actions up to and including termination of employment or contract.

---

## H. Policy Exceptions

### H.1 Exception Request Process
Employees requiring a temporary deviation from this policy shall:
1. Submit exception requests via the ServiceNow GRC/ITSM ticketing workflow with detailed business justification, risk assessment, and proposed compensating controls.
2. Obtain approval from the Information Security Officer for tactical exceptions (≤30 days) or the CISO for strategic exceptions (>30 days).
3. Accept exceptions valid for a maximum of 60 days unless formally renewed.
4. Document compensating controls implemented during the exception period.

### H.2 Exception Governance
- All active exceptions shall be reviewed monthly by the Information Security Officer to confirm continued necessity.
- Exception renewals shall require updated business justification and CISO approval.
- Each exception shall include a remediation plan with a target closure date not to exceed 120 days from initial approval.
- Exception tracking shall be maintained in the GRC platform with status updates provided to executive leadership quarterly.

---

## I. Related Policies

This policy is supported by the following subordinate policies and procedures:

1. **Information Security Policy** (parent document) – Establishes overarching security governance framework
2. **Risk Management Policy** – Defines risk assessment methodology for access control risks
3. **Incident Management Policy** – Defines procedures for responding to access-related security incidents
4. **Data Classification Policy** – Establishes data sensitivity levels informing access control decisions
5. **Third-Party/Vendor Risk Management Policy** – Extends access controls to external parties
6. **Security Awareness & Training Policy** – Defines training requirements for access control responsibilities

---

## J. Related Documents

1. IT Security Procedures Manual
2. Identity and Access Management (IAM) Standards
3. Privileged Access Management (PAM) Procedures
4. Account Provisioning and Deprovisioning Workflows
5. Access Review Procedures and Templates
6. [COBIT (Control Objectives for Information and Related Technologies)](https://www.isaca.org/resources/cobit)

---

## K. Review and Revision

This policy shall be reviewed annually or as necessary due to:

- Significant organizational changes
- Technology updates (new authentication mechanisms, IAM platforms)
- Regulatory changes (data protection laws, industry standards)
- Major security incidents involving access control failures
- Lessons learned from access reviews and audits

Revisions shall be approved by the policy owner and communicated to all employees within 14 days of approval.

---

## L. Framework Alignment

| Framework | Description | Alignment |
|-----------|-------------|-----------|
| **COBIT 2019** | IT Governance and Management Framework | DSS05.04 (Manage user identity and logical access), DSS05.05 (Manage physical access to IT assets), DSS06.03 (Manage roles, responsibilities, and access privileges) |
| **NIST SP 800-53 Rev. 5** | Security and Privacy Controls for Information Systems | AC-1 (Access Control Policy and Procedures), AC-2 (Account Management), AC-3 (Access Enforcement), AC-6 (Least Privilege), AC-7 (Unsuccessful Login Attempts), IA-2 (Identification and Authentication), IA-5 (Authenticator Management) |
| **ISO/IEC 27001:2022** | Information Security Management Systems | A.5.15 (Access control), A.5.16 (Identity management), A.5.17 (Authentication information), A.5.18 (Access rights), A.8.2 (Privileged access rights), A.8.3 (Information access restriction) |
| **NIST Cybersecurity Framework v1.1** | Cybersecurity Risk Management | PR.AC-1 (Identities and credentials are issued, managed, verified, revoked, and audited), PR.AC-3 (Remote access is managed), PR.AC-4 (Access permissions and authorizations are managed, incorporating least privilege and separation of duties), PR.AC-6 (Identities are proofed and bound to credentials) |
| **CIS Controls v8** | Critical Security Controls | 5.1 (Establish and maintain an inventory of accounts), 5.2 (Use unique passwords), 5.3 (Disable dormant accounts), 5.4 (Restrict administrator privileges to dedicated accounts), 6.1 (Establish an access granting process), 6.2 (Establish an access revoking process) |

**Note:** This policy aligns with these standards; certification and compliance scope are defined in the ISMS Statement of Applicability (SoA).

---

## M. Organizational Benefits

| Benefit Area | Description |
|--------------|-------------|
| **Risk Reduction** | Ensures only authorized personnel access sensitive information, reducing unauthorized access, data breaches, and insider threats |
| **Regulatory Compliance** | Supports compliance with SOC 2, ISO 27001, GDPR (where applicable based on data residency and customer contracts), HIPAA (for healthcare data processing), and PCI-DSS (for payment card data) through documented access controls and audit trails |
| **Clear Accountability** | Documented access decisions create audit trails establishing responsibility for data access and privileged operations |
| **Operational Efficiency** | Role-based access streamlines onboarding, reduces administrative overhead for access management, and accelerates provisioning |
| **Incident Response Support** | Access logging enables faster detection, investigation, and forensic analysis of security incidents |
| **Third-Party Risk Management** | Structured access controls extend to contractors and vendors, reducing external exposure and supply chain risk |
| **Business Continuity** | Proper access controls ensure authorized personnel can access critical systems during normal operations and disruptions |
| **Stakeholder Confidence** | Demonstrates commitment to protecting customer data and intellectual property through rigorous access governance |

---

## N. Evidence of Compliance

The organization shall maintain the following compliance evidence with defined retention periods:

### Evidence Index

| Evidence Type | System of Record | Owner | Retention Period |
|---------------|------------------|-------|------------------|
| Access Request Forms | ServiceNow ITSM | IT Security Team | 3 years |
| Role Definition Documents | Identity Management System | IT Security Team | Indefinite (current version) |
| ABAC Policy Configurations | Identity Management System | IT Security Team | Indefinite (current version) |
| MFA Enrollment Records | Identity Management System | IT Security Team | 3 years |
| Authentication Logs | SIEM / Identity Management System | IT Security Team | 1 year (standard), 3 years (privileged) |
| Access Review Reports | GRC Platform | IT Security Team | 3 years |
| Access Audit Documentation | GRC Platform | IT Security Team | 3 years |
| Access Logs | SIEM / System Logs | IT Security Team | 1 year (standard), 3 years (privileged) |
| Anomaly Detection Reports | SIEM | IT Security Team | 1 year |
| Access Revocation Records | ServiceNow ITSM | IT Security Team | 3 years |
| Service Account Inventory | GRC Platform / CMDB | IT Security Team | Indefinite (current version) |
| Break-Glass Account Test Reports | GRC Platform | IT Security Team | 3 years |
| Break-Glass Usage Logs | GRC Platform / SIEM | IT Security Team | 3 years |
| Remote Access Logs | VPN Logs / SIEM | IT Security Team | 1 year |
| Account Lifecycle Audit Trail | Identity Management System | IT Security Team | 3 years |
| Privileged Session Recordings | Privileged Access Management (PAM) | IT Security Team | 3 years |
| Dormant Account Reports | Identity Management System | IT Security Team | 1 year |

**Note:** Retention periods align with incident response, audit, and regulatory requirements. Critical security events involving privileged access are retained for **3 years minimum** to support forensic analysis and compliance obligations.


---

### N.1 Access Request and Provisioning Evidence
- **Access Request Forms:** ServiceNow tickets showing requester name, manager approval, business justification, requested systems/roles, approval date, and provisioning confirmation. Retained for 3 years.
- **Role Modification Requests:** Documented requests for role changes with manager approval and implementation date. Retained for 3 years.
- **Provisioning Timestamps:** System logs showing account creation date, provisioning completed date, and elapsed time from request to fulfillment. Retained for 3 years.

### N.2 Role-Based Access Control (RBAC) Evidence
- **Role Definition Documents:** Comprehensive documentation of each role, including role name, description, associated permissions, systems access, data classifications, separation of duties controls, and business justification. Retained indefinitely (current version with change history).
- **Role Assignment Matrix:** Mapping of users to assigned roles with effective dates and manager approval. Retained for 3 years.
- **Annual Role Review Reports:** Documentation of annual role definition reviews, including changes made, approvals, and rationale. Retained for 3 years.

### N.3 Attribute-Based Access Control (ABAC) Evidence
- **ABAC Policy Configurations:** Technical documentation of attribute-based access rules including user attributes (department, clearance level), resource attributes (data classification, sensitivity), environmental attributes (location, device posture, time), and policy logic. Retained indefinitely (current version with change history).
- **ABAC Policy Test Results:** Evidence of testing ABAC policies before production deployment. Retained for 3 years.
- **Annual ABAC Review Reports:** Documentation of annual ABAC policy reviews, including effectiveness assessment and updates. Retained for 3 years.

### N.4 Multi-Factor Authentication (MFA) Evidence
- **MFA Enrollment Records:** Documentation of user MFA enrollment, including user name, enrollment date, authentication method (SMS, authenticator app, hardware token), and enrollment verification. Retained for 3 years.
- **MFA Compliance Reports:** Monthly reports showing the percentage of users with MFA enabled by department and role. Retained for 1 year.
- **Authentication Logs:** System logs of successful and failed authentication attempts, including username, timestamp, IP address, device, MFA method, and success/failure status. Retained for 1 year (standard users), 3 years (privileged users).

### N.5 Access Review and Certification Evidence
- **Quarterly Access Review Reports:** Standard user access certification reports showing account name, role, systems accessed, data accessed, manager approval, review date, certification status (certified/revoked/modified), and reviewer comments. Retained for 3 years.
- **Monthly Privileged Access Review Reports:** Privileged account reviews with enhanced documentation, including business justification for continued access, recent privileged operations, and manager attestation. Retained for 3 years.
- **Access Review Remediation Tracking:** Documentation of findings from access review,s including accounts flagged for revocation/modification, remediation actions taken, completion dates, and verification. Retained for 3 years.

### N.6 Access Revocation Evidence
- **Access Revocation Records:** System logs showing account name, deprovisioning date, reason for revocation (termination, role change, access no longer needed), deprovisioning timestamp, and elapsed time from notification to revocation. Retained for 3 years.
- **Termination Checklists:** Documentation linking employee termination date to access revocation completion with sign-off from HR and IT Security. Retained for 3 years.
- **Dormant Account Reports:** Monthly reports identifying accounts inactive for >90 days with automatic disablement logs. Retained for 1 year.

### N.7 Privileged Access Management (PAM) Evidence
- **Privileged Access Inventory:** Comprehensive list of all privileged accounts, including account name, system, privileges granted, owner, business justification, and review date. Retained indefinitely (current version).
- **Privileged Session Recordings:** Video/keystroke recordings of privileged sessions for audit and forensic purposes. Retained for 3 years.
- **Just-in-Time (JIT) Access Logs:** Logs of temporary privilege escalation,s including requester, approver, elevation timestamp, de-escalation timestamp, and operations performed. Retained for 3 years.

### N.8 Security Monitoring Evidence
- **Access Anomaly Detection Reports:** SIEM-generated reports identifying unusual access patterns,s including off-hours access, geographic anomalies, privilege escalation attempts, and brute-force attacks. Retained for 1 year.
- **Access Control Violation Alerts:** Real-time alerts for unauthorized access attempts, failed authentication, and policy violations with incident ticket references. Retained for 1 year.
- **Access Audit Logs:** Comprehensive system logs of all access events, including user authentication, authorization decisions, resource access, and administrative actions. Retained for 1 year (standard users), 3 years (privileged users).

### N.9 Service Account Management Evidence
- **Service Account Inventory:** Comprehensive documentation of all service accounts, including account name, owner, business purpose, systems accessed, credential type, last rotation date, and review date. Retained indefinitely (current version with change history).
- **Service Account Credential Rotation Logs:** System logs documenting credential rotation events with rotation date, account name, and confirmation of successful update. Retained for 3 years.
- **Service Account Access Reviews:** Quarterly reviews validating continued business need, appropriate permissions, and owner confirmation. Retained for 3 years.

### N.10 Break-Glass Access Evidence
- **Break-Glass Account Inventory:** List of all break-glass accounts with system, custody arrangement, last test date, and last rotation date. Retained indefinitely (current version).
- **Break-Glass Usage Logs:** Detailed logs of all break-glass account activations, including activation timestamp, user identity, business justification, actions performed, and deactivation timestamp. Retained for 3 years (aligned with privileged access audit requirements).
- **Break-Glass Test Reports:** Quarterly test documentation showing test date, testers, functionality verification, and credential rotation confirmation. Retained for 3 years.

### N.11 Remote Access Evidence
- **VPN Access Logs:** Connection logs showing username, source IP, connection timestamp, disconnection timestamp, MFA verification, and data transferred. Retained for 1 year.
- **Device Compliance Reports:** Endpoint management reports showing device security posture (OS version, patch level, antivirus status, encryption status) for devices accessing organizational resources. Retained for 1 year.
- **Geographic Anomaly Alerts:** SIEM alerts for remote access from unusual or high-risk locations with investigation results. Retained for 1 year.

### N.12 Access Logging and Monitoring Evidence
- **Centralized Access Logs:** SIEM-aggregated logs of all access events across systems with timestamp, user, source, resource, action, and result. Retained for 1 year (standard), 3 years (privileged/financial/regulated).
- **Automated Alert Reports:** Real-time alerts for suspicious access patterns, including failed authentication, privilege escalation, off-hours access, and geographic anomalies, with incident disposition. Retained for 1 year.
- **Log Review Documentation:** Periodic manual reviews of access logs with findings, investigation notes, and remediation actions. Retained for 3 years.

### N.13 Performance Metrics Evidence
- **Access Control KPI Dashboards:** Monthly dashboards tracking MFA adoption rate, average provisioning time, average deprovisioning time, access review completion rate, dormant account percentage, and policy violation count. Retained for 1 year.
- **Trend Analysis Reports:** Quarterly reports showing access control performance trends and improvement initiatives. Retained for 3 years.

---

## Approval History

| Date | Approver | Status | Comments |
|------|----------|--------|----------|
| 2026-01-13 | Chief Information Security Officer | Approved | "The policy looks fantastic. I like how we're finally incorporating both RBAC & ABAC. Approved." |

---

## Revision History

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 1.0 | 2024-05-22 | Information Security Officer | Initial policy creation with RBAC/ABAC framework alignment |
| 2.0 | 2026-01-13 | Information Security Officer | Comprehensive rewrite into flagship portfolio format: added Policy Snapshot, enhanced minimum security requirements (service accounts, break-glass, remote access, logging), expanded evidence documentation with retention periods, strengthened exception governance, updated framework alignment, modernized password policy guidance |

---

## Document Control

- **Document ID:** KB-PORTFOLIO-0004
- **Version:** 2.0
- **Classification:** Internal
- **Last Updated:** 2026-01-13
- **Next Review Date:** 2027-01-13

---

*This policy document was generated from ServiceNow GRC and formatted for portfolio presentation.*

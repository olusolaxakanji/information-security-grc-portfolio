# Access Control Policy

**Emyzer Technology – ServiceNow GRC Policy Document**

---

## Policy Metadata

| Field | Value |
|-------|-------|
| **Policy Name** | Access Control Policy |
| **Type** | Policy |
| **Parent Policy** | Information Security Policy |
| **Owner** | Susan Orwell |
| **Owning Group** | App Engine Studio Users |
| **State** | Published |
| **Valid From** | 2024-05-22 |
| **Valid To** | 2025-05-22 |
| **Knowledge Base** | Governance, Risk, and Compliance |
| **KB Article** | KB0010005 |

---

## Description

**Purpose:** Establishes guidelines for managing access to information systems and data based on business and security requirements.

**Importance:** Ensures only authorized personnel have access to sensitive information, reducing the risk of unauthorized access.

**Relevant Frameworks:** COBIT, RBAC, and ABAC

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
- All third-party vendors and contractors

It encompasses all information systems, applications, and data repositories where Emyzer Technology conducts its business.

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

---

## D. Policy Statement

Emyzer Technology adheres to structured access control measures to protect information assets. The organization will:

1. **Grant access based on least privilege and need-to-know** principles to minimize exposure.
2. **Implement role-based access control (RBAC)** to assign permissions based on job functions.
3. **Apply attribute-based access control (ABAC)** for dynamic, context-aware security decisions.
4. **Require multi-factor authentication** for all system and data access.
5. **Conduct regular access reviews** to ensure appropriate access levels are maintained.

---

## E. Roles and Responsibilities

### IT Security Team
- Implement and manage access control measures
- Conduct access reviews and monitor access logs
- Enforce compliance with this policy

### Department Managers
- Identify role requirements for their teams
- Approve access requests based on job functions
- Ensure team compliance with access control policies

### Employees and Users
- Adhere to access control policies
- Safeguard authentication credentials
- Report suspicious access activities immediately

---

## F. Procedures

### F.1 Access Request and Approval
Submit an access request form to the IT Security Team. Department Managers review and approve requests based on role requirements. IT Security Team configures access according to approved requests.

### F.2 Role-Based Access Control (RBAC)
Access rights are assigned based on predefined roles corresponding to job functions within the organization. Role definitions are documented and reviewed annually.

### F.3 Attribute-Based Access Control (ABAC)
Access decisions incorporate user attributes, resource attributes, and environmental attributes. Dynamic, context-aware controls adjust access based on location, device, time, and resource sensitivity.

### F.4 User Authentication
All users must authenticate using secure methods, including multi-factor authentication (MFA), before accessing systems or data.

### F.5 Access Review and Audit
Conduct quarterly access reviews to ensure access levels remain appropriate. Perform annual audits to verify compliance with access control policies.

### F.6 Access Revocation
Revoke access immediately upon termination or role change of an employee. Conduct periodic checks to ensure timely revocation of unnecessary access.

---

## G. Compliance and Monitoring

### Continuous Monitoring
Monitor access logs and activities to detect unauthorized access and anomalies in real time.

### Internal Audits
Conduct regular audits to ensure adherence to the access control policy and identify areas for improvement.

### Enforcement
Non-compliance with this policy may result in disciplinary action including termination of employment or contract.

---

## H. Related Documents

1. Information Security Policy (parent document)
2. Risk Management Policy
3. Incident Management Policy
4. Data Classification Policy
5. Third-Party/Vendor Risk Management Policy
6. Security Awareness & Training Policy
7. [COBIT (Control Objectives for Information and Related Technologies)](https://www.isaca.org/resources/cobit)

---

## I. Review and Revision

This policy will be reviewed annually or as necessary due to:

- Significant organizational changes
- Technology updates
- Regulatory changes
- Major security incidents

Revisions will be approved by the policy owner and communicated to all employees.

---

## J. Framework Alignment

| Framework | Description | Alignment |
|-----------|-------------|-----------|
| **COBIT 2019** | IT Governance and Management Framework | DSS05.04 (Manage user identity and logical access), DSS05.05 (Manage physical access), DSS06.03 (Manage roles, responsibilities, and access privileges) |
| **NIST SP 800-53 Rev. 5** | Security and Privacy Controls | AC-1 (Policy and Procedures), AC-2 (Account Management), AC-3 (Access Enforcement), AC-6 (Least Privilege), IA-2 (Identification and Authentication) |
| **ISO/IEC 27001:2022** | Information Security Management | A.9.1 (Business requirements of access control), A.9.2 (User access management), A.9.3 (User responsibilities), A.9.4 (System and application access control) |
| **NIST Cybersecurity Framework** | Cybersecurity Risk Management | PR.AC (Identity Management, Authentication, and Access Control), PR.AC-1 (Identities and credentials managed), PR.AC-4 (Least privilege and separation of duties) |

---

## K. Organizational Benefits

Implementing this Access Control Policy provides Emyzer Technology with:

- **Risk Reduction:** Ensures only authorized personnel access sensitive information, reducing unauthorized access and data breaches
- **Regulatory Compliance:** Supports compliance with SOC 2, ISO 27001, and COBIT frameworks through documented access controls
- **Clear Accountability:** Documented access decisions create audit trails that establish responsibility for data access
- **Operational Efficiency:** Role-based access streamlines onboarding and reduces administrative overhead for access management
- **Incident Response Support:** Access logging enables faster detection and investigation of security incidents
- **Third-Party Risk Management:** Structured access controls extend to contractors and vendors, reducing external exposure

---

## L. Evidence of Compliance

| Evidence Type | Description | Frequency |
|---------------|-------------|-----------|
| Access Request Forms | Documented access request forms with manager approval signatures | Per request |
| Role Definition Documents | RBAC role definitions and permission mapping records | Annual review |
| ABAC Policy Configurations | Technical documentation of attribute-based access rules and configurations | Annual review |
| MFA Enrollment Records | Documentation of user enrollment in multi-factor authentication | Per user |
| Authentication Logs | System-generated logs of user authentication events | Continuous |
| Access Review Reports | Records of reviews validating appropriate access levels | Quarterly |
| Access Audit Documentation | Comprehensive audits verifying compliance with access control policies | Annual |
| Access Logs | System-generated logs of all access to information systems and data | Continuous |
| Anomaly Detection Reports | Reports identifying unauthorized access attempts and suspicious activity | Continuous |
| Access Revocation Records | Logs of access removal tied to termination or role change dates | Per event |

---

## Approval History

| Date | Approver | Status | Comments |
|------|----------|--------|----------|
| 2024-05-22 | Susan Orwell | Approved | "The policy looks fantastic. I like how we're finally incorporating both RBAC & ABAC. Approved." |

---

*This policy document was generated from ServiceNow GRC and formatted for portfolio presentation.*

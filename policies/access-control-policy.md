# Access Control Policy

**Emyzer Technology**

---

## Document Control

| Field | Details |
|-------|---------|
| **Policy Owner** | Susan Orwell |
| **Version** | 1.0 |
| **Effective Date** | May 22, 2024 |
| **Review Date** | May 22, 2025 |
| **Classification** | Internal |
| **Parent Policy** | Information Security Policy |

---

## A. Purpose

To establish guidelines and requirements for managing access to information systems and data within Emyzer Technology. This policy ensures confidentiality, integrity, and availability of information through effective access control measures aligned with COBIT, RBAC, and ABAC frameworks.

---

## B. Scope

This policy applies to all Emyzer Technology employees, contractors, vendors, and authorized users of Emyzer Technology's information systems and data. This includes all departments and activities related to access control management.

---

## C. Definitions

**COBIT (Control Objectives for Information and Related Technologies):** A framework for developing, implementing, monitoring, and improving IT governance and management practices.

**RBAC (Role-Based Access Control):** A method of regulating access to computer or network resources based on the roles of individual users within an enterprise.

**ABAC (Attribute-Based Access Control):** An access control method granting rights through combined attribute policies, including user attributes, resource attributes, and environmental conditions.

**MFA (Multi-Factor Authentication):** Identity verification requiring two or more distinct factors: something you know (password), something you have (device), or something you are (biometric).

**Least Privilege:** The principle of granting users only the minimum access necessary to perform their job functions.

**Need-to-Know:** Access is granted only when there is an active, legitimate business reason for the information.

---

## D. Policy Statement

Emyzer Technology is committed to protecting information assets through structured access control. All access to information systems and data shall be granted based on the principles of least privilege and need-to-know. Access decisions will incorporate both role-based and attribute-based controls to ensure dynamic, context-aware security.

---

## E. Roles and Responsibilities

**IT Security Team:** Implements and manages access control measures, conducts access reviews, monitors access logs, and enforces compliance with this policy.

**Department Managers:** Identifies role requirements, approves access requests based on job functions, and ensures team compliance with access control policies.

**All Employees and Users:** Adheres to access control policies, safeguards authentication credentials, and reports suspicious access activities immediately.

---

## F. Procedures

### F.1. Access Request and Approval

**F.1.1.** Submit an access request form to the IT Security Team.

**F.1.2.** Department Managers review and approve requests based on role requirements.

**F.1.3.** IT Security Team configures access according to approved requests.

### F.2. Role-Based Access Control (RBAC)

**F.2.1.** Access rights are assigned based on predefined roles corresponding to job functions within the organization.

**F.2.2.** Role definitions are documented and reviewed annually.

### F.3. Attribute-Based Access Control (ABAC)

**F.3.1.** Access decisions incorporate user attributes, resource attributes, and environmental attributes.

**F.3.2.** Dynamic, context-aware controls adjust access based on location, device, time, and resource sensitivity.

### F.4. User Authentication

**F.4.1.** All users must authenticate using secure methods, including multi-factor authentication (MFA), before accessing systems or data.

### F.5. Access Review and Audit

**F.5.1.** Conduct quarterly access reviews to ensure access levels remain appropriate.

**F.5.2.** Perform annual audits to verify compliance with access control policies.

### F.6. Access Revocation

**F.6.1.** Revoke access immediately upon termination or role change of an employee.

**F.6.2.** Conduct periodic checks to ensure timely revocation of unnecessary access.

---

## G. Compliance and Monitoring

The IT Security Team will monitor compliance with this policy through continuous monitoring of access logs and activities to detect unauthorized access and anomalies.

Non-compliance with this policy may result in disciplinary action including termination of employment or contract.

---

## H. Related Documents

### Internal Policies

- Information Security Policy (parent document)
- Risk Management Policy
- Incident Management Policy
- Data Classification Policy
- Third-Party/Vendor Risk Management Policy
- Security Awareness & Training Policy

### External Frameworks

- [COBIT (Control Objectives for Information and Related Technologies)](https://www.isaca.org/resources/cobit)

---

## I. Review and Revision

This policy will be reviewed and revised annually or as needed to address new risks, technologies, and compliance requirements. The IT Security Team is responsible for maintaining an up-to-date and effective policy.

---

## Framework Alignment

This policy addresses the following framework requirements:

**COBIT 2019 (Control Objectives for Information and Related Technologies):**
- DSS05.04: Manage user identity and logical access
- DSS05.05: Manage physical access to IT assets
- DSS06.03: Manage roles, responsibilities, access privileges, and levels of authority

**NIST SP 800-53 Rev. 5 (Security and Privacy Controls):**
- AC-1: Access Control Policy and Procedures
- AC-2: Account Management
- AC-3: Access Enforcement
- AC-6: Least Privilege
- AC-17: Remote Access
- IA-2: Identification and Authentication

**ISO/IEC 27001:2022 (Information Security Management):**
- A.9.1: Business requirements of access control
- A.9.2: User access management
- A.9.3: User responsibilities
- A.9.4: System and application access control

**NIST Cybersecurity Framework:**
- PR.AC (Identity Management, Authentication, and Access Control): Access to physical and logical assets is limited to authorized users, processes, and devices
- PR.AC-1: Identities and credentials are issued, managed, verified, revoked, and audited
- PR.AC-3: Remote access is managed
- PR.AC-4: Access permissions and authorizations are managed with least privilege and separation of duties

---

## Organizational Benefits

**Risk Reduction:** Ensures only authorized personnel access sensitive information, reducing the risk of unauthorized access and data breaches.

**Regulatory Compliance:** Supports compliance with SOC 2, ISO 27001, and COBIT frameworks through documented access controls.

**Clear Accountability:** Documented access decisions create audit trails that establish responsibility for data access.

**Operational Efficiency:** Role-based access streamlines onboarding and reduces administrative overhead for access management.

**Incident Response Support:** Access logging enables faster detection and investigation of security incidents.

**Third-Party Risk Management:** Structured access controls extend to contractors and vendors, reducing external exposure.

---

## Evidence of Compliance

| Evidence Type | Description | Frequency |
|---------------|-------------|-----------|
| Access Request Forms | Documented requests with manager approval signatures | Per request |
| Access Review Reports | Records of quarterly reviews validating appropriate access levels | Quarterly |
| Access Audit Documentation | Comprehensive audits verifying compliance with access control policies | Annual |
| Access Logs | System-generated logs of all access to information systems and data | Continuous |
| MFA Enrollment Records | Documentation of user enrollment in multi-factor authentication | Per user |
| Access Revocation Records | Logs of access removal tied to termination or role change dates | Per event |
| Role Definition Documents | Documented RBAC role definitions and associated permissions | Annual review |
| ABAC Policy Configurations | Technical documentation of attribute-based access rules | Annual review |

---

**Document History**

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 1.0 | May 22, 2024 | Susan Orwell | Initial policy creation, approved by policy owner |

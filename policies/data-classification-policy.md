# Data Classification Policy

**Emyzer Technology: Governance, Risk, and Compliance**

---

## Policy Metadata

| Attribute | Value |
|-----------|-------|
| **Policy Name** | Data Classification Policy |
| **Type** | Policy |
| **Owner** | Information Security Officer (Susan Orwell) |
| **Owning Group** | App Engine Admins |
| **State** | Published |
| **Valid From** | 2026-01-13 |
| **Valid To** | 2027-01-13 |
| **Approvers** | Chief Information Security Officer |
| **Reviewers** | GRC Analyst |
| **Knowledge Base** | Governance, Risk, and Compliance |
| **Published Policy** | KB-PORTFOLIO-0006 |

---

## Description

This policy establishes a framework for classifying information assets based on sensitivity, business value, and regulatory requirements to ensure appropriate protection throughout the data lifecycle.

**Impact:** Enables consistent data handling practices, supports regulatory compliance (GDPR, CCPA, PCI-DSS), reduces breach risk through appropriate controls, and optimizes security investment by aligning protection to data sensitivity.

**Relevant Standards:** ISO/IEC 27001 (A.5.12, A.5.13), NIST SP 800-53 (RA-2, SC-16), COBIT 2019 (APO01.06, DSS06.01)

---

## Policy Snapshot

| Dimension | Summary |
|-----------|---------|
| **Applies to** | All workforce members (employees, contractors, consultants, temporary staff) and third parties handling organizational data |
| **Covers** | All information assets regardless of format (digital, physical) or location (on-premises, cloud, third-party) |
| **Classification Levels** | Public, Internal, Confidential, Restricted (each with defined handling requirements) |
| **Review Cadence** | Annual review or upon major regulatory/organizational changes; data owners review classifications quarterly |
| **Key Governance** | Data Owners classify assets; Data Custodians implement controls; ISO provides oversight; CISO approves exceptions |
| **Exceptions Process** | ServiceNow workflow with ISO/CISO approval; maximum 90-day duration; quarterly review of active exceptions |
| **Evidence Maintained** | Data inventory, classification decisions, labeling audits, handling compliance records, disposal certificates (all with defined retention periods) |

---

## A. Purpose

To establish a consistent framework for classifying, labeling, and handling information assets based on their sensitivity, business value, and regulatory requirements. This policy ensures that appropriate security controls are applied throughout the data lifecycle, from creation to destruction, enabling Emyzer Technology to protect its information assets, meet compliance obligations, and optimize security investments.

---

## B. Scope

This policy applies to all employees, contractors, consultants, temporary staff, and third parties who create, collect, process, store, transmit, or dispose of information on behalf of Emyzer Technology. It encompasses all information assets regardless of format (electronic, physical, verbal) or storage location (on-premises systems, cloud services, third-party environments, removable media).

**Third-party applicability:** Third parties handling organizational data shall classify and protect data according to this policy via contractual requirements. Data shared with third parties shall retain its classification level and associated handling requirements.

---

## C. Definitions

1. **Data Classification:** The process of categorizing information based on its sensitivity, value, and criticality to determine appropriate protection levels.

2. **Data Owner:** The individual accountable for the classification, protection, and authorized use of specific data assets within their business domain.

3. **Data Custodian:** The individual or team responsible for implementing and maintaining technical controls to protect data as directed by the Data Owner.

4. **Data Steward:** The individual responsible for ensuring data quality, integrity, and compliance with classification requirements within assigned data domains.

5. **Personally Identifiable Information (PII):** Any information that can identify an individual directly or indirectly, including name, identification numbers, location data, and online identifiers.

6. **Sensitive Personal Data:** Special categories of personal data requiring enhanced protection, including health information, biometric data, racial/ethnic origin, and financial information.

---

## D. Policy Statement

Emyzer Technology requires all information assets to be classified according to their sensitivity and protected with controls appropriate to their classification level. To achieve this, the organization shall:

1. Establish and maintain a four-tier classification hierarchy: **Public, Internal, Confidential, and Restricted**.

2. Require Data Owners to classify all information assets within their domain **within 5 business days** of creation or acquisition.

3. Apply the **"highest classification applies"** principle when data of different classifications is combined.

4. Treat all unclassified data as **Internal** by default until formally assessed by an authorized Data Owner.

5. Maintain classification controls throughout the entire data lifecycle, including creation, storage, processing, transmission, and destruction.

6. Grant access to classified data only to individuals with a **legitimate business need** and appropriate authorization level.

7. Review data classifications **quarterly** by Data Owners to ensure continued accuracy, with reclassification requests processed within **10 business days**.

8. Label and mark classified information according to defined standards to enable proper identification and handling.

---

## E. Classification Levels

### E.1 Public (Level 1)

**Definition:** Information approved for unrestricted distribution with no adverse impact if disclosed.

**Examples:**
- Published marketing materials and press releases
- Public website content and job postings
- Annual reports intended for external stakeholders
- Product brochures and general company information

**Impact of Unauthorized Disclosure:** None or negligible.

### E.2 Internal (Level 2)

**Definition:** Information intended for internal business use that could cause minor harm if disclosed externally.

**Examples:**
- Internal policies, procedures, and guidelines
- Organizational charts and employee directories (non-sensitive)
- Internal meeting minutes and project documentation
- Non-sensitive operational reports

**Impact of Unauthorized Disclosure:** Minor operational inconvenience; limited reputational impact.

### E.3 Confidential (Level 3)

**Definition:** Sensitive information that could cause significant harm to Emyzer Technology, employees, customers, or partners if disclosed.

**Examples:**
- Customer data, contracts, and account information
- Financial records, forecasts, and pricing information
- Personally Identifiable Information (PII)
- Proprietary business processes and methodologies
- System architecture and security configurations
- Vendor agreements and contract terms

**Impact of Unauthorized Disclosure:** Significant financial loss; regulatory penalties; competitive disadvantage; legal liability; reputational damage.

### E.4 Restricted (Level 4)

**Definition:** Highly sensitive information requiring maximum protection, where unauthorized disclosure would cause severe or catastrophic harm.

**Examples:**
- Trade secrets and core intellectual property
- Protected Health Information (PHI)
- Payment card data (PCI scope)
- Encryption keys, certificates, and security credentials
- Merger and acquisition planning documents
- Executive strategic planning materials
- Critical security vulnerabilities (pre-remediation)

**Impact of Unauthorized Disclosure:** Severe financial loss; significant regulatory fines; existential business risk; legal prosecution; catastrophic reputational damage.

---

## F. Roles and Responsibilities

### F.1 Chief Information Security Officer (CISO)
Provides executive oversight of the data classification program. Shall approve strategic classification policy changes, exception requests exceeding 30 days, and risk acceptance decisions for Restricted data. Shall review classification program effectiveness **annually** as part of ISMS management review.

### F.2 Information Security Officer (ISO)
Shall develop, implement, and maintain the data classification framework under CISO direction. Shall review classification standards **annually** or upon regulatory changes. Shall approve tactical exceptions (≤30 days) and monitor classification compliance through quarterly audits.

### F.3 Data Owners
Shall classify information assets within their domain **within 5 business days** of creation or acquisition. Shall review classifications **quarterly** and upon significant changes to data use or regulatory requirements. Shall authorize access requests for their classified data **within 3 business days**. Shall report suspected misclassification or data incidents **within 24 hours** of discovery.

### F.4 Data Custodians (IT Department)
Shall implement technical controls based on classification requirements **within 10 business days** of assignment. Shall maintain encryption, DLP, and access control systems with **99.5% availability**. Shall execute secure disposal procedures **within 5 business days** of authorized request. Shall maintain classification-based access logs for defined retention periods.

### F.5 Data Stewards
Shall ensure data quality and integrity within assigned domains through **quarterly assessments**. Shall maintain the data inventory with current classification assignments, updated **within 5 business days** of changes. Shall coordinate with Legal and Compliance on regulatory classification requirements.

### F.6 All Employees
Shall complete data classification training **within 30 days** of hire and **annually** thereafter. Shall handle data according to its classification level and apply appropriate labels at the time of creation. Shall report suspected misclassification or policy violations **within 24 hours** of discovery.

---

## G. Minimum Security Requirements

### G.1 Requirements by Classification Level

| Control Domain | Public | Internal | Confidential | Restricted |
|----------------|--------|----------|--------------|------------|
| **Access Control** | None required | Role-based (RBAC) | Role-based + Manager approval | Individual approval + Executive authorization |
| **Authentication** | None required | Single-factor | Multi-factor (MFA) | MFA + Privileged Access Management |
| **Encryption at Rest** | None required | Recommended | Required (AES-128 minimum) | Required (AES-256) |
| **Encryption in Transit** | None required | TLS 1.2+ for external | TLS 1.2+ for all transmission | TLS 1.3 required |
| **Audit Logging** | None required | Authentication failures | All access and modifications | Comprehensive logging with SIEM integration |
| **DLP Monitoring** | None required | None required | Enabled | Real-time alerting with blocking |
| **Backup Encryption** | None required | Recommended | Required | Required with separate key management |
| **Data Masking** | None required | None required | Required in non-production | Required in all non-authorized views |

### G.2 Labeling Requirements

| Classification | Electronic Documents | Email | Physical Documents |
|----------------|---------------------|-------|-------------------|
| Public | None required | None required | None required |
| Internal | "INTERNAL USE ONLY" in header/footer | Subject line prefix: [INTERNAL] | "INTERNAL" watermark or stamp |
| Confidential | "CONFIDENTIAL" in header/footer with red text | Subject line prefix: [CONFIDENTIAL] | "CONFIDENTIAL" on every page |
| Restricted | "RESTRICTED" banner header/footer | Subject line prefix: [RESTRICTED]; encryption required | "RESTRICTED" with handling instructions on cover |

### G.3 Storage Requirements

| Classification | On-Premises | Cloud Services | Removable Media |
|----------------|-------------|----------------|-----------------|
| Public | No restrictions | Any cloud service | Permitted |
| Internal | Corporate systems | Approved cloud services | With manager approval |
| Confidential | Encrypted storage only | Approved cloud with encryption | Encrypted media only; ISO approval required |
| Restricted | Encrypted with access controls | Approved cloud with customer-managed keys | Prohibited without CISO approval |

### G.4 Transmission Requirements

| Classification | Internal Network | External Email | File Transfer |
|----------------|-----------------|----------------|---------------|
| Public | No restrictions | No restrictions | No restrictions |
| Internal | Standard protocols | Encryption recommended | Approved tools preferred |
| Confidential | Encrypted connections | Encrypted with DLP scan | Approved secure transfer tools only |
| Restricted | Encrypted and logged | Prohibited (use secure portal) | CISO-approved methods only |

### G.5 Disposal Requirements

| Classification | Electronic Media | Physical Documents | Disposal Verification |
|----------------|-----------------|-------------------|----------------------|
| Public | Standard deletion | Standard recycling | None required |
| Internal | Secure deletion (single overwrite) | Cross-cut shredding | None required |
| Confidential | DoD 5220.22-M or cryptographic erasure | Cross-cut shredding (witnessed) | Disposal log maintained |
| Restricted | Physical destruction or NIST SP 800-88 Purge | Witnessed destruction | Certificate of destruction required |

---

## H. Procedures

### H.1 Classification Procedure
1. **Identify:** Document the data type, source, business purpose, and responsible Data Owner.
2. **Assess:** Evaluate potential impact of unauthorized disclosure, modification, or loss across confidentiality, integrity, and availability.
3. **Determine Regulatory Requirements:** Identify applicable regulations (GDPR, CCPA, PCI-DSS, HIPAA) and contractual obligations.
4. **Assign Classification:** Select the appropriate level based on the highest impact assessment.
5. **Record:** Update the data inventory with classification, rationale, owner, and review date.
6. **Label:** Apply appropriate markings per labeling standards.
7. **Communicate:** Notify relevant stakeholders of classification and handling requirements.

### H.2 Reclassification Procedure
Reclassification is required when business use changes, regulatory requirements change, data sensitivity decreases due to time passage, or aggregation with other data increases sensitivity.

1. Data Owner submits reclassification request via ServiceNow with business justification.
2. Information Security reviews request **within 5 business days**.
3. If approved, Data Owner updates classification in data inventory.
4. Data Custodians adjust technical controls **within 10 business days**.
5. Stakeholders are notified of classification change.

### H.3 Third-Party Data Sharing Procedure
1. Data Owner confirms classification level and authorized sharing scope.
2. Legal/Procurement ensures contractual data protection requirements are in place.
3. Information Security validates third-party security controls meet classification requirements.
4. Data is transmitted using methods appropriate to classification level.
5. Data sharing is logged in the data inventory with recipient, date, and authorization reference.

---

## I. Compliance and Monitoring

Compliance with this policy shall be monitored through **quarterly classification audits** conducted by Information Security, combined with **continuous DLP monitoring** for Confidential and Restricted data. The ISO shall report classification compliance metrics to the CISO **monthly**.

**Monitoring Activities:**
- Quarterly data inventory reviews to verify classification accuracy
- Monthly DLP alert analysis for policy violations
- Annual labeling compliance audits (sample-based)
- Quarterly access reviews aligned to classification levels
- Annual third-party compliance assessments for data handlers

**Non-compliance** shall be addressed through documented corrective actions within **30 days**. Violations may result in access revocation, mandatory remedial training, and disciplinary actions up to and including termination. Willful mishandling of Restricted data may result in legal action.

---

## J. Policy Exceptions

### J.1 Exception Request Process
Employees requiring temporary deviation from this policy shall:
1. Submit exception requests via **ServiceNow GRC workflow** with detailed business justification, risk assessment, and proposed compensating controls.
2. Obtain approval from the Information Security Officer for exceptions involving Internal or Confidential data (≤30 days) or CISO for exceptions involving Restricted data or durations exceeding 30 days.
3. Accept exceptions valid for a maximum of **90 days** unless formally renewed.
4. Implement and document compensating controls during the exception period.

### J.2 Exception Governance
- All active exceptions shall be reviewed **quarterly** by the Information Security Officer.
- Exception renewals shall require updated business justification and risk assessment.
- Each exception shall include a remediation plan with a target closure date not exceeding **180 days** from initial approval.
- Exception tracking shall be maintained in the GRC platform with status updates provided to executive leadership **monthly**.

---

## K. Related Policies

This policy is supported by and supports the following policies:

1. [**Information Security Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/information-security-policy.md): Parent policy establishing the ISMS framework and governance structure.

2. [**Access Control Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/access-control-policy.md): Implements access requirements by classification level through RBAC/ABAC models and access review procedures.

3. [**Incident Management Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/incident-management-policy.md): Defines response procedures for data classification violations and data breach incidents.

4. [**Risk Management Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/risk-management-policy.md): Integrates classification-based risk assessment into enterprise risk management.

5. **Acceptable Use Policy**: Defines user responsibilities for handling classified information.

6. **Third-Party Risk Management Policy**: Establishes vendor requirements for protecting classified data.

---

## L. Related Documents

1. Data Inventory and Classification Register
2. Data Handling Procedures Manual
3. Encryption Standards and Key Management Procedures
4. Data Loss Prevention (DLP) Configuration Guide
5. Secure Disposal Procedures
6. Third-Party Data Sharing Agreement Template

---

## M. Review and Revision

This policy shall be reviewed **annually** or when significant changes occur (regulatory updates, major data incidents, organizational restructuring, technology changes) to ensure continued relevance and effectiveness. Classification levels and handling requirements shall be reviewed whenever new data types are introduced or regulatory requirements change. All revisions require CISO approval and notification to executive leadership.

---

## N. Framework Alignment

| Framework | Alignment |
|-----------|-----------|
| **ISO/IEC 27001** | A.5.12 (Classification of information), A.5.13 (Labelling of information), A.5.14 (Information transfer), A.7.10 (Storage media), A.8.10 (Information deletion) |
| **NIST SP 800-53** | RA-2 (Security Categorization), AC-16 (Security and Privacy Attributes), MP-4 (Media Storage), SC-16 (Transmission of Security Attributes) |
| **NIST Cybersecurity Framework** | ID.AM-5 (Resources are prioritized based on classification), PR.DS-1 (Data-at-rest is protected), PR.DS-2 (Data-in-transit is protected) |
| **COBIT 2019** | APO01.06 (Define information architecture), DSS05.02 (Manage identity and logical access), DSS06.01 (Align IT strategy with data classification) |
| **GDPR** | Article 5 (Principles relating to processing), Article 32 (Security of processing) |
| **PCI-DSS v4.0** | Requirement 3 (Protect stored account data), Requirement 4 (Protect cardholder data with strong cryptography during transmission) |

**Note:** This policy aligns with these standards; specific implementation controls are documented in the IT Security Procedures Manual.

---

## O. Organizational Benefit

| Benefit Area | Description |
|--------------|-------------|
| **Risk Reduction** | Applies appropriate controls to sensitive data, reducing breach likelihood and impact |
| **Regulatory Compliance** | Supports GDPR, CCPA, PCI-DSS, and HIPAA compliance through structured data handling |
| **Resource Optimization** | Focuses security investment on highest-value assets rather than uniform protection |
| **Operational Efficiency** | Provides clear handling guidance, reducing decision-making burden on employees |
| **Third-Party Trust** | Demonstrates structured data protection practices to customers and partners |
| **Incident Response** | Enables prioritized response based on data sensitivity when incidents occur |
| **Audit Readiness** | Maintains documented evidence of classification decisions and handling compliance |

---

## P. Evidence of Compliance

The organization shall maintain the following compliance evidence with defined retention periods:

### Evidence Index

| Evidence Type | System of Record | Owner | Retention Period |
|---------------|------------------|-------|------------------|
| Data Inventory | GRC Platform | Data Stewards | Indefinite (current version) |
| Classification Decisions | GRC Platform | Data Owners | Life of data + 3 years |
| Labeling Audit Reports | Document Repository | Information Security | 5 years |
| DLP Incident Reports | DLP Platform / SIEM | Information Security | 3 years |
| Access Authorization Records | Identity Management System | IT Department | 3 years |
| Training Completion Records | Learning Management System | Human Resources | 3 years |
| Disposal Certificates | Document Repository | Data Custodians | 7 years |
| Third-Party Assessments | Vendor Management System | Procurement / IT | Contract + 3 years |
| Exception Records | GRC Platform | Information Security | Exception duration + 3 years |
| Classification Audit Reports | GRC Platform | Information Security | 5 years |

---

### P.1 Data Inventory Evidence
- **Data Inventory Register:** Complete inventory maintained in GRC platform showing data asset name, description, owner, classification level, storage location, retention period, and last review date. Updated within 5 business days of changes.
- **Classification Decisions:** Documented rationale for each classification assignment, including impact assessment, regulatory considerations, and approving Data Owner. Retained for life of data plus 3 years.
- **Quarterly Review Records:** Evidence of Data Owner quarterly reviews showing assets reviewed, classification confirmations, and reclassification requests. Retained for 3 years.

### P.2 Labeling and Handling Evidence
- **Labeling Audit Reports:** Annual sample-based audits verifying electronic and physical documents bear appropriate classification markings. Findings, remediation plans, and closure evidence retained for 5 years.
- **DLP Incident Reports:** Records of policy violations detected by DLP systems, including incident details, classification involved, user, action taken, and resolution. Retained for 3 years.
- **Transmission Logs:** Logs of classified data transfers, particularly for Confidential and Restricted data sent externally. Retained for 1 year.

### P.3 Access Control Evidence
- **Access Authorization Records:** Service desk tickets and approval workflows for access to Confidential and Restricted data, showing requestor, Data Owner approval, and provisioning date. Retained for 3 years.
- **Quarterly Access Reviews:** Access certification reports showing users with access to classified data, their justification, and manager approval for continued access. Retained for 3 years.
- **Privileged Access Reviews:** Monthly reviews of accounts with access to Restricted data, including justification and CISO/executive approval. Retained for 3 years.

### P.4 Training Evidence
- **Training Completion Records:** LMS reports showing employee name, data classification training course, completion date, and assessment score. Retained for 3 years.
- **New Hire Training Records:** Evidence of classification training completed within 30 days of start date. Retained for 3 years.
- **Role-Specific Training:** Specialized training records for Data Owners, Data Stewards, and personnel handling Restricted data. Retained for 3 years.

### P.5 Disposal Evidence
- **Disposal Logs:** Records of data disposal requests, classification level, disposal method, execution date, and responsible party. Retained for 7 years.
- **Certificates of Destruction:** Third-party or witnessed destruction certificates for Confidential and Restricted data, including asset description, serial numbers (if applicable), destruction method, and date. Retained for 7 years.
- **Cryptographic Erasure Records:** Evidence of key destruction for encrypted media disposal. Retained for 7 years.

### P.6 Third-Party Evidence
- **Vendor Security Assessments:** Due diligence questionnaires and security reviews for vendors handling classified data, including classification levels they access and controls validated. Retained for contract duration plus 3 years.
- **Data Sharing Agreements:** Executed agreements specifying classification requirements, permitted use, and security obligations. Retained for contract duration plus 7 years.
- **Vendor Compliance Attestations:** Annual vendor attestations confirming continued compliance with classification handling requirements. Retained for 5 years.

### P.7 Exception and Audit Evidence
- **Exception Records:** Approved exception requests with business justification, risk assessment, compensating controls, approval chain, and expiration date. Retained for exception duration plus 3 years.
- **Classification Audit Reports:** Quarterly audit findings assessing classification accuracy, labeling compliance, handling adherence, and remediation tracking. Retained for 5 years.
- **Management Review Records:** Minutes from annual classification program review, including metrics, identified issues, and improvement actions. Retained for 5 years.

---

## Approval History

| Date | Approver | Status | Comments |
|------|----------|--------|----------|
| 2026-01-13 | Chief Information Security Officer | Approved | "Comprehensive framework that aligns with our ISMS and supports regulatory compliance. Approved for implementation." |

---

## Document Control

- **Document ID:** KB-PORTFOLIO-0006
- **Version:** 1.0
- **Classification:** Internal
- **Last Updated:** 2026-01-13
- **Next Review Date:** 2027-01-13

---

*This policy document was generated from ServiceNow GRC and formatted for portfolio presentation.*

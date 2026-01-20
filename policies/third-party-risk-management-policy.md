# Third-Party Risk Management Policy

**Emyzer Technology: Governance, Risk, and Compliance**

---

## Policy Metadata

| Attribute | Value |
|-----------|-------|
| **Policy Name** | Third-Party Risk Management Policy |
| **Type** | Policy |
| **Owner** | Information Security Officer (Susan Orwell) |
| **Owning Group** | App Engine Admins |
| **State** | Published |
| **Valid From** | 2026-01-13 |
| **Valid To** | 2027-01-13 |
| **Approvers** | Chief Information Security Officer |
| **Reviewers** | GRC Analyst |
| **Knowledge Base** | Governance, Risk, and Compliance |
| **Published Policy** | KB-PORTFOLIO-0008 |

---

## Description

This policy establishes a framework for identifying, assessing, managing, and monitoring risks associated with third-party vendors, suppliers, and service providers who access, process, store, or transmit Emyzer Technology information or provide critical services.

**Impact:** Reduces organizational exposure to supply chain risks, ensures vendor security practices meet organizational standards, supports regulatory compliance for third-party data handling, and protects against business disruption from vendor failures.

**Relevant Standards:** ISO/IEC 27001 (A.5.19 through A.5.23), NIST SP 800-53 (SA-9, SA-12, SR-1 through SR-12), NIST CSF (ID.SC), COBIT 2019 (APO10), SOC 2 Trust Services Criteria

---

## Policy Snapshot

| Dimension | Summary |
|-----------|---------|
| **Applies to** | All third parties who access organizational systems, process organizational data, or provide services critical to business operations |
| **Covers** | Vendor selection, due diligence, contracting, onboarding, ongoing monitoring, and offboarding across all third-party relationships |
| **Risk Tiers** | Critical, High, Medium, Low based on data access, system connectivity, and business criticality |
| **Review Cadence** | Annual policy review; vendor reassessment frequency based on risk tier (Critical: annual, High: annual, Medium: biennial, Low: triennial) |
| **Key Governance** | Procurement initiates engagements; ISO assesses security risk; Legal reviews contracts; business owners manage relationships; CISO approves Critical tier vendors |
| **Exceptions Process** | ServiceNow workflow with ISO/CISO approval; maximum 90 day duration; quarterly review of active exceptions |
| **Evidence Maintained** | Risk assessments, due diligence records, contracts, security certifications, audit reports, performance reviews (all with defined retention periods) |

---

## A. Purpose

To establish a comprehensive framework for managing risks associated with third-party relationships throughout the vendor lifecycle. This policy ensures that vendors, suppliers, contractors, and service providers meet Emyzer Technology security requirements, protect organizational data, maintain service quality, and comply with applicable regulations. Effective third-party risk management protects the organization from supply chain attacks, data breaches, service disruptions, regulatory penalties, and reputational damage.

---

## B. Scope

This policy applies to all third-party relationships where external entities:

- Access Emyzer Technology information systems or networks
- Process, store, or transmit organizational data (including customer data)
- Provide services critical to business operations
- Develop or maintain software or systems on behalf of the organization
- Have physical access to organizational facilities or data centers
- Provide cloud services, hosting, or infrastructure
- Supply hardware, software, or technology components
- Provide professional services with access to confidential information

**Third-party types covered:**
- Software vendors and SaaS providers
- Cloud service providers (IaaS, PaaS, SaaS)
- Managed service providers and outsourcing partners
- Consultants and contractors with system access
- Data processors and subprocessors
- Hardware suppliers and manufacturers
- Telecommunications providers
- Facilities and physical security providers
- Payment processors and financial service providers

**Exclusions:** Casual suppliers of commoditized goods with no data access or system connectivity may be excluded from full assessment requirements at the discretion of the ISO.

---

## C. Definitions

1. **Third Party:** Any external entity that provides products, services, or has access to organizational information, systems, or facilities.

2. **Vendor:** A third party that supplies goods or services under a contractual agreement.

3. **Service Provider:** A third party that delivers services (managed, professional, cloud, or outsourced) on behalf of the organization.

4. **Subcontractor/Subprocessor:** A third party engaged by a vendor to perform part of the contracted services, potentially with access to organizational data.

5. **Due Diligence:** The investigation and assessment process conducted before engaging a third party to evaluate their security posture, financial stability, and operational capabilities.

6. **Inherent Risk:** The level of risk posed by a third-party relationship before considering any mitigating controls.

7. **Residual Risk:** The level of risk remaining after security controls and contractual protections are applied.

8. **Fourth-Party Risk:** Risk arising from the third party's use of their own vendors and subcontractors who may access organizational data.

9. **Concentration Risk:** Risk arising from over-reliance on a single vendor or limited number of vendors for critical services.

---

## D. Policy Statement

Emyzer Technology requires all third-party relationships to be assessed, managed, and monitored commensurate with the risk they present to the organization. To achieve this, the organization shall:

1. Maintain a complete inventory of all third-party relationships with documented business owners and risk classifications.

2. Conduct risk-based due diligence **before** engaging any third party with access to organizational data or systems.

3. Classify all third parties into risk tiers (Critical, High, Medium, Low) based on data sensitivity, system access, and business criticality.

4. Require contractual security and privacy provisions appropriate to the risk tier and data classification involved.

5. Assess third-party security controls through questionnaires, certifications, audits, or assessments based on risk tier.

6. Monitor third-party performance, security posture, and compliance **continuously** for Critical tier and **periodically** for other tiers.

7. Require notification of security incidents affecting organizational data **within 24 hours** of discovery by the third party.

8. Conduct periodic reassessments of third-party risk at frequencies determined by risk tier.

9. Maintain documented procedures for third-party onboarding, ongoing management, and offboarding.

10. Review and update this policy **annually** to address evolving supply chain threats and regulatory requirements.

---

## E. Third-Party Risk Classification

### E.1 Risk Tier Criteria

Third parties shall be classified into risk tiers based on the following factors:

| Factor | Critical | High | Medium | Low |
|--------|----------|------|--------|-----|
| **Data Access** | Restricted data; large volumes of Confidential data | Confidential data | Internal data | Public data only or no data access |
| **System Access** | Direct access to production systems; privileged access | Network connectivity; application access | Limited system access; isolated environments | No system access |
| **Business Criticality** | Essential to core operations; no viable alternative | Important to operations; limited alternatives | Supports operations; alternatives available | Convenience services; easily replaceable |
| **Regulatory Impact** | Subject to direct regulatory oversight | Supports regulatory compliance | Minor compliance implications | No regulatory implications |

### E.2 Risk Tier Definitions

**Critical Tier:**
Third parties whose failure, breach, or compromise would cause severe operational disruption, significant regulatory penalties, or catastrophic reputational damage. Examples include primary cloud infrastructure providers, core banking/payment processors, and outsourced security operations.

**High Tier:**
Third parties with significant access to sensitive data or systems whose compromise would cause material harm. Examples include SaaS providers handling customer data, IT managed service providers, and software development partners.

**Medium Tier:**
Third parties with limited access to internal data or systems whose compromise would cause moderate, recoverable harm. Examples include HR software providers, marketing platforms with customer contact data, and professional consultants with project-specific access.

**Low Tier:**
Third parties with minimal or no access to sensitive data or systems whose compromise would cause minor inconvenience. Examples include office supply vendors, facilities maintenance providers (without data center access), and general professional services without data access.

### E.3 Risk Tier Requirements Summary

| Requirement | Critical | High | Medium | Low |
|-------------|----------|------|--------|-----|
| **Due Diligence Depth** | Comprehensive | Detailed | Standard | Basic |
| **Security Assessment** | On-site audit or SOC 2 Type II | SOC 2 or detailed questionnaire | Security questionnaire | Self-attestation |
| **Contract Requirements** | Full security schedule; audit rights; SLAs | Security schedule; audit rights | Standard security clauses | Basic terms |
| **Reassessment Frequency** | Annual | Annual | Every 2 years | Every 3 years |
| **Monitoring** | Continuous | Quarterly review | Semi-annual review | Annual review |
| **Incident Notification** | Within 24 hours | Within 24 hours | Within 48 hours | Within 72 hours |
| **Approval Authority** | CISO | ISO | Procurement + Business Owner | Business Owner |

---

## F. Third-Party Lifecycle Management

### F.1 Planning and Selection

Before engaging a third party:

1. **Business Owner** identifies business need and initiates vendor selection process.
2. **Procurement** identifies potential vendors and gathers preliminary information.
3. **ISO** conducts preliminary risk assessment to determine anticipated risk tier.
4. **Business Owner** evaluates vendor capabilities against business requirements.
5. **ISO** validates that security requirements appropriate to risk tier are included in RFP/RFQ.

### F.2 Due Diligence and Assessment

Before contract execution:

1. **Procurement** collects due diligence documentation from vendor.
2. **ISO** conducts security risk assessment appropriate to risk tier:
   - **Critical/High:** Comprehensive security questionnaire, review of SOC 2 Type II or equivalent, penetration test results, and business continuity plans
   - **Medium:** Standard security questionnaire and review of available certifications
   - **Low:** Basic security self-attestation
3. **Legal** reviews vendor contracts, privacy practices, and regulatory compliance.
4. **Finance** assesses vendor financial stability for Critical and High tier vendors.
5. **ISO** documents risk assessment findings and residual risk acceptance.
6. **Approval Authority** (per risk tier) approves or rejects vendor engagement.

### F.3 Contracting

All third-party contracts shall include provisions appropriate to the risk tier:

**All Tiers:**
- Confidentiality and non-disclosure obligations
- Data protection and security requirements
- Compliance with applicable laws and regulations
- Incident notification requirements
- Termination and transition provisions
- Insurance requirements (where applicable)

**Critical and High Tiers (additional requirements):**
- Right to audit or assess security controls
- Subcontractor/fourth-party approval requirements
- Service level agreements (SLAs) with remedies
- Business continuity and disaster recovery requirements
- Data return and destruction upon termination
- Liability and indemnification provisions
- Background check requirements for personnel with access

**Contracts involving personal data shall include:**
- Data processing agreement (DPA) compliant with GDPR/applicable regulations
- Defined purposes and limitations on data use
- Data subject rights support obligations
- Cross-border transfer mechanisms (where applicable)

### F.4 Onboarding

After contract execution:

1. **Procurement** records vendor in the third-party inventory with risk tier and business owner.
2. **IT** provisions vendor access according to principle of least privilege.
3. **ISO** validates security controls are implemented as agreed.
4. **Business Owner** provides vendor with relevant policies (Acceptable Use, Data Classification).
5. **IT** configures monitoring for vendor access and activities.
6. **Procurement** establishes performance monitoring and review schedule.

### F.5 Ongoing Monitoring and Management

During the relationship:

1. **Business Owner** monitors vendor performance against SLAs and business requirements.
2. **ISO** monitors vendor security posture through:
   - Review of updated certifications and audit reports
   - Periodic reassessments per risk tier schedule
   - Monitoring of vendor security ratings (for Critical tier)
   - Review of security incident notifications
3. **Procurement** manages contract compliance and renewal processes.
4. **IT** monitors vendor access logs and network activity.
5. **ISO** coordinates response to vendor security incidents affecting organizational data.

### F.6 Reassessment

Vendors shall be reassessed:

- Per the schedule defined by risk tier (Critical/High: annual; Medium: biennial; Low: triennial)
- Upon significant changes to scope of services or data access
- Following a security incident involving the vendor
- Upon notification of material changes to vendor security posture
- When regulatory requirements change

Reassessment shall include updated security questionnaire, review of current certifications, and validation that contractual requirements remain appropriate.

### F.7 Offboarding and Termination

Upon relationship termination:

1. **Business Owner** initiates termination process with defined end date.
2. **IT** revokes all vendor access to systems, networks, and facilities **within 24 hours** of termination date.
3. **IT** retrieves or disables any organizational equipment or credentials provided to vendor.
4. **Legal/Procurement** enforces data return and destruction obligations per contract.
5. **Vendor** provides certificate of data destruction within **30 days** of termination.
6. **ISO** validates access revocation and data destruction completion.
7. **Procurement** updates third-party inventory to reflect terminated status.
8. **Business Owner** retains vendor records per retention requirements.

---

## G. Fourth-Party and Subcontractor Management

### G.1 Fourth-Party Risk Requirements

Third parties shall:

1. Disclose material subcontractors and fourth parties who access organizational data or provide critical services.
2. Obtain written approval before engaging new subcontractors for Critical and High tier relationships.
3. Ensure subcontractors meet equivalent security requirements through flow-down provisions.
4. Maintain responsibility for subcontractor compliance with contractual obligations.
5. Notify Emyzer Technology of subcontractor security incidents affecting organizational data.

### G.2 Subcontractor Approval Process

For Critical and High tier vendors:

1. Vendor submits subcontractor request with business justification and security information.
2. ISO reviews subcontractor security posture and data access scope.
3. ISO approves or rejects subcontractor engagement **within 10 business days**.
4. Approved subcontractors are documented in the vendor record.

---

## H. Concentration and Continuity Risk

### H.1 Concentration Risk Management

The organization shall:

1. Identify single points of failure in the third-party portfolio.
2. Document alternative vendors or contingency plans for Critical tier services.
3. Avoid excessive reliance on single vendors for multiple critical services.
4. Monitor vendor financial stability and market position for concentration risks.
5. Report concentration risks to executive leadership **quarterly**.

### H.2 Business Continuity Requirements

Critical and High tier vendors shall:

1. Maintain documented business continuity and disaster recovery plans.
2. Test recovery capabilities **annually** and provide test results upon request.
3. Meet defined Recovery Time Objectives (RTO) and Recovery Point Objectives (RPO).
4. Notify Emyzer Technology of events affecting service continuity **within 4 hours**.
5. Participate in organization-led continuity exercises when requested.

---

## I. Incident Management

### I.1 Vendor Incident Notification Requirements

Third parties shall notify Emyzer Technology of security incidents:

| Risk Tier | Notification Timeframe | Notification Recipient |
|-----------|----------------------|------------------------|
| Critical | Within 24 hours | ISO and Business Owner |
| High | Within 24 hours | ISO and Business Owner |
| Medium | Within 48 hours | Business Owner (copied to ISO) |
| Low | Within 72 hours | Business Owner |

Notification shall include: nature of incident, data/systems affected, containment actions taken, and estimated impact.

### I.2 Incident Response Coordination

Upon vendor incident notification:

1. **ISO** assesses impact to organizational data and systems.
2. **ISO** coordinates with vendor on investigation and remediation.
3. **Legal** evaluates regulatory notification obligations.
4. **ISO** documents incident in the GRC platform.
5. **Business Owner** assesses business impact and communicates with stakeholders.
6. **ISO** conducts post-incident review and updates vendor risk assessment.

---

## J. Roles and Responsibilities

### J.1 Chief Information Security Officer (CISO)
Provides executive oversight of the third-party risk management program. Shall approve Critical tier vendor engagements, strategic policy changes, and risk acceptance decisions for vendors not meeting security requirements. Shall review program effectiveness **annually** as part of ISMS management review.

### J.2 Information Security Officer (ISO)
Shall develop, implement, and maintain the third-party risk management framework under CISO direction. Shall conduct or oversee security risk assessments for all tiers. Shall approve High tier vendor engagements. Shall monitor vendor security posture and coordinate incident response. Shall report third-party risk metrics to CISO **monthly**.

### J.3 Procurement
Shall manage vendor selection, contracting, and relationship administration. Shall maintain the third-party inventory with current status and business owners. Shall ensure contracts include required security provisions. Shall coordinate vendor onboarding and offboarding activities. Shall track contract renewals and trigger reassessments.

### J.4 Legal
Shall review and approve vendor contracts for legal sufficiency. Shall ensure data processing agreements comply with regulatory requirements. Shall advise on regulatory notification obligations following vendor incidents. Shall support contract negotiations for security and privacy terms.

### J.5 IT Department
Shall provision and deprovision vendor access according to approved requests. Shall implement technical controls to monitor and restrict vendor access. Shall maintain logs of vendor system activities. Shall support security assessments with technical validation.

### J.6 Business Owners
Shall identify business need for third-party engagements. Shall serve as primary relationship manager for assigned vendors. Shall monitor vendor performance against business requirements. Shall report vendor issues or incidents **within 24 hours** of discovery. Shall ensure vendor compliance with organizational policies.

### J.7 Finance
Shall assess vendor financial stability for Critical and High tier vendors. Shall review vendor insurance coverage and financial terms. Shall support evaluation of concentration risk.

---

## K. Compliance and Monitoring

### K.1 Program Monitoring

The third-party risk management program shall be monitored through:

- **Continuous:** Security rating monitoring for Critical tier vendors (where available)
- **Monthly:** ISO review of third-party inventory completeness and assessment status
- **Quarterly:** Executive reporting on third-party risk metrics and issues
- **Annual:** Comprehensive program effectiveness review as part of ISMS audit

### K.2 Key Performance Indicators

| KPI | Target | Measurement Frequency |
|-----|--------|----------------------|
| Third-party inventory completeness | 100% | Monthly |
| Vendors with current risk assessment | ≥95% | Monthly |
| Critical/High vendors with valid SOC 2 or equivalent | 100% | Quarterly |
| Overdue reassessments | <5% | Monthly |
| Average time to complete due diligence | <30 days | Monthly |
| Vendor incidents with timely notification | 100% | Per incident |
| Contracts with required security provisions | 100% | Quarterly |

### K.3 Non-Compliance

Non-compliance with this policy shall be addressed through:

- Escalation to CISO for unauthorized vendor engagements
- Remediation plans for vendors not meeting security requirements
- Contract renegotiation or termination for persistent non-compliance
- Disciplinary action for employees bypassing third-party risk processes

---

## L. Policy Exceptions

### L.1 Exception Request Process
Stakeholders requiring temporary deviation from this policy shall:
1. Submit exception requests via **ServiceNow GRC workflow** with detailed business justification, risk assessment, and proposed compensating controls.
2. Obtain approval from the Information Security Officer for Medium/Low tier exceptions or CISO for Critical/High tier exceptions.
3. Accept exceptions valid for a maximum of **90 days** unless formally renewed.
4. Implement and document compensating controls during the exception period.

### L.2 Exception Governance
- All active exceptions shall be reviewed **quarterly** by the Information Security Officer.
- Exception renewals shall require updated business justification and risk assessment.
- Each exception shall include a remediation plan with a target closure date not exceeding **180 days** from initial approval.
- Exception tracking shall be maintained in the GRC platform with status updates provided to executive leadership **monthly**.

---

## M. Related Policies

This policy is supported by and supports the following policies:

1. [**Information Security Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/information-security-policy.md): Parent policy establishing the ISMS framework and governance structure.

2. [**Access Control Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/access-control-policy.md): Defines access management requirements applicable to third-party access.

3. [**Data Classification Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/data-classification-policy.md): Defines data classification levels that determine third-party risk tier.

4. [**Incident Management Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/incident-management-policy.md): Defines response procedures for security incidents, including vendor-related incidents.

5. [**Risk Management Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/risk-management-policy.md): Integrates third-party risk into enterprise risk management.

6. [**Business Continuity and Disaster Recovery Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/bcdr-policy.md): Defines continuity requirements for critical vendors.

---

## N. Related Documents

1. Third-Party Risk Assessment Questionnaire
2. Vendor Security Requirements Checklist
3. Third-Party Inventory Register
4. Data Processing Agreement Template
5. Vendor Contract Security Schedule Template
6. Subcontractor Approval Request Form
7. Vendor Onboarding Checklist
8. Vendor Offboarding Checklist

---

## O. Review and Revision

This policy shall be reviewed **annually** or when significant changes occur (regulatory updates, major vendor incidents, organizational restructuring, supply chain threat landscape changes) to ensure continued relevance and effectiveness. The ISO shall assess policy effectiveness based on vendor risk metrics, incident trends, and audit findings. All revisions require CISO approval and notification to executive leadership.

---

## P. Framework Alignment

| Framework | Alignment |
|-----------|-----------|
| **ISO/IEC 27001** | A.5.19 (Information security in supplier relationships), A.5.20 (Addressing information security within supplier agreements), A.5.21 (Managing information security in the ICT supply chain), A.5.22 (Monitoring, review and change management of supplier services), A.5.23 (Information security for use of cloud services) |
| **NIST SP 800-53** | SA-9 (External System Services), SA-12 (Supply Chain Protection), SR-1 through SR-12 (Supply Chain Risk Management family) |
| **NIST Cybersecurity Framework** | ID.SC-1 through ID.SC-5 (Supply Chain Risk Management), ID.BE-1 (Supply chain role identified) |
| **COBIT 2019** | APO10.01 (Identify and evaluate supplier relationships), APO10.02 (Select suppliers), APO10.03 (Manage supplier relationships and contracts), APO10.04 (Manage supplier risk), APO10.05 (Monitor supplier performance) |
| **SOC 2** | CC9.2 (Risk from business partners and vendors) |
| **GDPR** | Article 28 (Processor), Article 32 (Security of processing) |
| **PCI DSS v4.0** | Requirement 12.8 (Manage service providers), Requirement 12.9 (Service provider acknowledgements) |

**Note:** This policy aligns with these standards; specific implementation controls are documented in the Third-Party Risk Management Procedures.

---

## Q. Organizational Benefit

| Benefit Area | Description |
|--------------|-------------|
| **Risk Reduction** | Systematic assessment and monitoring reduces exposure to supply chain attacks and vendor failures |
| **Regulatory Compliance** | Structured vendor management supports GDPR, PCI DSS, and industry requirements for third-party oversight |
| **Data Protection** | Contractual and technical controls ensure vendors protect organizational and customer data appropriately |
| **Operational Resilience** | Continuity requirements and concentration risk management reduce business disruption from vendor issues |
| **Informed Decision Making** | Risk-based approach enables leadership to make informed vendor selection and acceptance decisions |
| **Incident Preparedness** | Defined notification requirements and response procedures enable rapid response to vendor incidents |
| **Audit Readiness** | Documented assessments, contracts, and monitoring evidence demonstrate due diligence to auditors and regulators |

---

## R. Evidence of Compliance

The organization shall maintain the following compliance evidence with defined retention periods:

### Evidence Index

| Evidence Type | System of Record | Owner | Retention Period |
|---------------|------------------|-------|------------------|
| Third-Party Inventory | GRC Platform / Procurement System | Procurement | Indefinite (current version) |
| Risk Assessments | GRC Platform | Information Security | Contract + 5 years |
| Due Diligence Records | GRC Platform / Document Repository | Information Security | Contract + 5 years |
| Vendor Contracts | Contract Management System | Legal / Procurement | Contract + 7 years |
| Security Certifications (SOC 2, ISO) | Document Repository | Information Security | 3 years |
| Security Questionnaire Responses | GRC Platform | Information Security | 3 years |
| Performance Reviews | Procurement System | Procurement / Business Owner | 3 years |
| Incident Records | GRC Platform | Information Security | 7 years |
| Exception Records | GRC Platform | Information Security | Exception + 3 years |
| Offboarding Records | GRC Platform | Procurement | Contract + 5 years |

---

### R.1 Inventory and Classification Evidence
- **Third-Party Inventory:** Complete register of all third-party relationships maintained in GRC platform, showing vendor name, services provided, risk tier, business owner, contract dates, and assessment status. Updated within 5 business days of changes.
- **Risk Tier Classifications:** Documented risk tier assignments with supporting rationale based on data access, system connectivity, and business criticality. Retained for contract duration plus 5 years.
- **Concentration Risk Analysis:** Quarterly analysis identifying single points of failure and vendor dependencies. Retained for 5 years.

### R.2 Due Diligence Evidence
- **Security Risk Assessments:** Completed risk assessments documenting inherent risk, control evaluation, residual risk, and approval decisions. Retained for contract duration plus 5 years.
- **Security Questionnaire Responses:** Vendor-completed questionnaires with ISO review and findings. Retained for 3 years from assessment date.
- **Financial Assessments:** Financial stability reviews for Critical and High tier vendors. Retained for contract duration plus 3 years.
- **Reference Checks:** Documentation of reference checks conducted during vendor selection. Retained for contract duration plus 3 years.

### R.3 Certification and Audit Evidence
- **SOC 2 Reports:** Type II reports for Critical and High tier vendors, reviewed annually. Retained for 3 years.
- **ISO 27001 Certificates:** Certification evidence for vendors claiming ISO compliance. Retained for 3 years.
- **Penetration Test Results:** Third-party penetration test reports for Critical tier vendors (where provided). Retained for 3 years.
- **Audit Right Exercise Records:** Documentation of audits or assessments conducted under contractual audit rights. Retained for 5 years.

### R.4 Contract Evidence
- **Executed Contracts:** Signed vendor agreements with all schedules and amendments. Retained for contract duration plus 7 years.
- **Data Processing Agreements:** DPAs for vendors processing personal data. Retained for contract duration plus 7 years.
- **Security Schedules:** Contract exhibits specifying security requirements. Retained for contract duration plus 7 years.
- **Subcontractor Approvals:** Documentation of approved subcontractors for Critical and High tier vendors. Retained for contract duration plus 5 years.

### R.5 Monitoring Evidence
- **Reassessment Records:** Periodic reassessments per risk tier schedule, documenting any changes to risk posture. Retained for 3 years.
- **Performance Reviews:** Business owner reviews of vendor performance against SLAs and requirements. Retained for 3 years.
- **Security Rating Reports:** External security rating reports for Critical tier vendors (where utilized). Retained for 1 year.
- **Access Logs:** Logs of vendor access to organizational systems. Retained for 1 year.

### R.6 Incident Evidence
- **Vendor Incident Notifications:** Records of security incidents reported by vendors, including notification timeliness. Retained for 7 years.
- **Incident Investigation Records:** Documentation of incident investigation, impact assessment, and remediation. Retained for 7 years.
- **Post-Incident Reviews:** Lessons learned and vendor risk reassessments following incidents. Retained for 7 years.

### R.7 Lifecycle Evidence
- **Onboarding Records:** Documentation of vendor onboarding activities, including access provisioning and policy acknowledgement. Retained for contract duration plus 3 years.
- **Offboarding Records:** Documentation of termination activities, including access revocation and data destruction verification. Retained for contract duration plus 5 years.
- **Data Destruction Certificates:** Vendor-provided certificates confirming destruction of organizational data. Retained for 7 years.

### R.8 Exception and Governance Evidence
- **Exception Records:** Approved exception requests with business justification, risk assessment, compensating controls, and approval chain. Retained for exception duration plus 3 years.
- **Program Audit Reports:** Annual third-party risk management program assessments as part of ISMS audits. Retained for 5 years.
- **Executive Reports:** Quarterly reports to leadership on third-party risk metrics and issues. Retained for 5 years.

---

## Approval History

| Date | Approver | Status | Comments |
|------|----------|--------|----------|
| 2026-01-13 | Chief Information Security Officer | Approved | "Comprehensive third-party risk framework that addresses supply chain security requirements and supports our regulatory obligations. Approved for implementation." |

---

## Document Control

- **Document ID:** KB-PORTFOLIO-0008
- **Version:** 1.0
- **Classification:** Internal
- **Last Updated:** 2026-01-13
- **Next Review Date:** 2027-01-13

---

*This policy document was generated from ServiceNow GRC and formatted for portfolio presentation.*

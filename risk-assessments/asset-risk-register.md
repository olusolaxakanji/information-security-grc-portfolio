# Asset Risk Register

**Emyzer Technology - Governance, Risk, and Compliance Program**

---

## Document Information

| Attribute | Details |
|-----------|---------|
| **Document Title** | Asset Risk Register |
| **Document Type** | Risk Register |
| **Version** | 1.0 |
| **Effective Date** | 2024-05-22 |
| **Last Updated** | 2024-05-22 |
| **Owner** | Chief Information Security Officer (CISO) |
| **Classification** | Internal Use |

---

## 1. Purpose

The Asset Risk Register is the operational record of risks identified across Emyzer Technology's assets. It captures what could go wrong, how severe it would be, what we are doing about it, and who is accountable.

This register applies the scoring criteria, treatment options, and assessment process defined in the **Risk Assessment Methodology**. It does not duplicate that guidance. Instead, it puts the methodology into practice by documenting actual risks affecting real assets.

The register serves as:

- The single source of truth for asset-related risks across the organization
- The basis for executive reporting and risk-based decision making
- Evidence of a functioning risk management program for auditors and regulators
- A coordination tool connecting asset owners, risk owners, and treatment activities

---

## 2. Executive Summary

**Register snapshot as of 2024-05-22:**

| Risk Level | Count | Trend | Notes |
|------------|-------|-------|-------|
| Critical | 2 | Stable | Both in active treatment with executive oversight |
| High | 4 | Decreasing | Two risks reduced from Critical following Q1 control implementations |
| Medium | 6 | Increasing | Three new risks added from vendor assessment program |
| Low | 3 | Stable | Monitoring only; annual review scheduled |

**Key observations:**

The two critical risks both involve customer data exposure. One stems from legacy authentication weaknesses in the CRM system. The other relates to a cloud storage misconfiguration discovered during a recent security assessment. Both have funded treatment plans with target completion in Q3 2024.

The increase in medium risks reflects expanded visibility from the new vendor risk assessment program rather than deteriorating conditions. Previously unassessed third-party relationships are now documented and tracked.

**Decisions requiring attention:**

- RISK-2024-0047 (endpoint detection gap) requires budget approval for tooling. Deferred from Q1; risk owner requesting escalation.
- RISK-2024-0051 (key person dependency in security operations) has no viable mitigation. Formal acceptance recommended.

---

## 3. Asset Identification

### 3.1 Asset Categories

The register covers three asset categories:

**Information Assets.** Data requiring protection based on classification. Examples include customer records, employee data, financial information, intellectual property, and contractual documents.

**Technical Assets.** Systems that store, process, or transmit information. Examples include servers, cloud platforms, applications, databases, endpoints, and network infrastructure.

**Business Assets.** Processes, relationships, and capabilities that enable operations. Examples include critical workflows, vendor relationships, and key personnel.

### 3.2 Asset Ownership

Every asset has an assigned owner accountable for its protection and appropriate use. Asset owners participate in risk assessments, approve access, and escalate concerns. Ownership is assigned based on business accountability, not technical management.

The asset inventory is maintained in ServiceNow and feeds directly into this register.

---

## 4. Risk Register Structure

### 4.1 Field Definitions

| Field | Description |
|-------|-------------|
| **Risk ID** | Unique identifier for tracking and reference |
| **Asset Name** | The asset affected by this risk |
| **Asset Owner** | Individual accountable for the asset |
| **Asset Category** | Information, Technical, or Business asset classification |
| **Risk Description** | Narrative explaining the risk scenario and potential consequences |
| **Threat Source** | Origin of potential harm (adversarial, accidental, structural, environmental) |
| **Vulnerability** | Weakness that could be exploited |
| **Likelihood** | Probability rating per Risk Assessment Methodology |
| **Impact** | Consequence rating per Risk Assessment Methodology |
| **Risk Rating** | Calculated score and level (Critical, High, Medium, Low) |
| **Existing Controls** | Current measures reducing likelihood or impact |
| **Control Effectiveness** | Assessment of how well current controls perform |
| **Treatment Strategy** | Mitigate, Accept, Transfer, or Avoid |
| **Treatment Status** | Current state of risk response activities |
| **Risk Owner** | Individual accountable for managing this risk |
| **Target Date** | Expected completion for treatment activities |
| **Review Date** | Next scheduled reassessment |
| **Comments** | Additional context, decisions, and history |

### 4.2 Risk Status Values

| Status | Definition |
|--------|------------|
| Open | Identified and documented; treatment not yet planned |
| In Treatment | Mitigation activities underway |
| Monitoring | At acceptable level; ongoing observation |
| Accepted | Formally accepted by authorized individual |
| Closed | No longer applicable |

---

## 5. Risk Register

### RISK-2024-0042 | CRM System Authentication Weakness

| Field | Value |
|-------|-------|
| **Asset Name** | Customer Relationship Management (CRM) System |
| **Asset Owner** | Director of Sales Operations |
| **Asset Category** | Technical Asset |
| **Risk Description** | Unauthorized access to customer data through compromised credentials. The CRM contains contact information, purchase history, and support records for 50,000+ customers. Single-factor authentication makes accounts vulnerable to credential stuffing attacks using credentials leaked from other breaches. A successful attack could expose customer PII and damage trust. |
| **Threat Source** | Adversarial - External attacker |
| **Vulnerability** | Single-factor authentication; no detection of credential reuse |
| **Likelihood** | 4 (Likely) |
| **Impact** | 5 (Critical) - Regulatory notification required; reputational harm |
| **Risk Rating** | **20 - Critical** |
| **Existing Controls** | Password complexity requirements; account lockout after 5 failed attempts; quarterly access reviews |
| **Control Effectiveness** | Partial - Does not address credential reuse from external breaches |
| **Treatment Strategy** | Mitigate |
| **Treatment Status** | In Treatment |
| **Risk Owner** | IT Security Manager |
| **Target Date** | 2024-08-15 |
| **Review Date** | 2024-06-22 |
| **Comments** | MFA implementation approved in Q1 budget. Vendor selected (Okta). Pilot with sales team begins 2024-06-01. Full rollout targeted for August. Weekly status updates to CISO. |

---

### RISK-2024-0045 | Cloud Storage Misconfiguration

| Field | Value |
|-------|-------|
| **Asset Name** | AWS S3 Product Documentation Bucket |
| **Asset Owner** | VP of Engineering |
| **Asset Category** | Technical Asset |
| **Risk Description** | Sensitive product documentation exposed to unauthorized access due to overly permissive bucket policies. Security assessment discovered that internal API documentation and architecture diagrams were accessible without authentication. While not customer data, exposure could aid attackers in identifying system vulnerabilities. |
| **Threat Source** | Adversarial - External attacker; Accidental - Configuration error |
| **Vulnerability** | Misconfigured access policy allowing public read access |
| **Likelihood** | 5 (Almost Certain) - Actively exploitable |
| **Impact** | 4 (High) - Competitive disadvantage; aids future attacks |
| **Risk Rating** | **20 - Critical** |
| **Existing Controls** | None effective at time of discovery |
| **Control Effectiveness** | Ineffective |
| **Treatment Strategy** | Mitigate |
| **Treatment Status** | In Treatment |
| **Risk Owner** | Cloud Security Engineer |
| **Target Date** | 2024-06-01 |
| **Review Date** | 2024-06-15 |
| **Comments** | Immediate remediation: bucket policy corrected 2024-05-20. Broader remediation: implementing AWS Config rules to detect and auto-remediate public bucket policies. CloudTrail analysis underway to determine if unauthorized access occurred. No evidence of data exfiltration found to date. |

---

### RISK-2024-0038 | Ransomware Impact on Financial Systems

| Field | Value |
|-------|-------|
| **Asset Name** | Enterprise Resource Planning (ERP) System |
| **Asset Owner** | Chief Financial Officer |
| **Asset Category** | Technical Asset |
| **Risk Description** | Ransomware infection encrypts financial data and disrupts operations. The ERP system processes all financial transactions, payroll, and vendor payments. Extended unavailability would halt business operations and delay financial reporting. Recovery from backup could take 48-72 hours. |
| **Threat Source** | Adversarial - Ransomware operators |
| **Vulnerability** | Limited network segmentation; endpoint protection gaps on finance workstations |
| **Likelihood** | 3 (Possible) |
| **Impact** | 5 (Critical) - Business disruption; regulatory reporting delays |
| **Risk Rating** | **15 - High** |
| **Existing Controls** | Daily backups with 30-day retention; endpoint antivirus; email filtering |
| **Control Effectiveness** | Moderate - Backups tested quarterly; AV signatures may lag new variants |
| **Treatment Strategy** | Mitigate |
| **Treatment Status** | In Treatment |
| **Risk Owner** | IT Infrastructure Manager |
| **Target Date** | 2024-09-30 |
| **Review Date** | 2024-07-22 |
| **Comments** | Two-phase approach: (1) Network segmentation to isolate finance systems - in progress, 60% complete. (2) EDR deployment replacing legacy AV - vendor evaluation complete, procurement in progress. Risk reduced from Critical following backup immutability implementation in Q1. |

---

### RISK-2024-0047 | Endpoint Detection Gap

| Field | Value |
|-------|-------|
| **Asset Name** | Corporate Endpoint Fleet (Workstations and Laptops) |
| **Asset Owner** | Director of IT Operations |
| **Asset Category** | Technical Asset |
| **Risk Description** | Advanced threats evade signature-based antivirus on endpoints. Current AV solution relies on known malware signatures and cannot detect fileless attacks, living-off-the-land techniques, or zero-day exploits. Security team lacks visibility into endpoint behavior for threat hunting. |
| **Threat Source** | Adversarial - Advanced persistent threat; opportunistic attackers |
| **Vulnerability** | Reliance on signature-based detection only |
| **Likelihood** | 4 (Likely) |
| **Impact** | 4 (High) - Potential data breach; lateral movement |
| **Risk Rating** | **16 - Critical** |
| **Existing Controls** | Signature-based antivirus; host-based firewall; application allowlisting on critical systems |
| **Control Effectiveness** | Partial - Effective against known threats; blind to advanced techniques |
| **Treatment Strategy** | Mitigate |
| **Treatment Status** | Open - Awaiting Budget Approval |
| **Risk Owner** | IT Security Manager |
| **Target Date** | 2024-12-31 (if approved) |
| **Review Date** | 2024-06-22 |
| **Comments** | EDR solution (CrowdStrike or SentinelOne) proposed in Q1; deferred due to budget constraints. Risk owner requesting escalation to Risk Management Committee. Estimated cost: $180,000 annually. Compensating control: increased monitoring of high-risk users through SIEM. |

---

### RISK-2024-0031 | Third-Party Payment Processor Breach

| Field | Value |
|-------|-------|
| **Asset Name** | Payment Processing Vendor (PaymentCo) |
| **Asset Owner** | Director of Finance |
| **Asset Category** | Business Asset |
| **Risk Description** | Data breach at payment processor exposes customer payment information. PaymentCo processes all credit card transactions for Emyzer Technology's e-commerce platform. A breach at their environment could expose cardholder data, triggering PCI DSS notification requirements and potential fines even though the breach occurred externally. |
| **Threat Source** | Adversarial - Attack on third party |
| **Vulnerability** | Limited visibility into vendor security posture; contractual remedies only |
| **Likelihood** | 3 (Possible) |
| **Impact** | 4 (High) - PCI compliance implications; customer notification; reputational harm |
| **Risk Rating** | **12 - High** |
| **Existing Controls** | Annual SOC 2 Type II review; PCI DSS AOC on file; contractual security requirements; cyber insurance |
| **Control Effectiveness** | Moderate - Point-in-time assurance; limited real-time visibility |
| **Treatment Strategy** | Transfer (partial) and Mitigate |
| **Treatment Status** | Monitoring |
| **Risk Owner** | Vendor Risk Manager |
| **Target Date** | N/A - Ongoing monitoring |
| **Review Date** | 2024-08-22 |
| **Comments** | Cyber insurance provides $5M coverage for third-party breaches. Contract renewed 2024-03 with enhanced security addendum requiring 72-hour breach notification. Vendor added to continuous monitoring via SecurityScorecard. Current rating: A (87/100). |

---

### RISK-2024-0049 | Legacy Application End of Support

| Field | Value |
|-------|-------|
| **Asset Name** | Inventory Management System (Legacy) |
| **Asset Owner** | Director of Supply Chain |
| **Asset Category** | Technical Asset |
| **Risk Description** | Vendor ends support for inventory system in December 2024. After end-of-support, no security patches will be available. Known vulnerabilities will remain unaddressed, and compliance auditors will flag the unsupported software. System contains supplier information and inventory valuations. |
| **Threat Source** | Structural - Software end of life |
| **Vulnerability** | No security patches after December 2024 |
| **Likelihood** | 4 (Likely) - Vulnerabilities will emerge without remediation |
| **Impact** | 3 (Moderate) - Limited data sensitivity; workarounds available |
| **Risk Rating** | **12 - High** |
| **Existing Controls** | Network segmentation; restricted user access; enhanced monitoring |
| **Control Effectiveness** | Partial - Reduces but does not eliminate exposure |
| **Treatment Strategy** | Avoid |
| **Treatment Status** | In Treatment |
| **Risk Owner** | Director of Supply Chain |
| **Target Date** | 2024-11-30 |
| **Review Date** | 2024-07-22 |
| **Comments** | Replacement project approved. New system (NetSuite Inventory Module) implementation began 2024-04. Data migration scheduled for Q4. Legacy system decommission planned for November, ahead of support end date. |

---

### RISK-2024-0033 | Phishing Attack on Finance Team

| Field | Value |
|-------|-------|
| **Asset Name** | Finance Department User Accounts |
| **Asset Owner** | Chief Financial Officer |
| **Asset Category** | Information Asset |
| **Risk Description** | Finance team members targeted by sophisticated phishing attacks designed to steal credentials or initiate fraudulent wire transfers. Finance users have elevated access to banking systems and payment approval workflows. Successful business email compromise could result in direct financial loss. |
| **Threat Source** | Adversarial - Business email compromise actors |
| **Vulnerability** | Human susceptibility to social engineering |
| **Likelihood** | 4 (Likely) - Finance teams are high-value targets |
| **Impact** | 3 (Moderate) - Dual approval limits single-transaction loss |
| **Risk Rating** | **12 - High** |
| **Existing Controls** | Email filtering; MFA on banking systems; dual approval for transfers over $10,000; security awareness training |
| **Control Effectiveness** | Good - Multiple layers reduce likelihood and impact |
| **Treatment Strategy** | Mitigate |
| **Treatment Status** | Monitoring |
| **Risk Owner** | IT Security Manager |
| **Target Date** | N/A - Ongoing |
| **Review Date** | 2024-08-22 |
| **Comments** | Phishing simulation results improved from 18% click rate (2023-Q2) to 6% (2024-Q1) following targeted training. Finance team receives monthly simulations versus quarterly for general population. Verbal verification procedure implemented for wire transfer requests. |

---

### RISK-2024-0052 | Customer Data in Development Environment

| Field | Value |
|-------|-------|
| **Asset Name** | Development and Test Environments |
| **Asset Owner** | VP of Engineering |
| **Asset Category** | Technical Asset |
| **Risk Description** | Production customer data copied to development environments for testing purposes. Development environments have weaker access controls and are accessible to contractors. Data includes names, email addresses, and purchase history. Exposure would trigger breach notification requirements. |
| **Threat Source** | Accidental - Developer access; Adversarial - Contractor misuse |
| **Vulnerability** | Production data in lower-security environment |
| **Likelihood** | 3 (Possible) |
| **Impact** | 3 (Moderate) - PII exposure; notification required |
| **Risk Rating** | **9 - Medium** |
| **Existing Controls** | Contractor background checks; NDA agreements; access logging |
| **Control Effectiveness** | Partial - Does not prevent exposure, only provides accountability |
| **Treatment Strategy** | Mitigate |
| **Treatment Status** | In Treatment |
| **Risk Owner** | Engineering Manager |
| **Target Date** | 2024-07-31 |
| **Review Date** | 2024-07-22 |
| **Comments** | Data masking solution (Delphix) approved. Implementation in progress. Policy update drafted prohibiting production data in non-production environments without masking. Target: all PII masked in dev/test by end of Q3. |

---

### RISK-2024-0054 | HR System Vendor Security Weakness

| Field | Value |
|-------|-------|
| **Asset Name** | Human Resources Information System (Workday) |
| **Asset Owner** | Chief Human Resources Officer |
| **Asset Category** | Technical Asset |
| **Risk Description** | SaaS HR system vendor experiences security incident affecting tenant data. System contains sensitive employee information including SSN, compensation, performance reviews, and benefits elections. Vendor breach could expose entire workforce PII. |
| **Threat Source** | Adversarial - Attack on third party |
| **Vulnerability** | Reliance on vendor security controls |
| **Likelihood** | 2 (Unlikely) - Vendor has strong security posture |
| **Impact** | 4 (High) - Employee PII exposure; regulatory notification |
| **Risk Rating** | **8 - Medium** |
| **Existing Controls** | Vendor SOC 2 Type II annually; SSO integration; data encryption; cyber insurance |
| **Control Effectiveness** | Good - Mature vendor with demonstrated security program |
| **Treatment Strategy** | Transfer (partial) and Accept (residual) |
| **Treatment Status** | Monitoring |
| **Risk Owner** | Vendor Risk Manager |
| **Target Date** | N/A - Ongoing monitoring |
| **Review Date** | 2025-02-22 |
| **Comments** | Workday maintains strong security posture. Latest SOC 2 report (2024-01) showed no exceptions. Contract includes breach notification within 24 hours and indemnification. SecurityScorecard rating: A (92/100). Residual risk accepted by CHRO. |

---

### RISK-2024-0055 | Website Availability During Peak Sales

| Field | Value |
|-------|-------|
| **Asset Name** | E-commerce Website |
| **Asset Owner** | Director of Digital Commerce |
| **Asset Category** | Technical Asset |
| **Risk Description** | Website becomes unavailable during peak sales periods due to traffic surge or DDoS attack. Black Friday and holiday promotions generate 10x normal traffic. Extended outage during peak period would result in significant lost revenue and customer frustration. |
| **Threat Source** | Structural - Capacity exhaustion; Adversarial - DDoS attack |
| **Vulnerability** | Infrastructure scaling limitations; DDoS mitigation not tested at scale |
| **Likelihood** | 3 (Possible) |
| **Impact** | 3 (Moderate) - Revenue loss estimated at $50K per hour during peak |
| **Risk Rating** | **9 - Medium** |
| **Existing Controls** | Auto-scaling configured; CDN (CloudFront); basic DDoS protection (AWS Shield Standard) |
| **Control Effectiveness** | Moderate - Not tested at 10x load; Shield Standard has limitations |
| **Treatment Strategy** | Mitigate |
| **Treatment Status** | In Treatment |
| **Risk Owner** | Site Reliability Engineering Lead |
| **Target Date** | 2024-10-15 |
| **Review Date** | 2024-09-22 |
| **Comments** | Load testing scheduled for Q3 to validate scaling at 15x baseline. Evaluating AWS Shield Advanced for enhanced DDoS protection. Runbook being developed for traffic surge response. Must complete before November peak season. |

---

### RISK-2024-0051 | Key Person Dependency in Security Operations

| Field | Value |
|-------|-------|
| **Asset Name** | Security Operations Function |
| **Asset Owner** | Chief Information Security Officer |
| **Asset Category** | Business Asset |
| **Risk Description** | Single security engineer holds critical knowledge of SIEM configuration, incident response procedures, and threat detection rules. Unplanned departure would significantly degrade security monitoring and response capabilities. No backup resource currently trained. |
| **Threat Source** | Structural - Key person dependency |
| **Vulnerability** | Knowledge concentration; insufficient cross-training |
| **Likelihood** | 3 (Possible) |
| **Impact** | 3 (Moderate) - Degraded security posture; response delays |
| **Risk Rating** | **9 - Medium** |
| **Existing Controls** | Documentation requirements; managed SIEM vendor support available |
| **Control Effectiveness** | Partial - Documentation exists but is incomplete; vendor support is reactive |
| **Treatment Strategy** | Accept |
| **Treatment Status** | Pending Acceptance |
| **Risk Owner** | IT Security Manager |
| **Target Date** | N/A |
| **Review Date** | 2024-06-22 |
| **Comments** | Cross-training would require hiring additional security staff. Budget request for second security engineer denied in 2024 planning cycle. CISO recommends formal acceptance with compensating measures: (1) prioritize documentation completion, (2) establish retainer with IR firm for surge support, (3) revisit headcount in 2025 planning. Acceptance decision pending Risk Management Committee review. |

---

### RISK-2024-0039 | Backup Restoration Failure

| Field | Value |
|-------|-------|
| **Asset Name** | Enterprise Backup Infrastructure |
| **Asset Owner** | Director of IT Operations |
| **Asset Category** | Technical Asset |
| **Risk Description** | Backup restoration fails when needed during disaster recovery or ransomware event. Backups complete successfully but restoration has not been tested for all critical systems. Untested backups may be corrupted, incomplete, or take longer to restore than RTO allows. |
| **Threat Source** | Structural - Process gap |
| **Vulnerability** | Infrequent restoration testing |
| **Likelihood** | 2 (Unlikely) |
| **Impact** | 4 (High) - Extended outage if backups fail |
| **Risk Rating** | **8 - Medium** |
| **Existing Controls** | Daily backup jobs with success monitoring; quarterly restore tests for select systems |
| **Control Effectiveness** | Partial - Not all critical systems tested; full environment recovery not validated |
| **Treatment Strategy** | Mitigate |
| **Treatment Status** | Monitoring |
| **Risk Owner** | IT Infrastructure Manager |
| **Target Date** | N/A - Ongoing improvement |
| **Review Date** | 2024-11-22 |
| **Comments** | Annual DR exercise scheduled for Q4 will include full restoration test of critical systems. Restore test coverage expanded in 2024 from 5 systems to 12 systems quarterly. Immutable backup copy implemented Q1 to protect against ransomware encryption. |

---

### RISK-2024-0056 | Unauthorized Software Installation

| Field | Value |
|-------|-------|
| **Asset Name** | Corporate Endpoint Fleet |
| **Asset Owner** | Director of IT Operations |
| **Asset Category** | Technical Asset |
| **Risk Description** | Employees install unauthorized software that introduces vulnerabilities or malware. Users with local administrator rights can install browser extensions, utilities, and applications that bypass security controls. Shadow IT creates unmanaged attack surface. |
| **Threat Source** | Accidental - User behavior; Adversarial - Malware disguised as legitimate software |
| **Vulnerability** | Local administrator rights; lack of application control |
| **Likelihood** | 3 (Possible) |
| **Impact** | 2 (Low) - Individual endpoint compromise; limited lateral movement |
| **Risk Rating** | **6 - Medium** |
| **Existing Controls** | Antivirus scanning; user awareness training; prohibited software policy |
| **Control Effectiveness** | Partial - Policy exists but enforcement is limited |
| **Treatment Strategy** | Mitigate |
| **Treatment Status** | Monitoring |
| **Risk Owner** | IT Security Manager |
| **Target Date** | N/A - Phased approach |
| **Review Date** | 2025-02-22 |
| **Comments** | Full application allowlisting not feasible for engineering workstations. Phased approach: (1) Remove local admin for non-technical staff - completed 2024-Q1, (2) Implement software request process - in progress, (3) Deploy application control on high-risk systems - planned 2025. Current focus on detection rather than prevention. |

---

### RISK-2024-0029 | Physical Security of Server Room

| Field | Value |
|-------|-------|
| **Asset Name** | On-Premises Data Center |
| **Asset Owner** | Director of IT Operations |
| **Asset Category** | Technical Asset |
| **Risk Description** | Unauthorized physical access to server room results in theft, tampering, or sabotage. Server room contains production systems, backup infrastructure, and network equipment. Physical access could bypass logical controls entirely. |
| **Threat Source** | Adversarial - Insider or intruder; Accidental - Tailgating |
| **Vulnerability** | Single-factor access control (badge only) |
| **Likelihood** | 2 (Unlikely) |
| **Impact** | 3 (Moderate) - Equipment theft; potential data access |
| **Risk Rating** | **6 - Medium** |
| **Existing Controls** | Badge access; visitor sign-in; security camera coverage |
| **Control Effectiveness** | Moderate - Deters casual access; determined attacker could bypass |
| **Treatment Strategy** | Accept |
| **Treatment Status** | Accepted |
| **Risk Owner** | Facilities Manager |
| **Target Date** | N/A |
| **Review Date** | 2025-05-22 |
| **Comments** | Biometric access control evaluated; cost ($45K) exceeds risk reduction benefit given planned cloud migration. Risk accepted by Director of IT Operations (2024-03-15). Compensating measures: camera retention increased to 90 days; quarterly access list review implemented. Will reassess if cloud migration timeline extends beyond 2025. |

---

### RISK-2024-0058 | Email System Outage

| Field | Value |
|-------|-------|
| **Asset Name** | Microsoft 365 Email Service |
| **Asset Owner** | Director of IT Operations |
| **Asset Category** | Technical Asset |
| **Risk Description** | Email service becomes unavailable due to Microsoft outage or configuration error. Email is critical for internal and external communication. Extended outage would disrupt sales, customer support, and general operations. |
| **Threat Source** | Structural - Vendor outage; Accidental - Administrative error |
| **Vulnerability** | Dependence on single email platform |
| **Likelihood** | 2 (Unlikely) - Microsoft has strong availability record |
| **Impact** | 2 (Low) - Temporary disruption; workarounds available |
| **Risk Rating** | **4 - Low** |
| **Existing Controls** | Microsoft SLA (99.9%); change management for configuration; mobile access as backup |
| **Control Effectiveness** | Good - Vendor reliability; multiple access methods |
| **Treatment Strategy** | Accept |
| **Treatment Status** | Accepted |
| **Risk Owner** | IT Operations Manager |
| **Target Date** | N/A |
| **Review Date** | 2025-05-22 |
| **Comments** | Microsoft 365 availability exceeded 99.95% over past 12 months. Alternate communication via Teams (also M365) and phone available during outages. Cost of redundant email system not justified. Risk accepted by Director of IT Operations. |

---

### RISK-2024-0060 | Software License Non-Compliance

| Field | Value |
|-------|-------|
| **Asset Name** | Enterprise Software Portfolio |
| **Asset Owner** | Director of IT Operations |
| **Asset Category** | Business Asset |
| **Risk Description** | Software usage exceeds licensed quantities, resulting in audit findings and financial penalties. Decentralized software procurement and lack of usage tracking creates risk of unintentional over-deployment. Vendor audits can result in significant true-up costs. |
| **Threat Source** | Accidental - Procurement gaps |
| **Vulnerability** | Incomplete software asset management |
| **Likelihood** | 2 (Unlikely) |
| **Impact** | 2 (Low) - Financial impact; no security implications |
| **Risk Rating** | **4 - Low** |
| **Existing Controls** | Annual license reconciliation; centralized procurement for major vendors |
| **Control Effectiveness** | Moderate - Major vendors tracked; gaps in smaller purchases |
| **Treatment Strategy** | Mitigate |
| **Treatment Status** | Monitoring |
| **Risk Owner** | IT Asset Manager |
| **Target Date** | N/A - Ongoing |
| **Review Date** | 2025-05-22 |
| **Comments** | Software asset management tool (ServiceNow SAM) deployed 2024-Q1. Discovery running across endpoints. First comprehensive license position report expected Q3. Risk level may be adjusted based on findings. |

---

## 6. Risk Distribution

### By Risk Level

| Risk Level | Count | Percentage |
|------------|-------|------------|
| Critical | 2 | 13% |
| High | 4 | 27% |
| Medium | 7 | 47% |
| Low | 2 | 13% |
| **Total** | **15** | **100%** |

### By Category

| Category | Critical | High | Medium | Low | Total |
|----------|----------|------|--------|-----|-------|
| Information Security | 2 | 2 | 3 | 0 | 7 |
| Privacy | 0 | 0 | 1 | 0 | 1 |
| Operational | 0 | 1 | 2 | 2 | 5 |
| Third-Party | 0 | 1 | 1 | 0 | 2 |

### By Treatment Status

| Status | Count | Risk IDs |
|--------|-------|----------|
| In Treatment | 6 | 0042, 0045, 0038, 0049, 0052, 0055 |
| Monitoring | 5 | 0031, 0033, 0039, 0056, 0060 |
| Accepted | 2 | 0029, 0058 |
| Pending Acceptance | 1 | 0051 |
| Open (Awaiting Budget) | 1 | 0047 |

---

## 7. Governance

### 7.1 Review Cadence

| Activity | Frequency | Responsible |
|----------|-----------|-------------|
| Critical risk status check | Weekly | GRC Team |
| High risk status check | Bi-weekly | GRC Team |
| Treatment progress review | Monthly | Risk Owners |
| Full register review | Quarterly | Risk Management Committee |
| Risk reassessment | Per review date or trigger | GRC Team with Risk Owner |

### 7.2 Escalation Thresholds

- New Critical risk: Immediate CISO notification
- Risk increases to Critical: Notification within 24 hours
- Treatment deadline missed 30+ days: Escalation to Risk Management Committee
- Accepted risk conditions change: Reassessment triggered

### 7.3 Integration

This register connects to:

- **Incident Management:** Incidents update likelihood; post-incident reviews create new entries
- **Change Management:** Changes trigger reassessment for affected assets
- **Vendor Management:** Vendor assessments feed third-party risk entries
- **Audit:** Register provides evidence; findings may create entries
- **Business Continuity:** BIA informs impact ratings; register informs recovery priorities

---

## 8. Framework Alignment

This register supports:

- **NIST CSF:** ID.RA (Risk Assessment), ID.RM (Risk Management Strategy)
- **ISO 27001:** Clauses 6.1.2, 6.1.3, 8.2, 8.3
- **SOC 2:** CC3.1 through CC3.4
- **GDPR:** Articles 32 and 35

Assessment criteria and methodology details are in the **Risk Assessment Methodology** document.

---

## 9. Document Control

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 1.0 | 2024-05-22 | GRC Team | Initial release with 15 risk entries |

---

*Document Owner: Chief Information Security Officer*
*Last Updated: 2024-05-22*
*Next Review: 2024-08-22*

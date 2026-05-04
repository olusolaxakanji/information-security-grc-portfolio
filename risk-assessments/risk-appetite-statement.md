# Risk Appetite Statement

**Emyzer Technology - Governance, Risk, and Compliance Program**

---

## Document Information

| Attribute | Details |
|-----------|---------|
| **Document Title** | Risk Appetite Statement |
| **Version** | 1.0 |
| **Effective Date** | 2024-06-01 |
| **Owner** | Chief Information Security Officer (CISO) |
| **Approved By** | Risk Management Committee |
| **Classification** | Internal Use |
| **Review Cycle** | Annual or upon material change |

**Related Documents:** [Asset Risk Register v1.1](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/risk-assessments/asset-risk-register.md) | [Risk Assessment Methodology](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/risk-assessments/risk-assessment-methodology.md)

---

## 1. Purpose

The Risk Appetite Statement defines the nature and amount of risk Emyzer Technology is willing to accept in pursuit of its strategic objectives. It establishes boundaries within which risk decisions are made, communicated, and governed across the organization.

The statement serves three audiences:

- **Executives and the board**, who need a clear mandate for risk-based decision making.
- **Risk and security teams**, who translate appetite into operational controls and treatment priorities.
- **Auditors and regulators**, who require evidence that risk governance is structured, intentional, and documented.

This statement operates in direct relationship with the Asset Risk Register. Risk entries rated Critical or High that exceed the tolerances defined here require active treatment or formal executive acceptance before the next review cycle. Risk entries at Medium or Low are managed within normal operational governance.

---

## 2. Organizational Context

Emyzer Technology is a mid-market SaaS and e-commerce company that processes customer personally identifiable information (PII) and payment card data across cloud and on-premises environments. This profile creates specific risk obligations and shapes the appetite thresholds defined in this statement.

### 2.1 Regulatory and Standards Obligations

Emyzer Technology operates under the following regulatory and standards frameworks, each of which constrains the lower bound of acceptable risk posture:

| Framework | Applicable Scope | Risk Implication |
|-----------|-----------------|-----------------|
| **GDPR** | Customer PII processing and storage | Breach notification required; regulatory fines up to 4% of global revenue |
| **PCI DSS** | Payment card data via PaymentCo integration | Cardholder data exposure triggers compliance events even if breach is at a third party |
| **NIST CSF** | ID.RA and ID.RM functions | Governs risk identification, scoring, and management strategy |
| **ISO 27001** | Clauses 6.1.2, 6.1.3, 8.2, 8.3 | Risk treatment and residual risk acceptance must be documented |
| **SOC 2** | CC3.1 through CC3.4 | Risk assessment process must be demonstrable to auditors |

### 2.2 Strategic Context

Emyzer Technology's risk appetite is shaped by three strategic realities. First, customer trust is a competitive differentiator: data breaches or service failures directly erode the customer relationships that sustain revenue. Second, the company operates a payment-integrated e-commerce channel where availability and integrity failures have immediate, quantifiable revenue impact. Third, as a growing mid-market company, Emyzer must balance robust risk management against the resource constraints inherent to its stage of maturity.

---

## 3. Risk Appetite Statement

Emyzer Technology maintains a **low tolerance** for risks that threaten customer data, payment integrity, or regulatory standing. The company accepts **moderate operational risk** where robust controls and recovery capabilities are in place. It accepts the residual risk inherent in third-party dependencies when vendor assurance programs, contractual protections, and cyber insurance are in effect.

The following domain-specific appetite statements translate this overarching position into actionable guidance.

| Risk Domain | Appetite | Tolerance Threshold | Basis in Risk Register |
|-------------|----------|--------------------|-----------------------|
| **Customer Data & Privacy** | Zero tolerance for preventable exposure of customer PII or payment data | No Critical or High privacy risk left untreated beyond 90 days without executive acceptance | RISK-2024-0042 (CRM authentication); RISK-2024-0052 (dev environment data) |
| **Authentication & Access Control** | Low. MFA is required on all systems holding sensitive data. Credential-based attacks are a known, addressable threat. | Single-factor authentication on customer data systems is unacceptable. Must be remediated within the active budget cycle. | RISK-2024-0042: MFA rollout in progress. Target: 2024-08-15 |
| **Cloud Configuration & Infrastructure** | Low. Misconfigurations represent preventable, high-likelihood attack vectors. | Publicly accessible cloud storage containing internal documentation is unacceptable. Automated detection required. | RISK-2024-0045: Bucket policy corrected; AWS Config rules being implemented |
| **Endpoint Security** | Moderate. Signature-based AV is insufficient for advanced threats. EDR capability is the target state. | Endpoint detection gap rated Critical (score 16). Acceptable only with compensating SIEM monitoring. Budget decision required by Q3 2024. | RISK-2024-0047: Open, awaiting budget. Escalation requested to the Risk Management Committee. |
| **Ransomware & Business Disruption** | Low for critical financial systems. Recovery capability (RTO/RPO) must be validated, not assumed. | Untested backups on critical systems are unacceptable. Annual DR exercise mandatory. RTO for ERP must be verified within 72 hours. | RISK-2024-0038 (ERP ransomware); RISK-2024-0039 (backup restoration) |
| **Third-Party & Vendor Risk** | Moderate. Vendor risk is inherent in the business model. Acceptable when assurance is current, and insurance is in force. | Critical vendors must have a current SOC 2 Type II and SecurityScorecard rating above 80. Breach notification terms contractually required. | RISK-2024-0031 (PaymentCo); RISK-2024-0054 (Workday HR system) |
| **Service Availability** | Moderate. Availability risk during peak revenue periods requires active management and tested scalability. | E-commerce availability during peak periods must be tested to 15x baseline before November. Shield Advanced evaluation required. | RISK-2024-0055: Load testing scheduled Q3, completion target 2024-10-15 |
| **Human & Social Engineering Risk** | Moderate-Low. Human susceptibility cannot be eliminated but must be actively reduced through training and procedural controls. | Finance team phishing click rate must remain below 10%. Dual-approval controls are required for wire transfers above $10,000. | RISK-2024-0033: Current click rate 6% (improved from 18%). Controls in good standing. |
| **Key Person Dependency** | Moderate. Accepted where the budget does not support redundancy, with compensating documentation and an external retainer. | Key person risk in security operations may be formally accepted. Compensating measures required: documented procedures and an IR firm retainer. | RISK-2024-0051: Pending formal acceptance by Risk Management Committee |
| **Software & Asset Lifecycle** | Low-Moderate. End-of-life software is unacceptable on internet-facing systems. Acceptable on isolated, monitored legacy systems when migration is underway. | Unsupported software must have a documented migration timeline. Decommission must precede the vendor support end date. | RISK-2024-0049: NetSuite migration in progress. Decommission planned for November 2024. |

---

## 4. Risk Tolerance Thresholds

Risk tolerance defines the acceptable deviation from the appetite statement before escalation or mandatory treatment is required. The following thresholds apply to all risks scored using the Risk Assessment Methodology.

| Risk Level | Score Range | Tolerance Position | Required Action | Max Open Duration |
|------------|-------------|-------------------|-----------------|------------------|
| **Critical** | 15–25 | Intolerable without active treatment or formal acceptance | Immediate CISO notification. An active treatment plan or executive acceptance is required within 30 days. | 90 days before mandatory escalation to board |
| **High** | 10–14 | Tolerable with active treatment plan in place | Treatment plan must be defined within 60 days. Progress is reviewed bi-weekly. | 180 days before mandatory escalation |
| **Medium** | 5–9 | Acceptable. Managed within standard operational controls. | Documented in register. Reviewed quarterly. | Annual review sufficient |
| **Low** | 1–4 | Acceptable. Monitor for change. | Documented in register. Annual review. | Annual review sufficient |

> **Note on RISK-2024-0047:** This risk scores 16 (Critical) and its treatment is blocked by a pending budget decision. This is the sole instance where a Critical risk is open without an active treatment plan. It is tracked at Critical-level governance cadence, and the risk owner has requested escalation to the Risk Management Committee. This situation falls outside the stated tolerance and requires resolution in the current review cycle.

---

## 5. Unacceptable Risk Conditions

The following conditions are considered beyond appetite regardless of their score on the risk matrix. Any condition identified below triggers mandatory treatment regardless of available budget or resource constraints.

- Customer PII or payment cardholder data exposed without detection or notification controls in place.
- Internet-facing systems operating without MFA where data classification is Confidential or above.
- Cloud storage buckets configured with public read access containing internal or customer data.
- Critical systems without a tested backup and restoration procedure in the preceding 12 months.
- End-of-life software operating on internet-facing systems without an active migration plan and a defined decommission date.
- Third-party vendors with access to customer data and no current SOC 2 Type II or equivalent assurance on file.
- A Critical risk (score ≥ 15) open for more than 90 days without formal executive acceptance on record.

---

## 6. Governance and Accountability

Risk appetite is not a policy: it is a decision framework. It only functions when the accountability structure below is active and enforced.

| Role | Responsibility | Appetite-Related Action |
|------|---------------|------------------------|
| **Board / Executive Committee** | Set and approve the overall risk appetite; receive quarterly risk posture reporting | Formally accept any Critical risk that cannot be treated within 90 days |
| **Risk Management Committee** | Operationalize appetite; review escalated risks; approve formal acceptances | Review RISK-2024-0047 budget escalation; accept RISK-2024-0051 key person risk |
| **CISO** | Own this statement; maintain the Risk Register; escalate threshold breaches | Weekly Critical risk status checks; 24-hour notification of new Critical risks |
| **Risk Owners** | Execute treatment plans; report progress; flag blockers | Monthly treatment progress updates; escalate missed target dates within 10 days |
| **GRC Team** | Maintain the register; coordinate assessments; produce reporting | Bi-weekly High risk checks; quarterly full register review |
| **Asset Owners** | Accountable for protection of assigned assets; participate in assessments | Approve treatment decisions for assets under their ownership |

### 6.1 Escalation Triggers

The following events trigger mandatory escalation outside the standard review cadence:

- A new Critical risk is identified: immediate CISO notification required.
- An existing risk increases to Critical: notification within 24 hours.
- A treatment plan deadline is missed by 30 days or more: escalation to the Risk Management Committee.
- A formally accepted risk materially changes in likelihood, impact, or control effectiveness: reassessment triggered.
- A third-party vendor's SecurityScorecard rating drops below 80: immediate vendor risk review.

### 6.2 Review and Amendment

This statement is reviewed annually, or immediately upon any of the following triggers: material change in regulatory environment; significant shift in business model or technology environment; post-incident review identifying appetite misalignment; or Risk Management Committee direction.

---

## 7. Current Risk Posture Against Appetite

The following summary maps the current register snapshot (2024-05-22) against the appetite thresholds defined in this statement.

| Risk ID | Risk Level | Status | Appetite Alignment |
|---------|------------|--------|--------------------|
| RISK-2024-0042 | Critical (20) | In Treatment | ✅ Within appetite: active treatment underway. MFA rollout target August 2024. |
| RISK-2024-0045 | Critical (20) | In Treatment | ✅ Within appetite: immediate remediation applied. AWS Config automation in progress. |
| RISK-2024-0047 | Critical (16) | Open: Budget Pending | ⚠️ **Outside appetite.** Compensating control (SIEM) in place. Budget escalation is required this cycle. |
| RISK-2024-0038 | High (15) | In Treatment | ✅ Within appetite: network segmentation 60% complete. EDR procurement in progress. |
| RISK-2024-0031 | High (12) | Monitoring | ✅ Within appetite: SecurityScorecard A (87/100). Cyber insurance is in force. |
| RISK-2024-0049 | High (12) | In Treatment | ✅ Within appetite: migration underway. Decommission is planned before the support end date. |
| RISK-2024-0033 | High (12) | Monitoring | ✅ Within appetite: phishing click rate 6%, below 10% threshold. Dual-approval active. |
| RISK-2024-0051 | Medium (9) | Pending Acceptance | ✅ Within appetite if formally accepted with compensating measures documented. |
| RISK-2024-0052, 0054, 0055, 0039, 0056 | Medium (6–9) | In Treatment / Monitoring | ✅ Within appetite. Managed through standard operational controls and quarterly review. |
| RISK-2024-0029, 0058, 0060 | Low (4–6) | Accepted / Monitoring | ✅ Within appetite. Formal acceptance in place where applicable. Annual review scheduled. |

**Summary:** 14 of 15 risks are within appetite or have an active path to alignment. RISK-2024-0047 is the sole open exception requiring resolution this cycle. RISK-2024-0051 requires formal acceptance documentation before the next review date.

---

## 8. Document Control

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 1.0 | 2024-06-01 | GRC Team | Initial release. Derived from Asset Risk Register v1.1. |

---

*Document Owner: Chief Information Security Officer*
*Last Updated: 2024-06-01*
*Next Review: 2025-06-01 or upon material change*
*Classification: Internal Use*

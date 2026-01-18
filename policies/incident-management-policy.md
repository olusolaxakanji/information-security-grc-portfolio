# Incident Management Policy

**Emyzer Technology – Governance, Risk, and Compliance**

---

## Policy Metadata

| Attribute | Value |
|-----------|-------|
| **Policy Name** | Incident Management Policy |
| **Type** | Policy |
| **Owner** | Information Security Officer (Susan Orwell) |
| **Owning Group** | App Engine Studio Users |
| **Parent** | Information Security Policy |
| **State** | Published |
| **Valid From** | 2026-01-13 |
| **Valid To** | 2027-01-13 |
| **Approvers** | Chief Information Security Officer |
| **Reviewers** | GRC Analyst |
| **Knowledge Base** | Governance, Risk, and Compliance |
| **Published Policy** | KB-PORTFOLIO-0005 |

---

## Description

This policy provides a framework for detecting, reporting, and responding to information security incidents.

**Impact:** Ensures timely and effective response to security incidents, minimizing operational disruption and protecting sensitive information.

**Relevant Standards:** ISO/IEC 27035, NIST SP 800-61, GDPR

---

## Policy Snapshot

| Dimension | Summary |
|-----------|---------|
| **Applies to** | All departments, employees, contractors, and third-party vendors handling Emyzer Technology's information assets |
| **Covers** | All information systems, applications, networks, and data repositories; all security events and incidents regardless of source |
| **Review Cadence** | Annual review or upon major incidents/regulatory changes; post-incident reviews conducted per incident |
| **Key Governance** | ISO provides oversight; IRT manages response operations; department heads enforce compliance; all employees report incidents |
| **Exceptions Process** | ServiceNow workflow with ISO/CISO approval; maximum 90-day duration; quarterly review of active exceptions |
| **Evidence Maintained** | Incident reports, IRT meeting minutes, breach notifications, containment logs, recovery reports, post-incident reviews (all with defined retention periods) |

---

## A. Purpose

To establish a structured and consistent approach to managing information security incidents within Emyzer Technology. This policy aims to minimize the impact of incidents on operations, protect sensitive information, and ensure compliance with ISO/IEC 27035, NIST SP 800-61, and GDPR frameworks.

---

## B. Scope

This policy applies to all departments and activities within Emyzer Technology, including but not limited to Information Technology, Human Resources, Legal, Finance, Operations, and all third-party vendors and contractors handling Emyzer Technology's information assets. It encompasses all information systems, applications, networks, and data repositories where Emyzer Technology conducts its business.

**Third-party applicability:** Third parties handling organizational data or systems shall meet equivalent incident management controls via contractual requirements and periodic security reviews.

---

## C. Definitions

1. **Incident:** An unexpected event that compromises confidentiality, integrity, or availability of information.

2. **Incident Response Team (IRT):** A designated group responsible for managing and responding to security incidents.

3. **Personal Data:** Any information about an identifiable natural person as defined by GDPR.

4. **GDPR (General Data Protection Regulation):** A regulatory framework that sets guidelines for the collection and processing of personal data of individuals within the European Union.

5. **Security Event:** Any observable occurrence in a system or network that may indicate a security incident.

6. **Data Breach:** An incident involving unauthorized access, disclosure, or loss of personal or sensitive data.

7. **Containment:** Actions taken to limit the scope and impact of a security incident.

8. **Eradication:** The process of removing the root cause of a security incident.

9. **Post-Incident Review:** A structured analysis conducted after incident resolution to identify lessons learned.

---

## D. Policy Statement

Emyzer Technology is committed to promptly identifying, reporting, and responding to information security incidents. To achieve this, the organization shall:

1. Establish and maintain an Incident Response Team (IRT) with clearly defined roles and responsibilities.

2. Implement incident detection capabilities to identify security events in real time through SIEM and monitoring tools.

3. Follow structured incident response procedures aligned with ISO/IEC 27035 and NIST SP 800-61 with defined response timeframes (critical: 1 hour; high: 4 hours; medium: 24 hours; low: 72 hours).

4. Comply with GDPR breach notification requirements for incidents involving personal data, notifying supervisory authorities within **72 hours** of discovery.

5. Conduct post-incident reviews within **5 business days** of incident resolution to drive continuous improvement in security posture.

6. Review and audit the incident management program **annually** with continuous improvement through lessons learned integration.

---

## E. Roles and Responsibilities

### E.1 Chief Information Security Officer (CISO)
Shall provide executive oversight of the incident management program. Shall approve strategic incident response decisions and significant resource allocations. Shall serve as the escalation point for critical incidents and reportable breaches. Shall authorize external communications regarding security incidents.

### E.2 Information Security Officer (ISO)
Shall oversee the incident management process under the CISO's direction. Shall ensure compliance with relevant standards and regulations through documented evidence and periodic assessments. Shall report significant incidents to executive management within **4 hours** of classification. Acts as the delegated incident executive for day-to-day program operations.

### E.3 Incident Response Team (IRT)
Shall manage detection, analysis, containment, eradication, and recovery of incidents with documented procedures. Shall coordinate response activities across departments with **15-minute status updates** during active critical incidents. Shall maintain incident documentation and the chain of custody for evidence. Shall conduct post-incident reviews and implement lessons learned.

### E.4 Department Heads
Shall ensure teams comply with the incident management policy through **quarterly attestation**. Shall support incident response activities within their areas of responsibility. Shall participate in post-incident reviews and implement departmental corrective actions. Shall report suspected incidents within **1 hour** of discovery.

### E.5 All Employees
Shall report any suspected or actual information security incidents immediately to the ISO or IRT within **1 hour** of discovery. Shall preserve evidence and avoid actions that could worsen the incident. Shall cooperate fully with incident response activities. Shall complete **annual** incident response and onboarding training within 7 days of the start date.

---

## F. Minimum Security Requirements

The following requirements establish baseline incident management controls. Detailed implementation procedures are maintained in the **IT Incident Response Plan** and related operational documentation.

### F.1 Incident Detection
- Shall implement continuous security monitoring through SIEM, IDS/IPS, and endpoint detection tools.
- Shall configure automated alerting for security events exceeding defined thresholds.
- Shall maintain 24/7 monitoring coverage for critical systems and applications.
- Shall correlate security events across multiple data sources to identify potential incidents.

### F.2 Incident Reporting
- Shall report suspected incidents to the IRT within **1 hour** of discovery through established reporting channels (ServiceNow, security hotline, or direct contact).
- Shall log all incidents in the incident management system with initial classification and severity assessment within **30 minutes** of report receipt.
- Shall assign incident ticket numbers for tracking and documentation purposes.
- Shall acknowledge incident reports to the reporter within **15 minutes** during business hours.

### F.3 Incident Analysis
- Shall conduct preliminary analysis to determine scope, impact, and classification within **2 hours** of incident logging.
- Shall assess whether personal data is involved and initiate GDPR breach notification procedures if applicable.
- Shall document initial findings, affected systems, and potential attack vectors.
- Shall escalate incidents to the appropriate severity level based on analysis findings.

### F.4 Incident Classification
- Shall classify incidents by severity (Critical, High, Medium, Low) based on impact to confidentiality, integrity, and availability of information assets.
- Shall apply classification criteria: Critical (business-critical systems compromised, data breach confirmed); High (significant system impact, potential data exposure); Medium (limited impact, single system affected); Low (minimal impact, no data exposure).
- Shall reassess classification as new information becomes available during response.
- Shall document classification rationale and approvals in the incident record.

### F.5 Containment
- Shall implement immediate containment measures within defined timeframes: Critical (**1 hour**), High (**4 hours**), Medium (**24 hours**), Low (**72 hours**).
- Shall select containment strategies based on incident type: network isolation, account suspension, system shutdown, or traffic blocking.
- Shall document all containment actions with timestamps and responsible parties.
- Shall preserve evidence during containment for potential forensic analysis and legal proceedings.

### F.6 Eradication
- Shall identify and remove the root cause of the incident within **48 hours** of containment for critical/high incidents.
- Shall implement remediation actions, including patching vulnerabilities, removing malware, closing unauthorized access points, or rebuilding compromised systems.
- Shall verify eradication effectiveness through scanning and monitoring before proceeding to recovery.
- Shall document root cause analysis with contributing factors and remediation actions taken.

### F.7 Recovery
- Shall restore affected systems and services to normal operation following verified eradication.
- Shall verify system integrity through baseline comparison, integrity checking, and security scanning before returning to production.
- Shall implement enhanced monitoring for **30 days** following recovery to detect recurrence.
- Shall obtain business owner approval before returning systems to production.

### F.8 Post-Incident Review
- Shall conduct structured post-incident review within **5 business days** of incident resolution for all high and critical incidents.
- Shall document lessons learned, root cause analysis, and improvement recommendations.
- Shall assign corrective actions with owners and target completion dates.
- Shall share findings with relevant stakeholders and update procedures as necessary.

---

## G. Compliance and Monitoring

Compliance with this policy shall be monitored through **quarterly incident management reviews and control assessments** combined with **annual internal audits**. Non-compliance shall be addressed through documented corrective actions within 30 days. Violations may result in access revocation, mandatory corrective training, and disciplinary actions up to and including termination.

### Performance Metrics
Key performance indicators (KPIs) track incident response effectiveness, including:
- Mean Time to Detect (MTTD) incidents (target: <1 hour for critical systems)
- Mean Time to Contain (MTTC) incidents against SLA targets
- Mean Time to Recover (MTTR) from incidents
- Number of incidents by category and severity
- Percentage of incidents with completed post-incident reviews (target: 100% for high/critical)
- GDPR breach notifications submitted within 72-hour requirement (target: 100%)

---

## H. Policy Exceptions

### H.1 Exception Request Process
Employees requiring a temporary deviation from this policy shall:
1. Submit exception requests via the **ServiceNow GRC/ITSM ticketing workflow (or equivalent ticketing system)** with detailed business justification, risk assessment, and proposed compensating controls.
2. Obtain approval from the Information Security Officer for tactical exceptions (≤30 days) or the CISO for strategic exceptions (>30 days).
3. Accept exceptions valid for a maximum of **90 days** unless formally renewed.
4. Document compensating controls implemented during the exception period.

### H.2 Exception Governance
- All active exceptions shall be reviewed **quarterly** by the Information Security Officer to confirm continued necessity.
- Exception renewals shall require updated business justification and CISO approval.
- Each exception shall include a remediation plan with a target closure date not to exceed 180 days from initial approval.
- Exception tracking shall be maintained in the GRC platform with status updates provided to executive leadership **monthly**.

---

## I. Related Policies

This policy is supported by the following subordinate policies and procedures:

1. [**Information Security Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/information-security-policy.md) – Parent policy defining the ISMS framework, security controls, and overall governance structure for information protection.

2. [**Access Control Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/access-control-policy.md) – Defines authentication mechanisms, authorization models, and access revocation procedures used during incident containment.

3. [**Risk Management Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/risk-management-policy.md) – Defines risk assessment methodology and incident correlation analysis that informs incident prioritization and response.

4. **Data Protection and Privacy Policy** – Defines data classification, handling requirements, and GDPR compliance procedures for incidents involving personal data.

5. **Business Continuity and Disaster Recovery Policy** – Defines recovery procedures and business continuity activation criteria for incidents causing significant operational disruption.

---

## J. Related Documents

1. IT Incident Response Plan
2. GDPR Breach Notification Procedures
3. Forensic Investigation Procedures
4. Communication Plan (Internal/External)
5. Business Continuity Plan
6. Disaster Recovery Plan

---

## K. Review and Revision

This policy shall be reviewed **annually** or when significant changes occur (regulatory updates, major security incidents, organizational restructuring, technology changes, lessons learned from incident response activities) to ensure its continued relevance and effectiveness. Revisions shall be made to address emerging threats, regulatory changes, and improvements in best practices. All revisions require CISO approval and notification to executive leadership.

---

## L. Framework Alignment

| Framework | Alignment |
|-----------|-----------|
| **ISO/IEC 27035-1:2023** | Planning and preparation, Detection and reporting, Assessment and decision, Response activities, Lessons learned |
| **NIST SP 800-61 Rev. 2** | Preparation, Detection and Analysis, Containment/Eradication/Recovery, Post-Incident Activity |
| **GDPR (EU 2016/679)** | Article 33 (Breach notification to supervisory authority within 72 hours), Article 34 (Communication of breach to data subjects), Article 32 (Security of processing) |
| **NIST Cybersecurity Framework** | DE.CM (Security Continuous Monitoring), DE.AE (Anomalies and Events), RS.RP (Response Planning), RS.CO (Communications), RS.AN (Analysis), RS.MI (Mitigation), RC.RP (Recovery Planning) |
| **ISO/IEC 27001:2022** | Clause 10.2 (Nonconformity and corrective action), A.5.24 (Information security incident management planning and preparation), A.5.25 (Assessment and decision on information security events), A.5.26 (Response to information security incidents), A.5.27 (Learning from information security incidents) |

**Note:** This policy aligns with these standards; certification and compliance scope are defined in the ISMS Statement of Applicability (SoA).

---

## M. Organizational Benefit

| Benefit Area | Description |
|--------------|-------------|
| **Reduced Impact** | Structured incident response minimizes operational disruption, financial losses, and reputational damage from security events |
| **Regulatory Compliance** | Demonstrates adherence to GDPR breach notification requirements and industry-specific incident reporting obligations |
| **Reputation Protection** | Swift, professional incident handling protects organizational credibility and customer trust |
| **Continuous Improvement** | Post-incident reviews drive security posture enhancements and prevent recurring incidents |
| **Legal Protection** | Documented incident response processes provide evidence of due diligence in legal proceedings and regulatory investigations |
| **Stakeholder Confidence** | Clear incident management capabilities reassure customers, partners, and investors about organizational resilience |
| **Faster Recovery** | Established procedures enable quicker return to normal operations, minimizing business impact |
| **Threat Intelligence** | Incident analysis contributes to organizational threat intelligence and proactive defense capabilities |

---

## N. Evidence of Compliance

The organization shall maintain the following compliance evidence with defined retention periods:

### Evidence Index

| Evidence Type | System of Record | Owner | Retention Period |
|---------------|------------------|-------|------------------|
| Incident Reports | ServiceNow ITSM | Information Security Team | 7 years |
| IRT Meeting Minutes | Document Repository | Incident Response Team | 7 years |
| GDPR Breach Notifications | GRC Platform / Legal Repository | Data Protection Officer | 10 years |
| Containment Action Logs | ServiceNow ITSM / SIEM | Incident Response Team | 7 years |
| Eradication Documentation | Document Repository | Information Security Team | 7 years |
| Recovery Verification Reports | Document Repository | IT Operations | 5 years |
| Post-Incident Review Reports | GRC Platform | Information Security Officer | 7 years |
| Employee Training Records | Learning Management System (LMS) | Human Resources | 3 years |
| Incident Response Plan Tests | Document Repository | Information Security Officer | 5 years |
| Incident Metrics Dashboard | GRC Platform / SIEM | Information Security Officer | 3 years |
| Forensic Investigation Reports | Secure Document Repository | Information Security Team | 10 years |
| External Audit Reports | GRC Platform / Document Repository | Internal Audit | 7 years |

---

### N.1 Incident Detection and Reporting Evidence
- **Incident Reports:** Documented records of all security incidents maintained in ServiceNow ITSM, showing incident ID, detection timestamp, reporter, initial classification, severity, affected systems, and status. Created **per incident**. Retained for 7 years.
- **Security Event Logs:** SIEM logs showing detection of suspicious activities, automated alerts, and event correlation. Retained for 1 year (3 years for incidents).
- **Incident Intake Records:** Documentation of initial incident reports, including reporter contact, discovery method, and preliminary impact assessment. Retained for 7 years.

### N.2 Incident Analysis and Classification Evidence
- **Incident Analysis Reports:** Documentation of preliminary and detailed analysis showing scope determination, impact assessment, attack vector identification, and classification rationale. Completed within **2 hours** of incident logging. Retained for 7 years.
- **Classification Approval Records:** Documentation of severity classification decisions with approver name, timestamp, and supporting rationale. Retained for 7 years.
- **Threat Intelligence Correlation:** Analysis connecting incidents to known threat actors, campaigns, or attack patterns. Retained for 5 years.

### N.3 Containment and Eradication Evidence
- **Containment Action Logs:** Technical documentation of measures taken to contain, isolate, and mitigate incidents, including timestamps, actions taken, responsible parties, and effectiveness verification. Created **per incident**. Retained for 7 years.
- **Eradication Documentation:** Records of root cause analysis, remediation actions, vulnerability patches applied, and malware removal verification. Retained for 7 years.
- **Evidence Preservation Records:** Chain of custody documentation for forensic evidence, including collection method, storage location, and access log. Retained for 10 years.

### N.4 Recovery Evidence
- **Recovery Verification Reports:** Documentation of system restoration, integrity verification, baseline comparison results, and return-to-production approval. Created **per incident**. Retained for 5 years.
- **Enhanced Monitoring Logs:** Documentation of post-recovery monitoring activities and any detected anomalies during the 30-day monitoring period. Retained for 3 years.
- **Business Owner Approvals:** Signed authorization for returning systems to production following incident recovery. Retained for 5 years.

### N.5 GDPR Breach Notification Evidence
- **Breach Assessment Records:** Documentation of personal data impact assessment determining notification requirements. Created **per applicable incident**. Retained for 10 years.
- **Supervisory Authority Notifications:** Records of data breach notifications to supervisory authorities submitted within **72 hours** of discovery, including notification content and delivery confirmation. Retained for 10 years.
- **Data Subject Notifications:** Records of communications to affected data subjects when required, including notification content, recipient lists, and delivery confirmation. Retained for 10 years.
- **Notification Timeline Documentation:** Evidence demonstrating compliance with 72-hour notification requirement, including discovery timestamp and notification submission timestamp. Retained for 10 years.

### N.6 Post-Incident Review Evidence
- **Post-Incident Review Reports:** Structured analysis of incidents including timeline reconstruction, root cause analysis, lessons learned, and improvement recommendations. Completed within **5 business days** of incident resolution for high/critical incidents. Retained for 7 years.
- **Corrective Action Tracking:** Documentation of assigned corrective actions with owners, target completion dates, implementation evidence, and effectiveness verification. Retained for 5 years.
- **Procedure Updates:** Version-controlled documentation of incident response procedure updates resulting from lessons learned. Retained indefinitely (current version with history).

### N.7 Training and Preparedness Evidence
- **Employee Training Records:** Learning management system (LMS) reports showing employee name, course title, completion date, and pass/fail status for incident response awareness training. Retained for 3 years.
- **IRT Training Records:** Documentation of specialized training for Incident Response Team members, including technical skills, forensics, and communication protocols. Retained for 3 years.
- **Tabletop Exercise Records:** Sign-in sheets, scenario descriptions, participant responses, identified gaps, and improvement recommendations from **semi-annual** incident response exercises. Retained for 5 years.
- **Incident Response Plan Tests:** Results of simulation drills and tests of IRT readiness, including response times, communication effectiveness, and procedure adherence. Conducted **semi-annually**. Retained for 5 years.

### N.8 Audit and Metrics Evidence
- **Internal Audit Reports:** Annual internal incident management program audits showing findings, severity classifications, remediation plans, and closure evidence. Retained for 7 years.
- **External Audit Reports:** Third-party assessments of incident management program maturity and compliance. Retained for 7 years.
- **Incident Metrics Dashboard:** Real-time tracking of MTTD, MTTC, MTTR, incident volume by category/severity, and trend analysis. Exported **monthly**. Retained for 3 years.
- **KPI Reports:** Quarterly analysis of incident response performance against defined targets with variance explanations and improvement initiatives. Retained for 5 years.

---

## Approval History

| Date | Approver | Status | Comments |
|------|----------|--------|----------|
| 2026-01-13 | Chief Information Security Officer | Approved | "Comprehensive incident framework. Approved." |

---

## Document Control

- **Document ID:** KB-PORTFOLIO-0005
- **Version:** 2.0
- **Classification:** Internal
- **Last Updated:** 2026-01-13
- **Next Review Date:** 2027-01-13

---

*This policy document was generated from ServiceNow GRC and formatted for portfolio presentation.*

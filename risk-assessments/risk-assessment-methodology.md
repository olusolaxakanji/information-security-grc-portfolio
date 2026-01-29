# Risk Assessment Methodology

**Emyzer Technology - Governance, Risk, and Compliance Program**

---

## Document Information

| Attribute | Details |
|-----------|---------|
| **Document Title** | Risk Assessment Methodology |
| **Document Type** | Methodology |
| **Version** | 1.0 |
| **Effective Date** | 2024-05-22 |
| **Review Date** | 2025-05-22 |
| **Owner** | Chief Information Security Officer (CISO) |
| **Approver** | Risk Management Committee |
| **Classification** | Internal Use |

---

## A. Purpose

This document establishes a standardized methodology for identifying, analyzing, evaluating, and treating risks across Emyzer Technology. The methodology provides a consistent, repeatable framework for informed decision-making on risk treatment priorities and resource allocation.

The Risk Assessment Methodology serves as the operational foundation for Emyzer Technology's enterprise risk management program. It translates strategic risk appetite into practical assessment activities that protect organizational assets, ensure regulatory compliance, and support business objectives.

---

## B. Scope

This methodology applies to all risk assessment activities conducted within Emyzer Technology, including:

**Risk Categories Covered:**

- **Operational Risks:** Process failures, system outages, human error, and business disruption events
- **Information Security Risks:** Threats to confidentiality, integrity, and availability of information assets
- **Compliance Risks:** Regulatory violations, contractual breaches, and policy non-compliance
- **Privacy Risks:** Unauthorized processing, disclosure, or loss of personal data
- **Third-Party Risks:** Vendor and supplier-related exposures affecting Emyzer Technology operations
- **Strategic Risks:** Threats to organizational objectives, reputation, and competitive position

**Assessment Coverage:**

- Enterprise-wide risk assessments conducted annually
- Project-specific risk assessments for new initiatives
- System and application risk assessments prior to deployment
- Vendor risk assessments during procurement and periodic review
- Incident-driven risk assessments following security events
- Change-triggered risk assessments for significant operational changes

---

## C. Definitions

| Term | Definition |
|------|------------|
| **Risk** | The effect of uncertainty on objectives, expressed as a combination of likelihood and impact of a potential event |
| **Risk Assessment** | The overall process of risk identification, risk analysis, and risk evaluation |
| **Likelihood** | The probability that a given threat will exploit a vulnerability, measured on a defined scale |
| **Impact** | The magnitude of harm that could result from a risk event, measured across multiple dimensions |
| **Risk Owner** | The individual accountable for managing a specific risk and ensuring appropriate treatment |
| **Risk Tolerance** | The acceptable level of variation relative to achievement of objectives |
| **Risk Appetite** | The amount and type of risk an organization is willing to pursue or retain |
| **Risk Register** | A structured repository documenting identified risks, their attributes, and treatment status |
| **Inherent Risk** | The level of risk before any controls or mitigating factors are applied |
| **Residual Risk** | The level of risk remaining after controls have been implemented |
| **Control** | A measure that modifies risk, including policies, procedures, and technical safeguards |
| **Threat** | A potential cause of an unwanted incident that may result in harm |
| **Vulnerability** | A weakness that can be exploited by a threat to cause harm |
| **Asset** | Anything of value to the organization requiring protection |

---

## D. Risk Assessment Approach

Emyzer Technology employs a hybrid risk assessment approach that combines qualitative and quantitative methods to produce actionable risk intelligence.

### D.1 Qualitative Assessment

Qualitative assessment uses descriptive scales to evaluate likelihood and impact. This approach is appropriate when:

- Precise data is unavailable or impractical to obtain
- Rapid assessment is required for decision-making
- Comparing risks across different domains or categories
- Initial screening of risks for prioritization

Qualitative assessments produce risk ratings expressed as categories (Critical, High, Medium, Low) rather than numerical values. This method supports consistent communication and comparison of risks across the organization.

### D.2 Quantitative Assessment

Quantitative assessment assigns numerical values to likelihood and impact, often expressed in financial terms. This approach is appropriate when:

- Sufficient historical data exists to support statistical analysis
- Financial justification is required for risk treatment investments
- Comparing risks with significantly different characteristics
- Supporting insurance and risk transfer decisions

Quantitative assessments produce metrics such as Annual Loss Expectancy (ALE), Single Loss Expectancy (SLE), and Annualized Rate of Occurrence (ARO).

### D.3 Framework Alignment

This methodology aligns with recognized standards and frameworks:

| Framework | Application |
|-----------|-------------|
| **ISO 31000** | Enterprise risk management principles and process |
| **NIST SP 800-30** | Information security risk assessment guidance |
| **NIST Cybersecurity Framework** | Identify function and risk assessment activities |
| **ISO 27005** | Information security risk management |
| **COBIT 2019** | IT governance and risk management objectives |
| **FAIR** | Factor Analysis of Information Risk for quantitative assessment |

---

## E. Methodology Steps

The risk assessment process follows six sequential steps that form a continuous cycle.

### Step 1: Risk Identification

**Objective:** Systematically discover and document potential risks that could affect organizational objectives.

**Activities:**

1. **Asset Inventory Review:** Identify information assets, systems, processes, and third parties within the assessment scope
2. **Threat Identification:** Catalog potential threat sources, including adversarial, accidental, structural, and environmental threats
3. **Vulnerability Assessment:** Document weaknesses in systems, processes, and controls that could be exploited
4. **Stakeholder Consultation:** Conduct interviews with process owners, technical staff, and business leaders
5. **Historical Analysis:** Review incident records, audit findings, and industry threat intelligence
6. **Scenario Development:** Create risk scenarios describing how threats could exploit vulnerabilities

**Inputs:**
- Asset inventory and data classification records
- Network diagrams and system architecture documentation
- Previous risk assessment results
- Audit and compliance findings
- Incident and near-miss reports
- External threat intelligence reports

**Outputs:**
- Preliminary risk inventory with identified scenarios
- Updated asset and threat catalogs

### Step 2: Risk Analysis

**Objective:** Determine the likelihood and potential impact of each identified risk.

**Activities:**

1. **Likelihood Estimation:** Assess the probability of each risk scenario occurring using the likelihood scale
2. **Impact Assessment:** Evaluate potential consequences across impact dimensions (financial, operational, reputational, compliance, safety)
3. **Control Evaluation:** Document existing controls and assess their effectiveness
4. **Inherent Risk Calculation:** Determine risk level assuming no controls exist
5. **Residual Risk Calculation:** Determine risk level considering existing control effectiveness

**Inputs:**
- Preliminary risk inventory
- Control documentation
- Historical incident data
- Threat intelligence
- Expert judgment from subject matter experts

**Outputs:**
- Likelihood and impact ratings for each risk
- Inherent and residual risk scores
- Control effectiveness assessments

### Step 3: Risk Evaluation and Prioritization

**Objective:** Compare analyzed risks against risk criteria and prioritize for treatment.

**Activities:**

1. **Risk Scoring:** Calculate risk scores using the risk matrix
2. **Threshold Comparison:** Compare risk scores against defined tolerance thresholds
3. **Risk Ranking:** Order risks by score to establish treatment priorities
4. **Aggregation Analysis:** Identify risk concentrations and interdependencies
5. **Treatment Recommendation:** Recommend treatment approach based on risk level

**Inputs:**
- Analyzed risks with likelihood and impact ratings
- Risk tolerance thresholds
- Organizational risk appetite statement

**Outputs:**
- Prioritized risk register
- Treatment recommendations by risk level
- Risk heat map visualization

### Step 4: Risk Documentation

**Objective:** Record all risk information in the enterprise risk register.

**Activities:**

1. **Register Update:** Enter or update risk records in the risk register
2. **Ownership Assignment:** Assign risk owners accountable for each risk
3. **Attribute Documentation:** Record all risk attributes, including category, source, and affected assets
4. **Control Linkage:** Link risks to existing and planned controls
5. **Status Tracking:** Document assessment status and review dates

**Required Risk Register Fields:**

| Field | Description |
|-------|-------------|
| Risk ID | Unique identifier for the risk |
| Risk Title | Brief descriptive name |
| Risk Description | Detailed explanation of the risk scenario |
| Risk Category | Classification (operational, security, compliance, etc.) |
| Risk Owner | Accountable individual |
| Likelihood Rating | Assessed probability score |
| Impact Rating | Assessed consequence score |
| Inherent Risk Score | Risk level without controls |
| Existing Controls | Current mitigation measures |
| Control Effectiveness | Rating of control performance |
| Residual Risk Score | Risk level with current controls |
| Target Risk Level | Desired future risk level |
| Treatment Strategy | Accept, mitigate, transfer, or avoid |
| Treatment Actions | Planned risk reduction activities |
| Status | Open, in treatment, monitoring, closed |
| Last Assessment Date | Date of most recent evaluation |
| Next Review Date | Scheduled reassessment date |

**Outputs:**
- Completed risk register entries
- Risk documentation package

### Step 5: Risk Treatment and Mitigation

**Objective:** Select and implement appropriate responses to reduce risk to acceptable levels.

**Treatment Options:**

| Strategy | Description | When to Apply |
|----------|-------------|---------------|
| **Accept** | Acknowledge the risk and take no additional action | Risk is within tolerance; treatment cost exceeds benefit |
| **Mitigate** | Implement controls to reduce likelihood or impact | Risk exceeds tolerance; effective controls are available |
| **Transfer** | Shift risk to third party through insurance or contract | Risk is insurable; contractual transfer is feasible |
| **Avoid** | Eliminate the risk by ceasing the associated activity | Risk is unacceptable; no viable mitigation exists |

**Treatment Planning Activities:**

1. **Option Analysis:** Evaluate treatment alternatives for cost-effectiveness
2. **Control Selection:** Choose controls that address root causes
3. **Implementation Planning:** Develop timelines, resources, and responsibilities
4. **Residual Risk Projection:** Estimate post-treatment risk levels
5. **Approval:** Obtain risk owner and management approval for treatment plans

**Outputs:**
- Risk treatment plans
- Updated risk register with treatment details
- Resource requirements and timelines

### Step 6: Monitoring and Review

**Objective:** Track risk status and ensure treatment effectiveness over time.

**Activities:**

1. **Key Risk Indicator (KRI) Monitoring:** Track metrics that signal changes in risk levels
2. **Control Testing:** Periodically verify control effectiveness
3. **Treatment Progress Tracking:** Monitor implementation of risk treatment plans
4. **Trigger Event Monitoring:** Watch for events requiring reassessment
5. **Periodic Reassessment:** Conduct scheduled risk reviews

**Monitoring Frequencies:**

| Risk Level | Monitoring Frequency | Full Reassessment |
|------------|---------------------|-------------------|
| Critical | Weekly | Monthly |
| High | Bi-weekly | Quarterly |
| Medium | Monthly | Semi-annually |
| Low | Quarterly | Annually |

**Outputs:**
- KRI dashboards and trend reports
- Treatment progress reports
- Reassessment schedules
- Escalation notifications for threshold breaches

---

## F. Risk Scoring and Matrix

### F.1 Likelihood Scale

| Rating | Score | Description | Probability |
|--------|-------|-------------|-------------|
| **Almost Certain** | 5 | Expected to occur in most circumstances | Greater than 90% |
| **Likely** | 4 | Will probably occur in most circumstances | 60% to 90% |
| **Possible** | 3 | Might occur at some time | 30% to 60% |
| **Unlikely** | 2 | Could occur at some time | 10% to 30% |
| **Rare** | 1 | May occur only in exceptional circumstances | Less than 10% |

### F.2 Impact Scale

| Rating | Score | Financial Impact | Operational Impact | Reputational Impact | Compliance Impact |
|--------|-------|------------------|-------------------|--------------------|--------------------|
| **Catastrophic** | 5 | Greater than $10M | Extended enterprise-wide disruption | Sustained negative media coverage; executive changes | Major regulatory action; license revocation |
| **Major** | 4 | $1M to $10M | Significant multi-department impact | Regional negative media; customer attrition | Regulatory investigation; significant fines |
| **Moderate** | 3 | $100K to $1M | Notable impact on one department | Local media coverage; some customer complaints | Formal regulatory inquiry; minor fines |
| **Minor** | 2 | $10K to $100K | Limited impact; workarounds available | Internal stakeholder concerns | Internal audit findings; self-reported issues |
| **Insignificant** | 1 | Less than $10K | Minimal impact; easily absorbed | No external visibility | No regulatory implications |

### F.3 Risk Matrix

The risk score is calculated by multiplying the likelihood rating by the impact rating.

**Risk Score = Likelihood × Impact**

|  | **Insignificant (1)** | **Minor (2)** | **Moderate (3)** | **Major (4)** | **Catastrophic (5)** |
|---|:---:|:---:|:---:|:---:|:---:|
| **Almost Certain (5)** | 5 Medium | 10 High | 15 High | 20 Critical | 25 Critical |
| **Likely (4)** | 4 Low | 8 Medium | 12 High | 16 Critical | 20 Critical |
| **Possible (3)** | 3 Low | 6 Medium | 9 Medium | 12 High | 15 High |
| **Unlikely (2)** | 2 Low | 4 Low | 6 Medium | 8 Medium | 10 High |
| **Rare (1)** | 1 Low | 2 Low | 3 Low | 4 Low | 5 Medium |

### F.4 Risk Level Classifications

| Risk Level | Score Range | Treatment Requirement | Escalation |
|------------|-------------|----------------------|------------|
| **Critical** | 16 to 25 | Immediate action required; executive oversight | CISO and Executive Committee |
| **High** | 10 to 15 | Priority treatment within 30 days | Risk Management Committee |
| **Medium** | 5 to 9 | Treatment planning within 90 days | Department Head |
| **Low** | 1 to 4 | Monitor and include in annual review | Risk Owner |

---

## G. Roles and Responsibilities

### G.1 Risk Assessment Participants

| Role | Responsibilities |
|------|-----------------|
| **Chief Information Security Officer (CISO)** | Owns the risk assessment methodology; ensures adequate resources; reports enterprise risk posture to executive leadership |
| **Risk Management Committee** | Approves risk tolerance thresholds; reviews critical and high risks; authorizes treatment investments |
| **GRC Team** | Facilitates risk assessments; maintains the risk register; produces risk reports and dashboards |
| **Risk Owners** | Accept accountability for assigned risks; implement treatment plans; monitor risk status |
| **Business Unit Leaders** | Participate in risk identification; provide subject matter expertise; allocate resources for treatment |
| **IT Security Team** | Conduct technical risk assessments; implement security controls; monitor technical risk indicators |
| **Internal Audit** | Provide independent assurance on risk management effectiveness; validate control performance |
| **Process Owners** | Identify operational risks within their processes; implement procedural controls |

### G.2 Assessment Participation Matrix

| Assessment Type | Lead | Participants | Approver |
|-----------------|------|--------------|----------|
| Enterprise Risk Assessment | GRC Team | All Business Units, IT Security | Risk Management Committee |
| Information Security Risk Assessment | IT Security | GRC Team, IT Operations | CISO |
| Vendor Risk Assessment | GRC Team | Procurement, Legal, IT Security | Vendor Management Committee |
| Project Risk Assessment | Project Manager | GRC Team, Technical Leads | Project Sponsor |
| Compliance Risk Assessment | GRC Team | Legal, Compliance Officers | Chief Compliance Officer |

---

## H. Outputs and Reporting

### H.1 Assessment Deliverables

| Deliverable | Description | Frequency |
|-------------|-------------|-----------|
| **Risk Register** | Complete inventory of identified risks with all attributes | Continuous |
| **Risk Heat Map** | Visual representation of risk distribution by likelihood and impact | Quarterly |
| **Executive Risk Summary** | High-level overview of critical and high risks for leadership | Monthly |
| **Risk Treatment Status Report** | Progress on treatment implementation and residual risk trends | Monthly |
| **Risk Trend Analysis** | Historical comparison showing risk level changes over time | Quarterly |
| **Control Effectiveness Report** | Assessment of control performance and gaps | Semi-annually |
| **Assessment Completion Report** | Detailed findings from specific risk assessments | Per assessment |

### H.2 Reporting Distribution

| Report | Audience | Format |
|--------|----------|--------|
| Executive Risk Dashboard | Executive Committee, Board | Interactive dashboard |
| Risk Register Extract | Risk Management Committee | Spreadsheet and narrative |
| Department Risk Summary | Business Unit Leaders | Presentation and summary document |
| Technical Risk Report | IT Leadership | Detailed technical documentation |
| Compliance Risk Briefing | Legal and Compliance | Regulatory-focused summary |

### H.3 Sample Risk Heat Map Format

A risk heat map visualizes the distribution of risks across the likelihood-impact matrix. Each risk is plotted as a data point, with clustering indicating risk concentrations requiring management attention.

Heat maps are color-coded:
- **Red:** Critical risks requiring immediate action
- **Orange:** High risks requiring priority treatment
- **Yellow:** Medium risks requiring planned treatment
- **Green:** Low risks for monitoring

---

## I. Integration with GRC Program

### I.1 ServiceNow GRC Implementation

Risk assessments are conducted and documented within the ServiceNow GRC platform. The platform provides:

- Automated risk register with workflow capabilities
- Integration with control testing and compliance activities
- Real-time dashboards and reporting
- Issue tracking for treatment activities
- Audit trail for all risk management activities

### I.2 Related Processes

| Process | Integration Point |
|---------|------------------|
| **Incident Management** | Risk assessments triggered by security incidents; incident data informs likelihood estimates |
| **Change Management** | Risk assessments required for significant changes; change data identifies emerging risks |
| **Vendor Management** | Vendor risk assessments inform procurement decisions; vendor performance affects third-party risk ratings |
| **Audit Management** | Audit findings identify control gaps; risk assessments inform audit planning |
| **Business Continuity** | Business impact analysis feeds impact ratings; recovery requirements inform treatment priorities |

---

## J. Related Documents

The following documents support and complement this methodology:

1. Enterprise Risk Management Policy
2. Information Security Policy
3. Risk Management Policy
4. Access Control Policy
5. Incident Management Policy
6. Business Continuity and Disaster Recovery Policy
7. Third-Party Risk Management Policy
8. IT Governance Framework (COBIT)
9. Data Classification Standard
10. Control Testing Procedures

---

## K. Compliance and Monitoring

### K.1 Compliance Requirements

This methodology supports compliance with:

- **SOC 2 Type II:** Risk assessment and monitoring controls
- **ISO 27001:** Clause 6.1 (Actions to address risks and opportunities)
- **NIST Cybersecurity Framework:** ID.RA (Risk Assessment)
- **GDPR:** Article 32 (Security of processing) and Article 35 (Data protection impact assessment)
- **COBIT 2019:** APO12 (Managed Risk)

### K.2 Methodology Effectiveness Metrics

| Metric | Target | Measurement Frequency |
|--------|--------|----------------------|
| Risk Assessment Completion Rate | 100% of scheduled assessments | Quarterly |
| Risk Register Currency | All risks reviewed within defined cycle | Monthly |
| Treatment Plan Completion | 90% of treatments completed on time | Quarterly |
| Critical Risk Reduction | 25% annual reduction in critical risks | Annually |
| Risk Event Prediction Rate | 80% of incidents covered by identified risks | Annually |

---

## L. Continuous Improvement

### L.1 Methodology Review

This methodology undergoes review and update:

- **Annual Review:** Comprehensive evaluation of methodology effectiveness
- **Triggered Review:** Following significant incidents, regulatory changes, or organizational changes
- **Benchmark Review:** Comparison against industry practices and emerging standards

### L.2 Improvement Activities

1. **Lessons Learned Integration:** Incorporate findings from risk events and near-misses
2. **Stakeholder Feedback:** Collect input from assessment participants on process effectiveness
3. **Tool Enhancement:** Improve risk register and reporting capabilities based on user needs
4. **Training Updates:** Refresh risk assessment training based on methodology changes
5. **Framework Alignment:** Update methodology as referenced standards are revised

### L.3 Version Control

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 1.0 | 2024-05-22 | GRC Team | Initial release |

---

## M. Exceptions

Exceptions to this methodology require written approval from the Chief Information Security Officer. Exception requests must document:

- Justification for the exception
- Alternative risk assessment approach to be used
- Duration of the exception
- Compensating measures

Approved exceptions are recorded in the GRC exception register and reviewed quarterly.

---

## N. Enforcement

Compliance with this methodology is mandatory for all risk assessment activities. Non-compliance may result in:

- Invalid risk assessments requiring remediation
- Escalation to risk governance bodies
- Performance management actions for responsible parties
- Audit findings and remediation requirements

---

## O. Framework Alignment Summary

| Framework | Relevant Controls and Requirements |
|-----------|-----------------------------------|
| **ISO 31000:2018** | Clause 6: Risk assessment process |
| **NIST SP 800-30 Rev 1** | Risk assessment process and guidance |
| **NIST CSF** | ID.RA-1 through ID.RA-6 |
| **ISO 27001:2022** | A.5.29, A.5.30, A.8.8 |
| **COBIT 2019** | APO12.01 through APO12.06 |
| **SOC 2** | CC3.1 through CC3.4 |
| **GDPR** | Articles 32 and 35 |

---

## P. Evidence of Compliance

| Evidence Type | Description | Frequency |
|---------------|-------------|-----------|
| Risk Register | Complete risk inventory in ServiceNow GRC | Continuous |
| Assessment Reports | Documented findings from risk assessments | Per assessment |
| Heat Maps | Visual risk distribution reports | Quarterly |
| Committee Minutes | Risk Management Committee meeting records | Monthly |
| Treatment Plans | Documented risk treatment activities | Per risk |
| KRI Dashboards | Key risk indicator monitoring reports | Weekly to quarterly |
| Training Records | Risk assessment training completion | Annual |
| Review Records | Methodology review and update documentation | Annual |

---

## Appendix A: Risk Assessment Checklist

Use this checklist to ensure completeness for each risk assessment:

**Planning Phase:**
- [ ] Assessment scope defined and documented
- [ ] Stakeholders identified and notified
- [ ] Assessment timeline established
- [ ] Required inputs gathered (asset inventory, prior assessments, incident data)

**Identification Phase:**
- [ ] Asset inventory reviewed and updated
- [ ] Threat sources cataloged
- [ ] Vulnerabilities documented
- [ ] Stakeholder interviews conducted
- [ ] Risk scenarios developed

**Analysis Phase:**
- [ ] Likelihood ratings assigned with justification
- [ ] Impact ratings assigned across all dimensions
- [ ] Existing controls documented
- [ ] Control effectiveness evaluated
- [ ] Inherent and residual risk scores calculated

**Evaluation Phase:**
- [ ] Risks compared against tolerance thresholds
- [ ] Risks prioritized by score
- [ ] Treatment recommendations documented
- [ ] Heat map generated

**Documentation Phase:**
- [ ] Risk register updated in ServiceNow GRC
- [ ] Risk owners assigned and notified
- [ ] Treatment plans documented
- [ ] Assessment report completed

**Review Phase:**
- [ ] Findings reviewed with stakeholders
- [ ] Treatment plans approved
- [ ] Next assessment scheduled
- [ ] Lessons learned captured

---

## Appendix B: Risk Scenario Template

Use this template to document identified risk scenarios:

**Risk Scenario ID:** [Unique identifier]

**Risk Title:** [Brief descriptive name]

**Risk Description:**
[Detailed narrative describing the threat source, vulnerability exploited, and potential consequence]

**Threat Source:**
- [ ] Adversarial (malicious actor)
- [ ] Accidental (human error)
- [ ] Structural (equipment failure)
- [ ] Environmental (natural disaster)

**Affected Assets:**
[List of impacted systems, data, processes, or third parties]

**Existing Controls:**
[Current measures that reduce the likelihood or impact]

**Likelihood Rationale:**
[Justification for the assigned likelihood rating]

**Impact Rationale:**
[Justification for the assigned impact rating, including affected impact dimensions]

**Risk Owner:**
[Individual accountable for this risk]

---

*Document Owner: Chief Information Security Officer*  
*Last Updated: 2024-05-22*  
*Next Review: 2025-05-22*

# Risk Assessment Report

**Emyzer Technology – ServiceNow GRC Risk Assessment Document**

---

## Assessment Metadata

| Field | Value |
|-------|-------|
| **Assessment Name** | [Risk Assessment Name] |
| **Assessment ID** | [RA-YYYY-###] |
| **Assessment Type** | Annual / Project-Based / Triggered / Continuous |
| **Scope** | [System, Process, Department, or Enterprise-wide] |
| **Owner** | [Assessment Owner Name] |
| **Owning Group** | [Department/Team Name] |
| **State** | Draft / In Progress / Under Review / Complete |
| **Assessment Date** | [YYYY-MM-DD] |
| **Next Review Date** | [YYYY-MM-DD] |
| **Related Policy** | Risk Management Policy |
| **Knowledge Base** | Governance, Risk, and Compliance |

---

## Executive Summary

**Purpose:** [One sentence describing why this assessment was conducted.]

**Scope Summary:** [Brief description of what was assessed—systems, processes, data, third parties.]

**Key Findings:** [2-3 sentences summarizing the most significant risks identified.]

**Overall Risk Rating:** Critical / High / Medium / Low

**Recommendations:** [1-2 sentences on priority actions.]

---

## A. Assessment Objectives

This risk assessment was conducted to:

1. [Objective 1: e.g., Identify threats and vulnerabilities to information assets]
2. [Objective 2: e.g., Evaluate the likelihood and impact of identified risks]
3. [Objective 3: e.g., Prioritize risks for treatment based on organizational risk appetite]
4. [Objective 4: e.g., Recommend controls to mitigate unacceptable risks]
5. [Objective 5: e.g., Support compliance with regulatory and framework requirements]

---

## B. Scope and Boundaries

### In Scope

| Category | Items Included |
|----------|----------------|
| **Systems** | [List systems, applications, or platforms assessed] |
| **Data** | [List data types or classifications included] |
| **Processes** | [List business processes covered] |
| **Locations** | [List physical or logical locations] |
| **Third Parties** | [List vendors or partners included] |

### Out of Scope

| Category | Items Excluded | Reason |
|----------|----------------|--------|
| [Category] | [Item] | [Rationale for exclusion] |
| [Category] | [Item] | [Rationale for exclusion] |

### Boundaries and Constraints

- [Constraint 1: e.g., Assessment limited to production environment only]
- [Constraint 2: e.g., Third-party systems assessed based on questionnaire responses only]
- [Constraint 3: e.g., Physical security excluded—covered in separate assessment]

---

## C. Methodology

### Risk Assessment Framework

This assessment follows [Framework Name, e.g., NIST SP 800-30, ISO 31000, FAIR] methodology.

### Risk Calculation Formula

**Risk Score = Likelihood × Impact**

### Likelihood Scale

| Rating | Score | Description | Frequency |
|--------|-------|-------------|-----------|
| **Rare** | 1 | Highly unlikely to occur | Less than once per 5 years |
| **Unlikely** | 2 | Could occur but not expected | Once per 2-5 years |
| **Possible** | 3 | May occur at some point | Once per 1-2 years |
| **Likely** | 4 | Will probably occur | Multiple times per year |
| **Almost Certain** | 5 | Expected to occur frequently | Monthly or more often |

### Impact Scale

| Rating | Score | Financial Impact | Operational Impact | Reputational Impact |
|--------|-------|------------------|-------------------|---------------------|
| **Negligible** | 1 | < $10,000 | Minimal disruption, < 1 hour | No external awareness |
| **Minor** | 2 | $10,000 - $50,000 | Limited disruption, < 4 hours | Limited local awareness |
| **Moderate** | 3 | $50,000 - $250,000 | Significant disruption, < 1 day | Regional/industry awareness |
| **Major** | 4 | $250,000 - $1,000,000 | Severe disruption, 1-7 days | National media coverage |
| **Catastrophic** | 5 | > $1,000,000 | Critical failure, > 7 days | International coverage, regulatory action |

### Risk Rating Matrix

|  | **Impact** |||||
|--|------------|-----|-----|-----|-----|
| **Likelihood** | Negligible (1) | Minor (2) | Moderate (3) | Major (4) | Catastrophic (5) |
| Almost Certain (5) | 5 - Medium | 10 - High | 15 - High | 20 - Critical | 25 - Critical |
| Likely (4) | 4 - Low | 8 - Medium | 12 - High | 16 - Critical | 20 - Critical |
| Possible (3) | 3 - Low | 6 - Medium | 9 - Medium | 12 - High | 15 - High |
| Unlikely (2) | 2 - Low | 4 - Low | 6 - Medium | 8 - Medium | 10 - High |
| Rare (1) | 1 - Low | 2 - Low | 3 - Low | 4 - Low | 5 - Medium |

### Risk Rating Thresholds

| Rating | Score Range | Response Requirement |
|--------|-------------|---------------------|
| **Critical** | 16-25 | Immediate action required; escalate to executive leadership |
| **High** | 10-15 | Priority treatment within 30 days; management attention required |
| **Medium** | 5-9 | Treatment within 90 days; standard risk management process |
| **Low** | 1-4 | Accept or monitor; address opportunistically |

---

## D. Asset Inventory

| Asset ID | Asset Name | Asset Type | Owner | Classification | Criticality |
|----------|------------|------------|-------|----------------|-------------|
| [A-001] | [Asset Name] | Hardware / Software / Data / Process / People | [Owner] | Public / Internal / Confidential / Restricted | Critical / High / Medium / Low |
| [A-002] | [Asset Name] | [Type] | [Owner] | [Classification] | [Criticality] |
| [A-003] | [Asset Name] | [Type] | [Owner] | [Classification] | [Criticality] |
| [A-004] | [Asset Name] | [Type] | [Owner] | [Classification] | [Criticality] |
| [A-005] | [Asset Name] | [Type] | [Owner] | [Classification] | [Criticality] |

---

## E. Threat and Vulnerability Identification

### Threat Sources

| Threat ID | Threat Source | Threat Type | Motivation/Cause | Capability |
|-----------|---------------|-------------|------------------|------------|
| [T-001] | [e.g., External Attacker] | Adversarial / Accidental / Structural / Environmental | [e.g., Financial gain] | High / Medium / Low |
| [T-002] | [e.g., Insider Threat] | [Type] | [Motivation] | [Capability] |
| [T-003] | [e.g., Natural Disaster] | [Type] | [Cause] | [Capability] |
| [T-004] | [e.g., System Failure] | [Type] | [Cause] | [Capability] |

### Vulnerabilities Identified

| Vuln ID | Vulnerability | Affected Asset(s) | Related Threat(s) | Severity |
|---------|---------------|-------------------|-------------------|----------|
| [V-001] | [e.g., Unpatched software] | [Asset ID(s)] | [Threat ID(s)] | Critical / High / Medium / Low |
| [V-002] | [e.g., Weak authentication] | [Asset ID(s)] | [Threat ID(s)] | [Severity] |
| [V-003] | [e.g., Lack of encryption] | [Asset ID(s)] | [Threat ID(s)] | [Severity] |
| [V-004] | [e.g., Insufficient logging] | [Asset ID(s)] | [Threat ID(s)] | [Severity] |

---

## F. Risk Register

| Risk ID | Risk Description | Threat | Vulnerability | Affected Asset(s) | Likelihood | Impact | Inherent Risk Score | Existing Controls | Residual Risk Score | Risk Owner |
|---------|------------------|--------|---------------|-------------------|------------|--------|---------------------|-------------------|---------------------|------------|
| [R-001] | [Description of risk scenario] | [T-###] | [V-###] | [A-###] | [1-5] | [1-5] | [Score] - [Rating] | [Current controls in place] | [Score] - [Rating] | [Owner] |
| [R-002] | [Description] | [T-###] | [V-###] | [A-###] | [1-5] | [1-5] | [Score] - [Rating] | [Controls] | [Score] - [Rating] | [Owner] |
| [R-003] | [Description] | [T-###] | [V-###] | [A-###] | [1-5] | [1-5] | [Score] - [Rating] | [Controls] | [Score] - [Rating] | [Owner] |
| [R-004] | [Description] | [T-###] | [V-###] | [A-###] | [1-5] | [1-5] | [Score] - [Rating] | [Controls] | [Score] - [Rating] | [Owner] |
| [R-005] | [Description] | [T-###] | [V-###] | [A-###] | [1-5] | [1-5] | [Score] - [Rating] | [Controls] | [Score] - [Rating] | [Owner] |

---

## G. Risk Treatment Plan

| Risk ID | Risk Rating | Treatment Strategy | Recommended Controls | Priority | Target Date | Responsible Party | Status | Estimated Cost |
|---------|-------------|-------------------|----------------------|----------|-------------|-------------------|--------|----------------|
| [R-001] | [Rating] | Mitigate / Transfer / Accept / Avoid | [Specific control recommendations] | Critical / High / Medium / Low | [YYYY-MM-DD] | [Name/Role] | Not Started / In Progress / Complete | [$X,XXX] |
| [R-002] | [Rating] | [Strategy] | [Controls] | [Priority] | [Date] | [Party] | [Status] | [$X,XXX] |
| [R-003] | [Rating] | [Strategy] | [Controls] | [Priority] | [Date] | [Party] | [Status] | [$X,XXX] |
| [R-004] | [Rating] | [Strategy] | [Controls] | [Priority] | [Date] | [Party] | [Status] | [$X,XXX] |
| [R-005] | [Rating] | [Strategy] | [Controls] | [Priority] | [Date] | [Party] | [Status] | [$X,XXX] |

### Treatment Strategy Definitions

| Strategy | Definition | When to Use |
|----------|------------|-------------|
| **Mitigate** | Implement controls to reduce likelihood or impact | Risk exceeds appetite; cost-effective controls available |
| **Transfer** | Shift risk to third party (insurance, outsourcing) | Risk cannot be fully mitigated internally; transfer is cost-effective |
| **Accept** | Acknowledge risk without additional action | Risk within appetite; cost of treatment exceeds benefit |
| **Avoid** | Eliminate the activity or asset creating the risk | Risk unacceptable; no viable mitigation or transfer options |

---

## H. Risk Summary Dashboard

### Risk Distribution by Rating

| Rating | Count | Percentage |
|--------|-------|------------|
| Critical | [#] | [%] |
| High | [#] | [%] |
| Medium | [#] | [%] |
| Low | [#] | [%] |
| **Total** | **[#]** | **100%** |

### Risk Distribution by Category

| Category | Critical | High | Medium | Low | Total |
|----------|----------|------|--------|-----|-------|
| Technical | [#] | [#] | [#] | [#] | [#] |
| Operational | [#] | [#] | [#] | [#] | [#] |
| Compliance | [#] | [#] | [#] | [#] | [#] |
| Strategic | [#] | [#] | [#] | [#] | [#] |
| **Total** | **[#]** | **[#]** | **[#]** | **[#]** | **[#]** |

### Top 5 Risks Requiring Immediate Attention

| Rank | Risk ID | Risk Description | Risk Score | Treatment Priority |
|------|---------|------------------|------------|-------------------|
| 1 | [R-###] | [Brief description] | [Score] | [Priority] |
| 2 | [R-###] | [Brief description] | [Score] | [Priority] |
| 3 | [R-###] | [Brief description] | [Score] | [Priority] |
| 4 | [R-###] | [Brief description] | [Score] | [Priority] |
| 5 | [R-###] | [Brief description] | [Score] | [Priority] |

---

## I. Framework Alignment

| Framework | Description | Alignment |
|-----------|-------------|-----------|
| **NIST SP 800-30 Rev. 1** | Risk Assessment Guide | Task 2-1 (Threat identification), Task 2-2 (Vulnerability identification), Task 2-3 (Likelihood determination), Task 2-4 (Impact determination), Task 2-5 (Risk determination) |
| **NIST SP 800-53 Rev. 5** | Security and Privacy Controls | RA-1 (Policy and Procedures), RA-2 (Security Categorization), RA-3 (Risk Assessment), RA-5 (Vulnerability Monitoring), RA-7 (Risk Response) |
| **ISO/IEC 27005:2022** | Information Security Risk Management | Clause 7 (Context establishment), Clause 8 (Risk assessment), Clause 9 (Risk treatment), Clause 10 (Risk acceptance) |
| **ISO 31000:2018** | Risk Management Framework | Clause 5.4 (Risk assessment), Clause 5.5 (Risk treatment), Clause 6 (Process) |
| **NIST Cybersecurity Framework** | Cybersecurity Risk Management | ID.RA (Risk Assessment), ID.RM (Risk Management Strategy), RS.MI (Mitigation) |
| **COBIT 2019** | IT Governance and Management | APO12 (Managed Risk), EDM03 (Ensured Risk Optimization) |
| **FAIR** | Factor Analysis of Information Risk | Risk quantification methodology for cyber and operational risk |

---

## J. Assumptions and Limitations

### Assumptions

1. [Assumption 1: e.g., Information provided by asset owners is accurate and complete]
2. [Assumption 2: e.g., Threat landscape reflects current intelligence as of assessment date]
3. [Assumption 3: e.g., Existing controls are operating as designed]
4. [Assumption 4: e.g., Risk appetite statements reflect current organizational tolerance]

### Limitations

1. [Limitation 1: e.g., Assessment based on point-in-time data; risks may change]
2. [Limitation 2: e.g., Some systems could not be scanned due to operational constraints]
3. [Limitation 3: e.g., Third-party risk based on self-reported questionnaires]
4. [Limitation 4: e.g., Quantitative financial impacts are estimates based on industry benchmarks]

---

## K. Recommendations

### Immediate Actions (0-30 Days)

1. [Recommendation 1: Address critical/high risks requiring immediate attention]
2. [Recommendation 2: Specific control implementation]
3. [Recommendation 3: Escalation or communication requirement]

### Short-Term Actions (30-90 Days)

1. [Recommendation 1: Address remaining high and medium risks]
2. [Recommendation 2: Process or policy improvements]
3. [Recommendation 3: Training or awareness initiatives]

### Long-Term Actions (90+ Days)

1. [Recommendation 1: Strategic risk reduction initiatives]
2. [Recommendation 2: Architecture or technology improvements]
3. [Recommendation 3: Continuous monitoring enhancements]

---

## L. Related Documents

1. Risk Management Policy
2. Information Security Policy
3. [Previous Risk Assessment Report]
4. [Vulnerability Assessment Report]
5. [Threat Intelligence Report]
6. [Business Impact Analysis]
7. [Control Testing Results]

---

## M. Approval and Sign-Off

| Role | Name | Signature | Date |
|------|------|-----------|------|
| Assessment Lead | [Name] | | [YYYY-MM-DD] |
| Risk Owner | [Name] | | [YYYY-MM-DD] |
| IT Security Manager | [Name] | | [YYYY-MM-DD] |
| CISO / Executive Sponsor | [Name] | | [YYYY-MM-DD] |

### Approval Comments

| Date | Reviewer | Comments |
|------|----------|----------|
| [YYYY-MM-DD] | [Name] | "[Comments on assessment findings and recommendations]" |

---

## Appendices

### Appendix A: Detailed Risk Scenarios

[Include detailed risk scenario narratives for critical and high risks if needed]

### Appendix B: Control Gap Analysis

[Include mapping of recommended controls to existing control gaps]

### Appendix C: Supporting Evidence

[Reference vulnerability scan reports, penetration test results, or other technical evidence]

---

*This risk assessment document was generated from ServiceNow GRC and formatted for portfolio presentation.*

---

## Template Usage Notes (Remove Before Use)

### How to Use This Template

1. **Replace all bracketed placeholders** `[text]` with your specific content
2. **Customize scales** to match your organization's risk appetite and tolerance
3. **Adjust financial thresholds** in the Impact Scale to reflect your organization's materiality
4. **Add or remove risk entries** in the Risk Register based on actual findings
5. **Remove this section** before publishing

### Risk Assessment Best Practices

| Practice | Rationale |
|----------|-----------|
| **Use consistent IDs** | Enables traceability (R-001 → T-001 → V-001 → A-001) |
| **Document assumptions** | Provides context for risk ratings and supports defensibility |
| **Separate inherent vs. residual risk** | Shows value of existing controls |
| **Assign risk owners** | Establishes accountability for treatment |
| **Include cost estimates** | Supports business case for risk treatment |
| **Map to frameworks** | Demonstrates compliance alignment |

### Common Risk Categories

| Category | Examples |
|----------|----------|
| **Technical** | System vulnerabilities, misconfigurations, technical debt |
| **Operational** | Process failures, human error, capacity constraints |
| **Compliance** | Regulatory violations, audit findings, contractual breaches |
| **Strategic** | Market changes, competitive threats, technology obsolescence |
| **Financial** | Budget overruns, fraud, economic conditions |
| **Reputational** | Brand damage, customer trust, public relations |

### ServiceNow GRC Integration Notes

- Risk Register entries map to `sn_risk_risk` table
- Risk Assessments map to `sn_risk_assessment` table
- Treatment Plans map to `sn_risk_response_task` table
- Use consistent naming conventions for cross-referencing

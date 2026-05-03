# Quarterly Board / Executive GRC Report — Template

---

## Template Metadata

| Field               | Value                                                                                    |
|---------------------|------------------------------------------------------------------------------------------|
| Template ID         | TMPL-BR-001                                                                              |
| Version             | 1.0                                                                                      |
| Status              | Active                                                                                   |
| Purpose             | Quarterly executive/board GRC reporting on information security and risk posture         |
| Owner               | CISO / GRC Team                                                                          |
| Approved By         | CISO                                                                                     |
| Review Frequency    | Annual (or following material change to reporting requirements)                          |
| GitHub Reference    | https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/templates/board-report-v1.md |

---

## Instructions for Use

**Purpose of this template**
This template is used by the GRC team to produce the Quarterly Board / Executive GRC Report. The report is presented to the board (or its delegated sub-committee, e.g. Audit & Risk Committee) to provide assurance on the organisation's information security posture, regulatory compliance status, and material risk changes.

**Frequency and timing**
Produce this report within 15 business days of the end of each calendar quarter (31 March, 30 June, 30 September, 31 December). The draft must be circulated to the CISO for review at least 5 business days before the board meeting at which it will be presented.

**Who prepares this report**
The GRC Lead or GRC Analyst assembles the report based on inputs from risk owners, the ISO, legal counsel, and other control owners. The CISO reviews, amends, and owns the final report.

**Who approves and presents**
The CISO approves the report before distribution. The CISO (or ISO on delegation) presents Section 1–10 to the board or executive committee. Supporting detail is available on request but is not included in the main report pack.

**Guidance for each section**
Section-level guidance appears in *italics* within each section below. Remove all guidance notes and placeholder text before finalising the report for distribution.

**Classification**
This report is classified at minimum **Confidential**. Handle, store, and distribute accordingly. Do not circulate outside board members and designated executive recipients without CISO approval.

---

## Section 1: Report Header

| Field               | Detail                                         |
|---------------------|------------------------------------------------|
| Organisation        | [ORGANISATION NAME]                            |
| Reporting Period    | [Q1 / Q2 / Q3 / Q4 YYYY — e.g., Q1 2025]      |
| Report Reference    | [GRC-BR-YYYY-QN — e.g., GRC-BR-2025-Q1]       |
| Prepared By         | [Name, Role]                                   |
| Reviewed By         | [CISO Name]                                    |
| Review Date         | [YYYY-MM-DD]                                   |
| Board Meeting Date  | [YYYY-MM-DD]                                   |
| Classification      | [Confidential / Restricted]                    |
| Version             | [e.g., v1.0 — increment for each revision]     |

---

## Section 2: Executive Summary

*Write 3–4 sentences maximum. This section is read independently by board members who may not review the rest of the report. State: (1) the overall risk posture verdict (Improving / Stable / Deteriorating) and a one-sentence rationale; (2) the one or two issues most requiring board attention or decision this quarter; (3) any material regulatory change or external threat development relevant to the board's oversight role. Do not include operational detail here — direct the reader to the relevant section for detail. Avoid technical jargon.*

**Overall Risk Posture: [IMPROVING / STABLE / DETERIORATING]**

[EXECUTIVE SUMMARY TEXT — 3–4 sentences]

*Example (do not copy verbatim):*
*"The overall information security risk posture is assessed as Stable this quarter. Remediation of three high-severity findings from the Q3 internal audit is on track, with two closed and one expected to close by [date]. The board's attention is drawn to Section 7, which notes the approaching deadline for [regulatory obligation]. No regulatory-reportable incidents occurred during the period."*

---

## Section 3: Risk Posture Dashboard

*Update the RAG rating and trend indicator for each domain based on evidence gathered during the quarter. Use the RAG definitions in Appendix A. The trend indicator reflects movement since the previous quarterly report: ↑ = improving, ↓ = deteriorating, → = stable. The "Change Since Last Report" column should briefly explain what drove any rating change.*

| Risk Domain              | Risk Level (RAG) | Trend (↑ ↓ →) | Notes                                         | Change Since Last Report         |
|--------------------------|------------------|----------------|-----------------------------------------------|----------------------------------|
| Information Security     | [RED/AMBER/GREEN] | [↑ ↓ →]       | [brief summary]                               | [what changed and why]           |
| Privacy / Data Protection | [RED/AMBER/GREEN] | [↑ ↓ →]      | [brief summary]                               | [what changed and why]           |
| AI Governance            | [RED/AMBER/GREEN] | [↑ ↓ →]       | [brief summary]                               | [what changed and why]           |
| Third-Party Risk         | [RED/AMBER/GREEN] | [↑ ↓ →]       | [brief summary]                               | [what changed and why]           |
| Business Continuity      | [RED/AMBER/GREEN] | [↑ ↓ →]       | [brief summary]                               | [what changed and why]           |
| Regulatory Compliance    | [RED/AMBER/GREEN] | [↑ ↓ →]       | [brief summary]                               | [what changed and why]           |

*See Appendix A for RAG definitions.*

---

## Section 4: Key Risk Register Changes

*Include only risks where the rating, ownership, or treatment status changed materially during the quarter. Do not list all risks in the register. Focus on movements to RED or movements from RED to AMBER/GREEN, newly identified HIGH risks, and risks where the board previously requested monitoring. Omit risks that remained stable.*

| Risk ID      | Risk Title                    | Previous Rating | Current Rating | Change Driver                              | Action Required                  |
|--------------|-------------------------------|-----------------|----------------|--------------------------------------------|----------------------------------|
| [RISK-XXX]   | [Risk title]                  | [H/M/L/Critical] | [H/M/L/Critical] | [what caused the change]                | [decision or monitoring required] |
| [RISK-XXX]   | [Risk title]                  | [H/M/L/Critical] | [H/M/L/Critical] | [what caused the change]                | [decision or monitoring required] |
| [RISK-XXX]   | [Risk title]                  | [H/M/L/Critical] | [H/M/L/Critical] | [what caused the change]                | [decision or monitoring required] |
| [RISK-XXX]   | [Risk title]                  | [H/M/L/Critical] | [H/M/L/Critical] | [what caused the change]                | [decision or monitoring required] |

*Add rows as needed. If no material changes occurred, state: "No material risk register changes this quarter."*

---

## Section 5: Open Findings and Remediation Status

*Include all open findings from internal audits, external audits, control tests, regulatory examinations, and penetration tests. Highlight any finding open for more than 90 days in **bold**. Do not include findings closed before the report date. Findings at Critical or High severity that are open for more than 90 days without a documented extension approval should be flagged to the board as a point of concern.*

| Finding ID     | Source                      | Severity         | Policy / Control Reference | Days Open | Status                  | Target Close Date |
|----------------|-----------------------------|------------------|----------------------------|-----------|-------------------------|-------------------|
| [FND-YYYY-NNN] | [Audit / Control Test / Pen Test] | [Crit/High/Med/Low] | [policy + section]    | [N days]  | [In Progress / Overdue / Blocked] | [YYYY-MM-DD] |
| [FND-YYYY-NNN] | [Audit / Control Test / Pen Test] | [Crit/High/Med/Low] | [policy + section]    | [N days]  | [In Progress / Overdue / Blocked] | [YYYY-MM-DD] |
| [FND-YYYY-NNN] | [Audit / Control Test / Pen Test] | [Crit/High/Med/Low] | [policy + section]    | [N days]  | [In Progress / Overdue / Blocked] | [YYYY-MM-DD] |
| [FND-YYYY-NNN] | [Audit / Control Test / Pen Test] | [Crit/High/Med/Low] | [policy + section]    | [N days]  | [In Progress / Overdue / Blocked] | [YYYY-MM-DD] |

*Total open findings: [N] — Critical: [N] | High: [N] | Medium: [N] | Low: [N]*
*Findings open >90 days: [N] — [list IDs if any; explain board-level action required]*

---

## Section 6: Control Performance

*Summarise control testing activity completed during the quarter. Include only domains where testing was performed. Do not include domains where no testing was scheduled this quarter — note those as "Not tested this period (scheduled [quarter])". The pass rate is the proportion of controls tested that were found fully effective.*

| Control Domain              | Controls Tested This Period | Pass Rate | Failures | Remediation Status                        |
|-----------------------------|-----------------------------|-----------|----------|-------------------------------------------|
| Access Control              | [N]                         | [X%]      | [N]      | [brief status of any remediation in progress] |
| Cryptography / Key Management | [N]                       | [X%]      | [N]      | [brief status]                            |
| Incident Management         | [N]                         | [X%]      | [N]      | [brief status]                            |
| Third-Party / Supplier Controls | [N]                     | [X%]      | [N]      | [brief status]                            |
| AI Governance Controls      | [N]                         | [X%]      | [N]      | [brief status]                            |
| Business Continuity         | [N]                         | [X%]      | [N]      | [brief status]                            |
| [Other domain]              | [N]                         | [X%]      | [N]      | [brief status]                            |

*Overall this period: [N] controls tested | [N] passed ([X%]) | [N] failed | [N] partially effective*

---

## Section 7: Compliance and Regulatory Obligations

*List all active regulatory and contractual compliance obligations relevant to information security, privacy, and AI governance. Update the status each quarter. Note any upcoming regulatory changes that will require policy, process, or technology changes. Flag any obligation where the status is "At Risk" or "Non-Compliant" to the board immediately — do not wait for the quarterly report cycle.*

| Obligation                         | Regulatory / Contractual Basis         | Status                          | Next Deadline    | Owner                  |
|------------------------------------|----------------------------------------|---------------------------------|------------------|------------------------|
| [Obligation title]                 | [e.g., UK GDPR Article 32 [VERIFY]]   | [Compliant / At Risk / Gap Identified] | [YYYY-MM-DD] | [role / name]       |
| [Obligation title]                 | [e.g., ISO 27001:2022 certification]  | [Compliant / At Risk / Gap Identified] | [YYYY-MM-DD] | [role / name]       |
| [Obligation title]                 | [e.g., EU AI Act Article 9 [VERIFY]]  | [Compliant / At Risk / Gap Identified] | [YYYY-MM-DD] | [role / name]       |
| [Obligation title]                 | [contractual — customer DPA]          | [Compliant / At Risk / Gap Identified] | [YYYY-MM-DD] | [role / name]       |
| [Obligation title]                 | [regulatory]                          | [Compliant / At Risk / Gap Identified] | [YYYY-MM-DD] | [role / name]       |

**Upcoming Regulatory Changes:**
*List any regulatory developments expected to affect obligations within the next 12 months. Include the anticipated implementation date, the nature of the change, and the current preparation status.*

| Regulatory Change                  | Anticipated Effective Date | Impact Assessment           | Preparation Status    |
|------------------------------------|----------------------------|-----------------------------|-----------------------|
| [regulation / guidance name]       | [YYYY-MM-DD]               | [High / Medium / Low]       | [Not Started / In Progress / Ready] |

---

## Section 8: Incidents and Near-Misses

*Report all information security incidents and privacy incidents that occurred or were discovered during the reporting period. Include near-misses where lessons-learned actions are outstanding. Incidents that met the regulatory reporting threshold should be clearly identified in a separate row or flagged with an asterisk (*). For each incident, state whether any required notifications were made and confirm that mandatory notification deadlines were met.*

| Incident ID    | Date       | Severity         | Description (brief)                            | Status           | Lessons Learned Applied? |
|----------------|------------|------------------|------------------------------------------------|------------------|--------------------------|
| [INC-YYYY-NNN] | [YYYY-MM-DD] | [Crit/High/Med/Low] | [1–2 sentence description]               | [Closed / Under Review / Monitoring] | [Yes / No / In Progress] |
| [INC-YYYY-NNN] | [YYYY-MM-DD] | [Crit/High/Med/Low] | [1–2 sentence description]               | [Closed / Under Review / Monitoring] | [Yes / No / In Progress] |

*Total incidents this period: [N] — Critical: [N] | High: [N] | Medium: [N] | Low: [N]*
*Regulatory-reportable incidents: [N] — [list IDs; confirm notifications made on time]*

*If no incidents: "No information security or privacy incidents were recorded during this reporting period."*

---

## Section 9: Decisions Required

*List only items that require a formal board or executive committee decision, policy acceptance, or risk acceptance at board level. Do not include items that are within management's delegated authority. Each item should identify the decision required, the consequence of not deciding, and the recommended course of action (optional — include if GRC team has a clear recommendation).*

- **[Decision Item 1]:** [Describe the decision required. State the consequence of not deciding. Identify any deadline.] *Recommended action: [Yes/No/Defer with conditions]*

- **[Decision Item 2]:** [Describe the decision required. State the consequence of not deciding.] *Recommended action: [Yes/No/Defer with conditions]*

- **[Decision Item 3]:** [Risk acceptance item — describe the residual risk being formally accepted, the duration of acceptance, and the conditions attached.]

*If no decisions are required: "No items require board decision this period. All risk and compliance matters are within management's delegated authority."*

---

## Section 10: Forward Look

*Summarise the key GRC activities, milestones, regulatory events, and risk triggers expected in the next 90 days. This helps the board anticipate items they will need to consider at the next reporting cycle. Include both planned activities (audits, certifications, exercises) and external events (regulatory deadlines, industry threat intelligence).*

| Period             | Item                                           | Risk Implication                     | Preparation Status    |
|--------------------|------------------------------------------------|--------------------------------------|-----------------------|
| [Month YYYY]       | [activity or event]                            | [risk if delayed or not completed]   | [On Track / At Risk / Not Started] |
| [Month YYYY]       | [activity or event]                            | [risk if delayed or not completed]   | [On Track / At Risk / Not Started] |
| [Month YYYY]       | [activity or event]                            | [risk if delayed or not completed]   | [On Track / At Risk / Not Started] |
| [Month YYYY]       | [regulatory deadline or audit window]          | [risk if not met]                    | [On Track / At Risk / Not Started] |
| [Month YYYY]       | [control testing or certification activity]    | [risk if not completed]              | [On Track / At Risk / Not Started] |

---

## Appendix A: RAG Definitions and Risk Level Glossary

### RAG Status Definitions

| Status | Colour | Definition                                                                                      |
|--------|--------|-------------------------------------------------------------------------------------------------|
| GREEN  | Green  | Risk is within appetite. Controls are effective. No material issues. Normal monitoring applies. |
| AMBER  | Amber  | Risk is approaching or slightly above appetite. One or more controls are weak or failing. Active management required. Board should be aware. |
| RED    | Red    | Risk is above appetite. Material control failure or compliance gap. Immediate escalation and board attention required. |

### Risk Rating Definitions (used in Risk Register)

| Rating   | Likelihood    | Impact        | Description                                                             |
|----------|---------------|---------------|-------------------------------------------------------------------------|
| Critical | Almost Certain| Catastrophic  | Existential or severe financial/regulatory/reputational consequence. Board-level risk acceptance required. |
| High     | Likely        | Major         | Significant impact on operations, compliance, or reputation. CISO-level ownership. |
| Medium   | Possible      | Moderate      | Manageable impact. Risk owner accountability. Standard monitoring.     |
| Low      | Unlikely      | Minor         | Within normal operational tolerance. Routine tracking only.            |

### Finding Severity Definitions

| Severity | Definition                                                                                                           |
|----------|----------------------------------------------------------------------------------------------------------------------|
| Critical | Immediate threat to confidentiality, integrity, or availability of critical data or systems. Requires immediate remediation. |
| High     | Significant control failure with potential for material harm. Remediation required within 30 days.                  |
| Medium   | Control weakness that increases risk but does not represent immediate material threat. Remediation within 90 days.  |
| Low      | Minor gap or improvement opportunity. Remediation within 180 days or next scheduled review cycle.                   |

---

*End of Template TMPL-BR-001 v1.0. Remove all guidance text (italicised instructions and placeholder labels) before distributing the completed report.*

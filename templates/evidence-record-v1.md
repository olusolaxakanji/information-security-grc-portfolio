# GRC Evidence Record: Template

---

## Template Metadata

| Field               | Value                                                                                        |
|---------------------|----------------------------------------------------------------------------------------------|
| Template ID         | TMPL-ER-001                                                                                  |
| Version             | 1.0                                                                                          |
| Status              | Active                                                                                       |
| Purpose             | Document individual evidence items for control testing and compliance assurance              |
| Owner               | GRC Team                                                                                     |
| Approved By         | ISO / GRC Lead                                                                               |
| Review Frequency    | Annual                                                                                       |
| GitHub Reference    | https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/templates/evidence-record-v1.md |

---

## Instructions for Use

**When to use this template**
Use an Evidence Record (ER) to document any individual piece of evidence collected in support of a control test, compliance assertion, audit response, or regulatory submission. Create one Evidence Record per discrete evidence item. Where a single piece of evidence supports multiple controls, one Evidence Record may reference multiple Control IDs, but the primary control must be identified.

**Difference between an Evidence Record and a Control Testing Record**
A **Control Testing Record** (see TMPL-CR-001) documents the overall test of a control: the methodology, sample, all evidence collected, the finding, and the management response. It is the parent record for a control test.

An **Evidence Record** documents a *single piece of evidence* that feeds into one or more control tests or compliance assertions. It is a child record. The relationship is: one Control Testing Record may reference many Evidence Records. Evidence Records may also exist independently of a control test: for example, to retain evidence in response to a regulatory inquiry or to document a compliance artefact for a certification audit.

**Numbering convention**
Evidence IDs follow the format ER-YYYY-NNNN (e.g., ER-2025-0042). Numbers are assigned sequentially by the GRC platform or by the GRC team's evidence log. Do not reuse IDs.

**Storage requirements**
All completed Evidence Records and their associated evidence artefacts must be stored in the designated GRC platform or document repository per the Evidence Retention and Management Procedure. Hardcopy evidence must be scanned and stored digitally within 5 business days of collection.

**Quality standard**
Evidence must be sufficient, reliable, relevant, and timely (SRRT). Section 5 of this template assesses these attributes. Evidence assessed as "Insufficient" in Section 5 cannot be used to satisfy a control requirement without supplementary evidence.

---

## Section 1: Evidence Identification

| Field               | Detail                                                                                    |
|---------------------|-------------------------------------------------------------------------------------------|
| Evidence ID         | [ER-YYYY-NNNN]                                                                            |
| Evidence Title      | [Descriptive title, e.g., "Q1 2025 User Access Review Approval Email, ServiceNow"]     |
| Evidence Type       | [Select one: Policy Document / Procedure / Log or Audit Trail / Screenshot / Test Result / Interview Notes / Contract / Certificate / Configuration Record / Training Record / Other: specify] |
| Date of Evidence    | [YYYY-MM-DD: the date the evidence was created or the event occurred]                   |
| Date Collected      | [YYYY-MM-DD: the date the GRC team obtained or captured the evidence]                   |
| Collected By        | [Full name, Role: e.g., Jane Smith, GRC Analyst]                                        |
| Evidence Reference  | [File name, ticket number, or unique identifier for the artefact]                        |

*The "Date of Evidence" and "Date Collected" may differ. For example, a log extracted on 2025-03-28 covering events from 2025-01-01 to 2025-03-31 has a Date of Evidence spanning that range, and a Date Collected of 2025-03-28. Always record both accurately.*

---

## Section 2: Control Reference

| Field                    | Detail                                                                                  |
|--------------------------|-----------------------------------------------------------------------------------------|
| Primary Control ID       | [e.g., ET-CTRL-001: use the organisation's control register ID]                       |
| Control Title            | [e.g., Access Control Review and Certification]                                         |
| Policy Reference         | [Policy name, section, and version: e.g., Access Control Policy v2.1, Section 4.3]   |
| Framework Reference      | [e.g., ISO 27001:2022 Annex A Control A.8.2 [VERIFY]; NIST CSF 2.0 PR.AA-05 [VERIFY]] |
| Secondary Controls       | [List any additional Control IDs this evidence also supports, if applicable]           |
| Testing Period           | [YYYY-MM-DD to YYYY-MM-DD: the control testing window this evidence supports]         |
| Associated Test Record   | [Reference to the parent Control Testing Record, e.g., CTR-2025-0018, if applicable]  |

*Framework references should be verified against the authoritative published standard before recording. Mark citations as [VERIFY] if not independently confirmed.*

---

## Section 3: Evidence Description

*Describe what the evidence is, what it shows, and why it satisfies the control requirement. Be specific: a reviewer unfamiliar with the control should be able to understand what the evidence demonstrates from this description alone. Note any limitations, gaps, or caveats. For example: if a log covers only part of the testing period, state what period is covered and why the remainder is unavailable. If the evidence is an extract rather than a complete record, state what was excluded and why.*

**What the evidence shows:**
[Describe the content and nature of the evidence item. What event, activity, or state does it document?]

**How it satisfies the control requirement:**
[Explain the specific control requirement or assertion this evidence supports. Reference the control objective.]

**Limitations or caveats:**
[Note any gaps, partial coverage, or reliability concerns. If none, state "None identified."]

---

## Section 4: Evidence Storage

| Field               | Detail                                                                                    |
|---------------------|-------------------------------------------------------------------------------------------|
| System of Record    | [e.g., GRC Platform (ServiceNow) / SharePoint Document Repository / SIEM / LMS / Email Archive / Physical File] |
| Storage Location    | [Full path, folder reference, or system record ID: sufficient for another reviewer to locate the artefact] |
| File Name / Format  | [e.g., ER-2025-0042_access-review-approval.pdf]                                          |
| Retention Period    | [State the applicable retention period per the Data Retention Policy: e.g., 7 years from collection date] |
| Retention Owner     | [Role responsible for ensuring retention obligations are met: e.g., GRC Lead]           |
| Access Restriction  | [Who can access this evidence: e.g., GRC Team, Internal Audit, External Auditors on request] |
| Destruction Date    | [YYYY-MM-DD: calculated from collection date + retention period, unless superseded by litigation hold] |

*Evidence stored outside the designated system of record must be approved by the GRC Lead and the reason documented here.*

---

## Section 5: Quality Assessment

*Complete this section to assess whether the evidence meets the SRRT standard (Sufficient, Reliable, Relevant, Timely). An overall assessment of "Satisfactory" is required before the evidence can be used to support a control test conclusion. If the overall assessment is "Requires Supplement" or "Insufficient," document the corrective action in the notes field.*

| Quality Attribute | Assessment                                | Notes / Explanation                                              |
|-------------------|-------------------------------------------|------------------------------------------------------------------|
| Completeness      | [Complete / Partial]                      | [If partial: describe what is missing and why]                   |
| Relevance         | [Directly relevant / Indirectly relevant] | [If indirect: explain the inferential link to the control]       |
| Reliability       | [Primary source / Secondary source]       | [Primary = direct from system of record; Secondary = derived, reported, or summarised] |
| Timeliness        | [Within required window: Yes / No]        | [State the required collection window and whether this evidence falls within it] |
| **Overall Assessment** | [**Satisfactory** / **Requires Supplement** / **Insufficient**] | [Summary conclusion and any required follow-up action] |

**If supplementary evidence is required:**
[Describe what additional evidence is needed, who is responsible for obtaining it, and the target date.]

---

## Section 6: Assessor Sign-Off

*All three sign-off roles must be completed before the Evidence Record is finalised. The "Accepted By" column represents the person who formally accepts the evidence as suitable for use in the control test or compliance submission.*

| Role            | Name                        | Date         | Signature / Initial |
|-----------------|-----------------------------|--------------|---------------------|
| Collected By    | [Name, Role]                | [YYYY-MM-DD] | [Initials]          |
| Reviewed By     | [Name, Role: peer reviewer or senior GRC analyst] | [YYYY-MM-DD] | [Initials] |
| Accepted By     | [Name, Role: GRC Lead, ISO, or designated approver] | [YYYY-MM-DD] | [Initials] |

---

## Appendix: Common Evidence Types by Control Domain

*This table provides guidance on the typical evidence types collected for each control domain. It is not exhaustive: the appropriate evidence type depends on the specific control being tested. Use as a starting point when planning evidence collection for a new control test cycle.*

| Control Domain                  | Typical Evidence Types                                                                                 |
|---------------------------------|--------------------------------------------------------------------------------------------------------|
| Access Control                  | Access review reports, provisioning/deprovisioning tickets, role change records, privileged access logs, RBAC configuration screenshots |
| Cryptography / Key Management   | Key management procedure, key inventory records, certificate expiry reports, rotation logs, HSM configuration records |
| Vulnerability Management        | Vulnerability scan reports, patch deployment records, exception logs, remediation tracking tickets      |
| Security Awareness and Training | LMS completion reports, training attendance records, phishing simulation results, competency assessment results |
| Incident Management             | Incident tickets, post-incident review reports, notification records, timeline documentation, lessons-learned logs |
| Third-Party Risk                | Vendor assessments, SOC 2 reports, ISO 27001 certificates, DPA execution records, SecurityScorecard exports |
| Business Continuity             | BCP test reports, DR test results, test invocation records, recovery time measurements, exercise after-action reports |
| Change Management               | Change Advisory Board (CAB) minutes, approved change tickets, post-implementation review records       |
| Data Protection / Privacy       | DPIA records, data subject request logs, consent records, data breach notification evidence, privacy impact assessments |
| AI Governance                   | AI system risk assessments, conformity declarations, operator training records, human oversight logs, model performance monitoring reports |
| Physical Security               | CCTV access records, visitor logs, clean desk audit results, secure disposal certificates              |
| Audit Logging and Monitoring    | SIEM alert records, log integrity verification reports, audit log configuration screenshots, retention verification |

---

*End of Template TMPL-ER-001 v1.0. Remove all guidance text (italicised instructions) before submitting a completed Evidence Record.*

# Control Testing and Performance Record — Template

---

## Template Metadata

| Field               | Value                                                                                        |
|---------------------|----------------------------------------------------------------------------------------------|
| Template ID         | TMPL-CR-001                                                                                  |
| Version             | 1.0                                                                                          |
| Status              | Active                                                                                       |
| Purpose             | Document control testing methodology, evidence collected, results, and findings              |
| Owner               | GRC Team                                                                                     |
| Approved By         | ISO / GRC Lead                                                                               |
| Review Frequency    | Annual                                                                                       |
| GitHub Reference    | https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/templates/control-record-v1.md |

---

## Instructions for Use

**Design Effectiveness vs. Operating Effectiveness testing**

These are two distinct test types, and both may be required for a given control:

**Design Effectiveness (DE)** testing evaluates whether a control is designed in a way that, if it operates as intended, would prevent or detect the risk it is meant to address. DE testing asks: "Is this control theoretically capable of doing what it is supposed to do?" DE testing is typically performed when a control is newly implemented, when the policy or procedure underpinning the control changes materially, or as part of an initial assessment. DE testing generally does not require a sample — it is a qualitative assessment of the control's design logic, assigned owner, documented procedure, and defined frequency.

**Operating Effectiveness (OE)** testing evaluates whether a control has actually operated as designed over a defined period. OE testing asks: "Did this control work, consistently, during the testing window?" OE testing requires a defined population and a sample drawn from it. Results are expressed in terms of exception rates. OE testing is performed periodically according to the control's testing frequency (see the organisation's Control Testing Schedule).

**When each is performed**
- Perform DE testing: on new controls; when a control's procedure, owner, or frequency changes materially; at least once every two years for all controls in the control framework.
- Perform OE testing: according to the Control Testing Schedule; more frequently for Critical and High controls; as a response to a finding or near-miss.

**Who performs control testing**
Control testing is performed by the GRC team or by internal audit. Control owners do not test their own controls — this would compromise independence. For ISO 27001 certification purposes, internal audit testing may supplement GRC testing but the ISO must document the overall assessment. External penetration testing and third-party audits may also contribute evidence but are documented separately before being referenced in this record.

**Numbering convention**
Control testing records follow the format CTR-YYYY-NNNN (e.g., CTR-2025-0023). Assigned sequentially by the GRC platform or GRC team log. Findings raised from this record follow the format FND-YYYY-NNNN.

**Relationship to Evidence Records**
Each piece of evidence collected during testing should be documented in a separate Evidence Record (TMPL-ER-001). Reference the Evidence Record IDs in Section 5 of this template. Do not attach raw evidence artefacts directly to this record unless required by the GRC platform's configuration.

---

## Section 1: Control Identification

| Field               | Detail                                                                                    |
|---------------------|-------------------------------------------------------------------------------------------|
| Control Testing Record ID | [CTR-YYYY-NNNN]                                                                    |
| Control ID          | [e.g., ET-CTRL-001 — use the Control Register ID]                                        |
| Control Title       | [e.g., Access Control Review and Certification]                                           |
| Policy Reference    | [Policy name, section, and version — e.g., Access Control Policy v2.1, Section 5.1]     |
| Control Objective   | [State the control objective in one sentence — what risk does this control mitigate?]    |
| Control Type        | [Preventive / Detective / Corrective]                                                    |
| Control Frequency   | [How often should the control operate — e.g., Quarterly / Monthly / Event-driven]       |
| Control Owner       | [Role — not name — of the person responsible for operating the control]                  |
| Testing Period      | [YYYY-MM-DD to YYYY-MM-DD — the period of activity covered by this test]                |
| Testing Conducted   | [YYYY-MM-DD — date the test was actually performed]                                      |
| Tester              | [Full name, Role — must be independent of the control owner]                             |
| Test Type           | [Design Effectiveness / Operating Effectiveness / Both]                                  |
| Scheduled or Ad Hoc | [Scheduled — per Control Testing Schedule / Ad Hoc — reason: [state reason]]            |
| Framework References | [e.g., ISO 27001:2022 Annex A A.8.2 [VERIFY]; NIST CSF 2.0 PR.AA-05 [VERIFY]]         |

---

## Section 2: Testing Methodology

*Complete this section before performing the test. Document the planned methodology so that the test can be reproduced by a different tester and reviewed by an auditor.*

| Field                    | Detail                                                                                    |
|--------------------------|-------------------------------------------------------------------------------------------|
| Population Definition    | [Describe the total population from which the sample will be drawn. E.g., "All user provisioning requests processed via the ITSM ticketing system between 2025-01-01 and 2025-03-31." State the total population size: N = [X]] |
| Sample Size              | [State the number of items selected: n = [X]. Provide the sampling rationale — e.g., "For a population of N > 100, a sample of 25 items is selected per AICPA Attribute Sampling guidance [VERIFY]. For a population of N = 25–100, sample of 10 items selected."] |
| Selection Method         | [Random (preferred) / Judgmental (explain criteria) / Systematic (explain interval)]     |
| Testing Approach         | [Select all that apply: Inquiry / Observation / Inspection of documentation / Re-performance / Automated data analysis] |
| Testing Procedure        | [Step-by-step description of exactly what the tester did to test this control. Be specific enough that a different tester could replicate the test and reach a comparable conclusion. Example: "1. Export all user access review records from ServiceNow for Q1 2025. 2. Using random number generator, select 25 records. 3. For each selected record, verify: (a) review was completed by an authorised certifier; (b) review decision was documented; (c) any access changes were actioned within the required timeframe. 4. Compare certifier identity against the Approved Certifier List."] |
| Tools Used               | [List any tools, scripts, or platforms used — e.g., ServiceNow export, Excel random sampling formula, SIEM query] |

---

## Section 3: Design Effectiveness Assessment

*Complete this section if Test Type includes "Design Effectiveness." If OE-only test, mark this section as "N/A — Design Effectiveness not tested this cycle."*

| Design Attribute                                             | Assessment          | Notes                                                    |
|--------------------------------------------------------------|---------------------|----------------------------------------------------------|
| Is the control objective clearly defined?                   | [Yes / No / Partial] | [observation]                                           |
| Is the control designed to address the identified risk?     | [Yes / No / Partial] | [does the control logic actually address the risk?]     |
| Is control frequency appropriate for the risk level?        | [Yes / No / Partial] | [e.g., is quarterly review frequent enough for a Critical control?] |
| Is control ownership clearly assigned to a named role?      | [Yes / No]           | [if No: who currently performs the control and is this documented?] |
| Is a documented procedure in place (SOP or policy section)? | [Yes / No]           | [reference the procedure document and version]          |
| Are the inputs and outputs of the control clearly defined?  | [Yes / No / Partial] | [can the tester identify what evidence the control should produce?] |
| Are compensating controls required due to design gaps?      | [Yes / No]           | [if Yes: describe the gap and recommended compensating control] |

**Overall Design Assessment:** [Effective / Partially Effective / Ineffective]

**Design Notes:**
[Summarise the design assessment. If Partially Effective or Ineffective, describe the specific design gap and its risk implication. Reference any prior design assessment for comparison.]

---

## Section 4: Operating Effectiveness Assessment

*Complete this section if Test Type includes "Operating Effectiveness." Record each sampled item in the table below. Add or remove rows as needed to match the sample size defined in Section 2. Provide enough detail in the "Evidence Found" column for a reviewer to verify the test result without returning to the raw evidence artefact.*

| Item # | Date / Reference     | Description                           | Expected Evidence                              | Evidence Found                                | Pass / Fail | Notes                                |
|--------|----------------------|---------------------------------------|------------------------------------------------|-----------------------------------------------|-------------|--------------------------------------|
| 1      | [YYYY-MM-DD / ref]   | [brief description of sampled item]   | [what evidence should exist to show control operated] | [what was actually found — be specific] | [Pass / Fail / N/A] | [any observation] |
| 2      | [YYYY-MM-DD / ref]   | [brief description of sampled item]   | [expected evidence]                            | [evidence found]                              | [Pass / Fail / N/A] | [observation]    |
| 3      | [YYYY-MM-DD / ref]   | [brief description of sampled item]   | [expected evidence]                            | [evidence found]                              | [Pass / Fail / N/A] | [observation]    |
| 4      | [YYYY-MM-DD / ref]   | [brief description of sampled item]   | [expected evidence]                            | [evidence found]                              | [Pass / Fail / N/A] | [observation]    |
| 5      | [YYYY-MM-DD / ref]   | [brief description of sampled item]   | [expected evidence]                            | [evidence found]                              | [Pass / Fail / N/A] | [observation]    |
| 6      | [YYYY-MM-DD / ref]   | [brief description of sampled item]   | [expected evidence]                            | [evidence found]                              | [Pass / Fail / N/A] | [observation]    |
| [...]  | [...]                | [add rows as needed]                  | [...]                                          | [...]                                         | [...]       | [...]            |

**Exception Summary:**
- Total items tested: [N]
- Items passed: [N]
- Items with exceptions: [N]
- Exception rate: [N of N = X%]

**Overall Operating Effectiveness Assessment:**
- **Effective** — exception rate 0% to 5% (0 to 1 exception in 25 items)
- **Partially Effective** — exception rate >5% to 20% (2 to 5 exceptions in 25 items)
- **Ineffective** — exception rate >20% (6+ exceptions in 25 items)

**Assessment:** [Effective / Partially Effective / Ineffective]

*Note on exception rate thresholds: thresholds above are based on a sample size of 25 for populations over 100. Adjust proportionally for smaller samples. For populations of 1–25, any exception is material and requires a finding.*

---

## Section 5: Evidence Collected

*List all evidence items collected during this control test. Each item should have a corresponding Evidence Record (TMPL-ER-001). Where evidence records have not been raised separately (e.g., for low-complexity tests), include sufficient detail in the Notes column for a reviewer to locate and assess the evidence.*

| Evidence ID       | Evidence Type                   | Date of Evidence | Storage Location / Path                         | Notes                                             |
|-------------------|---------------------------------|------------------|-------------------------------------------------|---------------------------------------------------|
| [ER-YYYY-NNNN]    | [Log / Screenshot / Report / etc.] | [YYYY-MM-DD] | [GRC platform reference or file path]           | [brief description of what this evidence shows]  |
| [ER-YYYY-NNNN]    | [Log / Screenshot / Report / etc.] | [YYYY-MM-DD] | [GRC platform reference or file path]           | [brief description]                               |
| [ER-YYYY-NNNN]    | [Log / Screenshot / Report / etc.] | [YYYY-MM-DD] | [GRC platform reference or file path]           | [brief description]                               |
| [ER-YYYY-NNNN]    | [Log / Screenshot / Report / etc.] | [YYYY-MM-DD] | [GRC platform reference or file path]           | [brief description]                               |

---

## Section 6: Finding

*Complete this section only if the control test resulted in an Ineffective or Partially Effective assessment. If the control passed fully, mark this section "N/A — No finding raised." If a finding is raised, it must also be recorded in the organisation's Finding Register and referenced in the Quarterly GRC Board Report.*

| Field             | Detail                                                                                     |
|-------------------|--------------------------------------------------------------------------------------------|
| Finding ID        | [FND-YYYY-NNNN — assigned by GRC team]                                                    |
| Finding Title     | [Descriptive title — e.g., "Quarterly Access Review Not Completed for 3 of 25 Sampled Accounts"] |
| Severity          | [Critical / High / Medium / Low — see Appendix: Finding Severity Matrix]                 |
| Root Cause        | [Select primary root cause: Design gap / Operational gap — control not followed / Resource gap — insufficient capacity to operate control / Technology gap — system does not support the control / Process gap — no procedure exists] |
| Finding Description | [Detailed narrative. Describe exactly what failed, in which items, over what period. Quote evidence where relevant. Do not conflate the finding with the recommendation — describe the problem objectively.] |
| Impact            | [What risk is elevated as a result of this finding? What could happen as a consequence of this control failure? Be specific — reference the threat scenario the control was designed to prevent.] |
| Repeat Finding?   | [Yes — previously identified as [FND-YYYY-NNNN] on [date] / No — first occurrence]        |
| Recommendation    | [Specific, actionable remediation steps. Include: what must change (policy, process, system, training, ownership); who should make the change; by when. Do not recommend vague improvements — each recommendation should be verifiable.] |

---

## Section 7: Management Response

*The control owner (or their delegate) must provide a formal response to any finding raised in Section 6. The response must be received within 10 business days of the finding being issued. GRC will chase overdue responses after 10 days and escalate to the ISO after 20 days.*

| Field                      | Detail                                                                                    |
|----------------------------|-------------------------------------------------------------------------------------------|
| Agreed?                    | [Yes — management agrees with the finding and recommendation / Partial — management agrees with the finding but proposes an alternative remediation / No — management disputes the finding (full rationale required)] |
| Management Response        | [Management's plan to address the finding. If "Partial" or "No," provide full rationale. If "No," the GRC Lead will escalate to the ISO for resolution.] |
| Proposed Remediation Steps | [Specific steps management will take]                                                    |
| Target Completion Date     | [YYYY-MM-DD]                                                                             |
| Interim Risk Treatment     | [What will management do to reduce risk while remediation is underway? If no interim treatment, state "None — management accepts interim risk." CISO approval required for that acceptance.] |
| Responder                  | [Full name, Role, Date]                                                                  |

---

## Section 8: Review and Approval

*All three roles must sign off before the Control Testing Record is finalised and lodged in the GRC platform.*

| Role                     | Name               | Role Title           | Date         | Sign-Off / Initial |
|--------------------------|--------------------|----------------------|--------------|--------------------|
| Tested By                | [Name]             | [e.g., GRC Analyst]  | [YYYY-MM-DD] | [Initial]          |
| Reviewed By              | [Name]             | [e.g., GRC Lead]     | [YYYY-MM-DD] | [Initial]          |
| Quality Reviewed By      | [Name]             | [e.g., ISO or CISO]  | [YYYY-MM-DD] | [Initial]          |

---

## Appendix: Finding Severity Matrix

*Use this matrix to assign the severity level to any finding raised in Section 6. Severity is based on the combination of risk impact and control criticality. Where two criteria apply, use the higher severity.*

| Severity | Criteria                                                                                                               | Required Remediation Timeline | Board Reporting Threshold |
|----------|------------------------------------------------------------------------------------------------------------------------|-------------------------------|---------------------------|
| Critical | (a) Immediate threat to confidentiality, integrity, or availability of Restricted or Confidential data; OR (b) Control failure on a Critical-rated control; OR (c) Finding indicates actual breach or regulatory violation | Immediate — within 7 days    | Yes — include in next board report and notify CISO immediately |
| High     | (a) Significant control failure with potential for material harm if not remediated; OR (b) Control failure on a High-rated control; OR (c) Repeat finding from a prior testing cycle | Within 30 days                | Yes — include in quarterly board report |
| Medium   | (a) Control weakness that increases risk but does not represent immediate material threat; OR (b) Exception rate between 5% and 20%; OR (c) Design gap without current evidence of exploitation | Within 90 days                | Report in aggregate in quarterly board report |
| Low      | (a) Minor gap or improvement opportunity; OR (b) Single exception in a large sample with no pattern; OR (c) Documentation deficiency with no operational impact | Within 180 days or next scheduled review | Report in aggregate; not individually named in board report |

*Finding severity may be escalated at the discretion of the ISO or CISO based on context, threat intelligence, or regulatory environment.*

---

*End of Template TMPL-CR-001 v1.0. Remove all guidance text (italicised instructions) before distributing a completed Control Testing Record. Completed records must be stored in the GRC platform and referenced in the Control Register.*

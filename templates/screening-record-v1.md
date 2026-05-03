# Vendor / Personnel Screening Record — Template

---

## Template Metadata

| Field               | Value                                                                                        |
|---------------------|----------------------------------------------------------------------------------------------|
| Template ID         | TMPL-SR-001                                                                                  |
| Version             | 1.0                                                                                          |
| Status              | Active                                                                                       |
| Purpose             | Document screening outcomes for vendors and personnel in trusted or sensitive roles          |
| Owner               | Vendor Risk Manager / Human Resources                                                        |
| Approved By         | ISO / CISO                                                                                   |
| Review Frequency    | Annual                                                                                       |
| GitHub Reference    | https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/templates/screening-record-v1.md |

---

## Instructions for Use

**Two use cases for this template**

This template serves two distinct but structurally similar screening purposes. Complete the correct sections for each use case:

1. **Vendor Security Screening** — used when onboarding a new vendor, conducting a periodic vendor review, or responding to a material change in a vendor's circumstances (e.g., change of ownership, security incident, regulatory sanction). The Vendor Risk Manager owns vendor screening records. Complete Sections 1, 2 (vendor checklist), 3, 4, and 5.

2. **Personnel Background Screening** — used when engaging an individual in a role classified as High Sensitivity (e.g., privileged system access, access to restricted data, financial authority, executive role) or when periodic re-screening is triggered. Human Resources owns personnel screening records, in coordination with the ISO. Complete Sections 1, 2 (personnel checklist), 3, 4, and the Privacy Notice.

**When to use**
- **New engagement** — before any system access, data access, or service commencement is granted.
- **Periodic review** — per the frequency defined in the Appendix. Periodic reviews must be completed and approved before the previous screening period expires.
- **Material change** — following a significant event affecting the subject (e.g., vendor security incident, change in sub-processors, key personnel change at a Critical-tier vendor; or change in an individual's role, personal circumstances triggering re-screening under policy).
- **Trigger event** — following a security alert, regulatory notification, or adverse media report relating to the subject.

**Who retains records**
Vendor screening records are retained by the Vendor Risk Manager and stored in the GRC platform. Personnel screening records are retained by Human Resources in a separate, access-restricted repository. Personnel screening records must not be stored in the general GRC platform or accessible to staff outside HR, Legal, and the ISO. Access to personnel screening records is on a strict need-to-know basis.

**Privacy considerations for personnel screening**
The collection and processing of background screening data about individuals is subject to applicable data protection law. Before initiating personnel screening, ensure: (a) the legal basis for processing has been identified; (b) the individual has received the applicable privacy notice (see Section 7 of this template); (c) screening checks are limited to those that are proportionate to the role and legally permissible in the applicable jurisdiction; (d) results are handled by designated HR personnel only and not shared outside the defined approval chain. Criminal record check results must be handled per the organisation's Sensitive Data Handling Procedure.

**Numbering convention**
Screening IDs follow the format SR-YYYY-NNNN (e.g., SR-2025-0017). Assigned sequentially by the Vendor Risk Manager (vendor) or HR (personnel).

---

## Section 1: Subject Identification

| Field                      | Detail                                                                                          |
|----------------------------|-------------------------------------------------------------------------------------------------|
| Screening ID               | [SR-YYYY-NNNN]                                                                                  |
| Subject Type               | [Vendor / Individual]                                                                           |
| Subject Name               | [Legal entity name (vendor) or individual's full legal name (personnel) — see privacy note for individual records] |
| Subject Classification     | **Vendor:** [Risk Tier: Critical / High / Medium / Low — per Third-Party Risk Management Policy] **OR** **Personnel:** [Role Sensitivity: High / Standard] |
| Screening Date             | [YYYY-MM-DD — date screening was initiated]                                                    |
| Screened By                | [Full name, Role — e.g., Alex Reid, Vendor Risk Manager]                                       |
| Screening Reason           | [New engagement / Periodic review / Material change / Trigger event]                           |
| Previous Screening ID      | [SR-YYYY-NNNN, or "N/A — first screening"]                                                     |
| Previous Screening Date    | [YYYY-MM-DD, or N/A]                                                                           |

---

## Section 2: Screening Scope

*Complete the appropriate checklist below based on the Subject Type. Mark each check as Required (Y/N — based on subject classification and role), Completed (Y/N), and record the outcome. Not all checks apply to all subjects — use the Appendix to determine which checks are required for a given tier or role sensitivity level. Where a check is not required, mark as "N/A" with a brief rationale.*

### 2A: Vendor Screening Checks

| Screening Check                   | Required? | Completed? | Outcome                          | Notes / Evidence Reference                          |
|-----------------------------------|-----------|------------|----------------------------------|-----------------------------------------------------|
| Information Security Assessment   | [Y/N/N/A] | [Y/N]      | [Pass / Pass with conditions / Fail / Pending] | [brief description of assessment and findings] |
| Financial Stability Check         | [Y/N/N/A] | [Y/N]      | [Pass / Pass with conditions / Fail / Pending] | [source used — e.g., credit agency report, Companies House, audited accounts] |
| Regulatory and Sanction List Check | [Y/N/N/A] | [Y/N]     | [Pass / No adverse findings / Adverse finding — detail in notes] | [lists checked — e.g., OFAC, HM Treasury, UN] |
| Previous Incident History         | [Y/N/N/A] | [Y/N]      | [No known incidents / Known incident — see notes] | [source: public disclosure, vendor self-declaration, threat intelligence] |
| Sub-contractor / Sub-processor Security | [Y/N/N/A] | [Y/N] | [Adequate / Gaps identified / Not disclosed] | [sub-processors identified; assessed against same framework?] |
| Data Processing Terms (DPA / GDPR Article 28 [VERIFY]) | [Y/N/N/A] | [Y/N] | [Executed / Pending / Not Required] | [DPA reference number and execution date, or explanation] |
| Insurance Verification            | [Y/N/N/A] | [Y/N]      | [Adequate / Gaps / Not provided]  | [minimum coverage levels required; actual coverage confirmed]  |
| BCP / DR Capability               | [Y/N/N/A] | [Y/N]      | [Adequate / Not assessed / Gaps] | [basis of assessment — e.g., BCP questionnaire, site visit, BCP document review] |
| AI-Specific Due Diligence         | [Y/N/N/A — required for AI vendors] | [Y/N] | [Pass / Conditions / Fail] | [complete if vendor provides AI systems or processes data through AI — reference AI Vendor Due Diligence Addendum] |

### 2B: Personnel Screening Checks

| Screening Check                                      | Required? | Completed? | Outcome                           | Notes                                               |
|------------------------------------------------------|-----------|------------|-----------------------------------|-----------------------------------------------------|
| Identity Verification (government-issued photo ID)   | [Y/N/N/A] | [Y/N]      | [Verified / Not verified]         | [document type and reference — do not record full ID number in this record] |
| Right to Work / Eligibility Verification             | [Y/N/N/A] | [Y/N]      | [Confirmed / Not confirmed]       | [statutory basis; expiry date of right to work if applicable] |
| Criminal Record Check                                | [Y/N/N/A] | [Y/N]      | [No relevant convictions / Relevant disclosure — HR decision required] | [standard or enhanced; jurisdiction; provider; reference] |
| Employment History Verification (minimum 5 years)   | [Y/N/N/A] | [Y/N]      | [Verified / Gaps identified]      | [period covered; any unexplained gaps?]             |
| Reference Checks (minimum 2 professional references) | [Y/N/N/A] | [Y/N]      | [Satisfactory / Concerns raised]  | [references contacted; summary of outcomes]        |
| Credit Check (financially sensitive roles only)      | [Y/N/N/A] | [Y/N]      | [Satisfactory / Concerns raised / Adverse finding] | [required legal basis; result summary — do not record credit score in detail] |
| Regulatory Fitness Check (if regulated role)         | [Y/N/N/A] | [Y/N]      | [Confirmed / Not applicable / Adverse] | [e.g., FCA register check; professional body membership] |
| Conflict of Interest Declaration                     | [Y/N/N/A] | [Y/N]      | [No conflict declared / Conflict declared — see HR record] | [declaration form reference] |

---

## Section 3: Screening Outcome

| Field                   | Detail                                                                                         |
|-------------------------|------------------------------------------------------------------------------------------------|
| Overall Outcome         | [Approved / Approved with Conditions / Deferred / Rejected]                                   |
| Risk Rating             | [Critical / High / Medium / Low]                                                               |
| Conditions (if any)     | [List each condition with a target date and responsible owner. Conditions must be resolved within the agreed timeframe or the approval lapses.] |
| Outcome Rationale       | [Brief narrative explaining the basis for the overall outcome. Reference specific checks and their results. For "Approved with Conditions" and "Rejected," include sufficient detail to support an audit trail.] |

*Where the outcome is "Rejected," the subject must be notified in a manner consistent with applicable law and organisational policy. For vendor rejections, the Vendor Risk Manager coordinates the notification. For personnel rejections, HR coordinates notification in consultation with Legal.*

*Where the outcome is "Deferred," record the specific condition(s) that must be resolved before screening can be completed and the target resolution date.*

---

## Section 4: Approval

| Field                   | Detail                                                                                         |
|-------------------------|------------------------------------------------------------------------------------------------|
| Reviewed By             | [Full name, Role, Date — first-line review, e.g., Vendor Risk Manager or HR Business Partner] |
| Approved By             | [Full name, Role, Date — final approval authority — for Critical/High vendors: CISO or ISO; for High Sensitivity personnel: ISO with HR sign-off] |
| Approval Conditions     | [Restate any conditions attached to the approval that must be tracked to closure]              |
| Next Screening Due      | [YYYY-MM-DD — calculated from the Appendix frequency table]                                   |
| Ongoing Monitoring Required | [Yes / No — if Yes, complete Section 5]                                                   |

---

## Section 5: Ongoing Monitoring (Vendors Only)

*Complete this section for all Critical and High-tier vendors. For Medium-tier vendors, complete where continuous monitoring tooling is available. Low-tier vendors are not typically subject to ongoing automated monitoring.*

| Field                           | Detail                                                                                    |
|---------------------------------|-------------------------------------------------------------------------------------------|
| Continuous Monitoring Tool      | [e.g., SecurityScorecard / BitSight / Recorded Future / UpGuard — specify tool name and version] |
| Current Score / Rating          | [Numerical score and/or letter grade as at screening date]                               |
| Score as of Previous Review     | [Score at time of last periodic screening, for trend comparison]                         |
| Alert Threshold                 | [Define the score or event that would trigger an out-of-cycle re-screening or escalation — e.g., "Score drops below 70 / Grade falls to C or below"] |
| Monitoring Frequency            | [Continuous automated / Weekly digest / Monthly review]                                  |
| Monitoring Owner                | [Role — e.g., Vendor Risk Manager]                                                       |
| Active Alerts at Time of Review | [None / List active alerts with brief description and status]                            |

---

## Section 6: Privacy Notice (Personnel Screening Only)

*This section must be completed and provided to the individual before any background screening checks are initiated. The signed acknowledgement must be retained by HR.*

**Data Controller:** [Organisation legal name]
**Purpose of processing:** To verify the identity, eligibility, professional history, and fitness for employment of individuals in designated sensitive roles, as required by the organisation's Personnel Screening Policy and applicable legal obligations.
**Legal basis:** [e.g., Legitimate interests (security and integrity of information assets) / Legal obligation (right to work verification) / Consent (criminal record check where required by law) — specify the basis for each check type and jurisdiction] [VERIFY applicable legal basis with Legal Counsel before use]
**Data collected:** Identity documents, employment history, professional references, criminal record (where applicable), credit history (where applicable), regulatory status (where applicable).
**Recipients:** Processed by [screening provider name if external]. Results shared only with HR, the appointing manager (outcome only, not detail), the ISO, and Legal Counsel where required.
**Retention period:** Screening records are retained for [state period — e.g., duration of employment plus 7 years] in accordance with the Data Retention Policy, except where a shorter or longer period is required by applicable law.
**Your rights:** You have the right to access, correct, and in certain circumstances request erasure of your personal data. You also have the right to lodge a complaint with the applicable supervisory authority. Contact [privacy@organisation.com] to exercise your rights.
**Automated decisions:** Screening results are not subject to automated decision-making. All screening outcomes are reviewed and determined by a qualified HR professional.

*Individual's acknowledgement:*
By signing below, I confirm that I have received and read this privacy notice and I consent to the processing of my personal data as described above for the purposes of background screening.

| Name               | Signature | Date         |
|--------------------|-----------|--------------|
| [Individual name]  | _________ | [YYYY-MM-DD] |

---

## Appendix: Screening Frequency by Role or Vendor Tier

| Subject Type  | Classification           | Screening Checks Required                                   | Initial Screening | Periodic Review Frequency |
|---------------|--------------------------|-------------------------------------------------------------|-------------------|---------------------------|
| Vendor        | Critical                 | All checks in Section 2A including AI addendum if applicable | Before contract execution | Annual |
| Vendor        | High                     | All checks except AI addendum (unless AI vendor)            | Before contract execution | Annual |
| Vendor        | Medium                   | InfoSec assessment, DPA if applicable, sanctions check       | Before contract execution | Every 2 years |
| Vendor        | Low                      | Sanctions check, basic InfoSec questionnaire                | Before contract execution | Every 3 years or on material change |
| Individual    | High Sensitivity          | All checks in Section 2B applicable to role                 | Before access granted | Every 3 years or on material change |
| Individual    | Standard                 | Identity verification, right to work, employment history (3 years), 1 reference | Before start date | On material change only |
| Contractor    | Any (system access)      | Identity verification, right to work, conflict of interest, professional insurance | Before access granted | On contract renewal |

*Screening frequency may be increased at the discretion of the ISO or CISO based on risk profile, threat intelligence, or regulatory requirements.*

---

*End of Template TMPL-SR-001 v1.0. Remove all guidance text before distributing a completed Screening Record. Personnel records must be stored separately from vendor records per the access restriction requirements in the Instructions.*

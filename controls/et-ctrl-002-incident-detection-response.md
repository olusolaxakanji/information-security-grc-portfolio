# ET-CTRL-002: Incident Detection and Response

| Field | Value |
|---|---|
| Control ID | ET-CTRL-002 |
| Title | Incident Detection and Response |
| Entity | Emyzer Technology |
| Regulatory citation | [ISO 27001:2022](https://www.iso.org/standard/27001.html) A.5.24 (IR planning and preparation), A.5.25 (Assessment of information security events), A.5.26 (Response to information security incidents), A.5.27 (Learning from incidents); [NIST SP 800-61 Rev. 2](https://csrc.nist.gov/pubs/sp/800/61/r2/final) Section 3 (Handling an Incident); [GDPR](https://gdpr.eu/article-33-notification-of-a-personal-data-breach/) Art. 33 (72-hour supervisory authority notification), Art. 34 (Communication to data subjects) |
| Control owner | Information Security Officer (Susan Orwell) |
| Control type | Corrective / Detective |
| Testing frequency | Per incident; Annual tabletop exercise |
| Last tested | [DATE] |
| Test result | [Pass / Fail / Exception noted] |
| Evidence reference | `evidence/[YEAR]/ET-CTRL-002/` |
| Status | Active |

---

## Control Description

The Incident Response Team (IRT), led by the ISO, manages all security incidents from detection through post-incident review in accordance with the Incident Management Policy (KB-PORTFOLIO-0005).

**Incident lifecycle:**

1. **Detection**: Security events are surfaced via SIEM alerts, user reports, third-party notifications, or automated monitoring tools.
2. **Classification**: The IRT classifies the incident within 1 hour of detection using the four-tier severity model (Critical, High, Medium, Low) defined in the Incident Management Policy.
3. **Containment**: Immediate containment actions are taken to limit impact. Containment completion timeframes are severity-dependent.
4. **Eradication and recovery**: Root cause is removed and affected systems are returned to an operational state, with sign-off from business owners before production restoration.
5. **Post-incident review**: A formal post-incident review is completed for all Medium or higher severity incidents. Findings are documented and remediation actions are tracked in ServiceNow to closure.

**GDPR notification:** Personal data breaches meeting the Article 33 threshold are reported to the relevant supervisory authority within 72 hours of detection. Article 34 notifications to affected individuals are issued when required. Legal Counsel is notified at the point of incident classification as High or Critical. All notification decisions and timelines are documented.

**Annual tabletop exercise:** Tests the IRT's response capability against a realistic simulated scenario and informs plan updates.

## Test Procedure

1. Pull all incident tickets from ServiceNow for the review period. Confirm each was opened and classified within the 1-hour detection-to-classification window.
2. For Critical and High severity incidents: confirm containment actions were completed within the policy-required timeframe and escalation to the CISO was documented.
3. For all Medium and above incidents: confirm a post-incident review was completed, findings are documented, and remediation actions have assigned owners and target closure dates.
4. For any incident involving personal data: confirm that GDPR Article 33/34 notification obligations were formally assessed, the assessment was documented, and where triggered, notifications were filed within 72 hours.
5. For the annual tabletop exercise: confirm the exercise was conducted, a results report was produced, the scenario was realistic (e.g., ransomware, insider threat, supply chain compromise), and any plan updates were incorporated.
6. File all incident reports, post-incident reviews, notification records, and exercise reports in `evidence/[YEAR]/ET-CTRL-002/`.

## Escalation

Critical severity incidents are escalated to the CISO within 1 hour of classification and to the Security Steering Committee within 4 hours. Legal Counsel is notified for any incident with personal data exposure or a plausible regulatory notification obligation. All escalation actions and timestamps are documented in the ServiceNow incident record.

## Change History

| Version | Date | Changed by | Summary of change |
|---|---|---|---|
| 1.0 | 2026-01-13 | Information Security Officer | Initial version |

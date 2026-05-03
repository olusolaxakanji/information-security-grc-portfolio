# ET-CTRL-006 — Security Awareness Training Completion

| Field | Value |
|---|---|
| Control ID | ET-CTRL-006 |
| Title | Security Awareness Training Completion |
| Entity | Emyzer Technology |
| Regulatory citation | [ISO 27001:2022](https://www.iso.org/standard/27001.html) A.6.3 (Information security awareness, education and training); [NIST SP 800-50 Rev. 1](https://csrc.nist.gov/pubs/sp/800/50/r1/final) [VERIFY — confirm Rev. 1 finalization status; original SP 800-50 published 2003, draft Rev. 1 circulated 2022–2023]; [NIST CSF 2.0](https://www.nist.gov/cyberframework) PR.AT-1 (Users are informed and trained), PR.AT-2 (Privileged users understand their responsibilities) |
| Control owner | Information Security Officer (Susan Orwell) |
| Control type | Preventive |
| Testing frequency | Monthly (phishing simulations); Annual (core training completion) |
| Last tested | [DATE] |
| Test result | [Pass / Fail / Exception noted] |
| Evidence reference | `evidence/[YEAR]/ET-CTRL-006/` |
| Status | Active |

---

## Control Description

The ISO, with support from HR, operates a continuous security awareness programme covering all employees, contractors, and third parties with access to Emyzer Technology systems.

**Annual core training:** All in-scope personnel must complete the annual security awareness course in the Learning Management System (LMS). Completion is a condition of continued system access. Topics include: data classification and handling, password hygiene and MFA, phishing recognition, acceptable use obligations, incident reporting procedure, and AI tool usage rules under the Acceptable Use Policy. Completion deadlines: within 30 days of hire for new starters; by 31 January each year for annual renewal.

**Role-based training:** Personnel in privileged roles — IT administrators, finance, HR, legal — complete additional modules covering topics relevant to their access level and data handling responsibilities. Completion deadline matches the core training annual cycle.

**Monthly phishing simulations:** Simulated campaigns are delivered to all in-scope staff monthly using a rotating template library covering current threat types (credential harvesting, invoice fraud, impersonation, AI-generated lures). Click and credential-submission rates are tracked by department. Individuals who click in three or more consecutive simulations receive mandatory remedial training within 5 business days.

**Programme effectiveness review:** The ISO compiles aggregate completion rates and phishing simulation trend data quarterly and reports results to the Security Steering Committee.

## Test Procedure

1. Pull the LMS completion report for the review period. Confirm that all active employees, contractors, and third-party users met the applicable completion deadline (30-day new-hire window or 31 January annual deadline).
2. Identify any individuals who did not complete training and confirm that system access was suspended until completion — or that a CISO-approved exception is on file.
3. Pull the monthly phishing simulation results for the period. Review click rates and credential-submission rates by department. Compare against the prior quarter's baseline.
4. For each month in the period, confirm that individuals who clicked in three consecutive simulations received remedial training within the 5-business-day window.
5. Confirm that role-based training completion rates for all privileged-access roles reached 100% before the annual deadline.
6. Confirm that the quarterly effectiveness report was produced and submitted to the Security Steering Committee.
7. File the LMS completion report, phishing simulation results, remedial training records, and effectiveness report in `evidence/[YEAR]/ET-CTRL-006/`.

## Escalation

Departments with core training completion below 90% at the annual deadline are escalated to the relevant Department Head by the ISO, with a 10-business-day cure period. Persistent non-compliance beyond that window is escalated to the CISO for executive intervention and potential access suspension. A department-level phishing click rate exceeding 20% in two consecutive months triggers a mandatory departmental security awareness session.

## Change History

| Version | Date | Changed by | Summary of change |
|---|---|---|---|
| 1.0 | 2026-01-13 | Information Security Officer | Initial version |

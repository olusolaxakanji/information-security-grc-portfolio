# ET-CTRL-001: Access Control Review and Certification

| Field | Value |
|---|---|
| Control ID | ET-CTRL-001 |
| Title | Access Control Review and Certification |
| Entity | Emyzer Technology |
| Regulatory citation | [ISO 27001:2022](https://www.iso.org/standard/27001.html) A.5.15 (Access control), A.5.16 (Identity management), A.5.18 (Access rights); [NIST SP 800-53 Rev. 5](https://csrc.nist.gov/pubs/sp/800/53/r5/upd1/final) AC-2 (Account Management), AC-3 (Access Enforcement), AC-6 (Least Privilege) |
| Control owner | Information Security Officer (Susan Orwell) |
| Control type | Detective |
| Testing frequency | Quarterly (standard users); Monthly (privileged users) |
| Last tested | [DATE] |
| Test result | [Pass / Fail / Exception noted] |
| Evidence reference | `evidence/[YEAR]/ET-CTRL-001/` |
| Status | Active |

---

## Control Description

The Information Security Officer conducts periodic certifications of user access rights to verify that access granted to information systems, applications, and data remains appropriate to each user's current role and documented business need.

**Standard user certification (quarterly):** Department managers review and attest to the appropriateness of every active account within their area of responsibility. Accounts lacking a current business justification are flagged for revocation within 30 days of the review completion date.

**Privileged access certification (monthly):** The ISO reviews all privileged accounts, including administrator, service, and break-glass accounts, against documented business justifications. Privileged access without current written justification is revoked within 15 days.

Access review records are maintained in ServiceNow and retained for 3 years. The identity management system is the system of record for account state; ServiceNow holds the governance record.

## Test Procedure

1. Extract a full active account report from the identity management system for the review period, segmented by account type (standard, privileged, service, break-glass).
2. For standard accounts: confirm that each department manager completed their quarterly attestation and documented an approval or revocation decision for every account in scope.
3. For privileged accounts: confirm the ISO completed the monthly review, every account has current written justification on file, and any accounts flagged in the prior month were remediated within the 15-day window.
4. Verify that accounts for terminated employees were revoked on the same business day as termination, and transferred employees' access was adjusted within 24 hours of the role change.
5. Check for dormant accounts (inactive >90 days) and confirm automated disablement executed correctly for the period.
6. Document all findings, exceptions, and remediation status in the evidence record and file in `evidence/[YEAR]/ET-CTRL-001/`.

## Escalation

Access review failures, including overdue certifications, unrevoked terminated-employee accounts, or unjustified privileged access, are escalated to the CISO within 24 hours of discovery. The ISO opens a remediation ticket in ServiceNow with a mandatory closure deadline. Systemic failures (two or more consecutive quarters of incomplete certifications in the same department) are escalated to the Security Steering Committee.

## Change History

| Version | Date | Changed by | Summary of change |
|---|---|---|---|
| 1.0 | 2026-01-13 | Information Security Officer | Initial version |

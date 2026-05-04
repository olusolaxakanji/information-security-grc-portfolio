# Quarterly User Access Review: Attestation Record

**Emyzer Nexus / Emyzer Technology: Q1 2025**

---

## Document Metadata

| Field | Detail |
|---|---|
| **Document ID** | OPR-AR-2025-001 |
| **Document Title** | Quarterly User Access Review: Attestation Record Q1 2025 |
| **Review Period** | 1 January 2025 – 31 March 2025 |
| **Review Completion Date** | 2025-03-28 |
| **Owner** | Information Security Officer (Susan Orwell) |
| **Prepared By** | GRC Analyst (J. Mirren) in collaboration with System Owners |
| **Reviewed By** | CISO |
| **Approved / Attested By** | See Section 7: Attestation Sign-offs |
| **Classification** | Internal: Restricted |
| **Version** | 1.0 |
| **Governing Control** | [ET-CTRL-001: Access Control Review](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/controls/et-ctrl-001-access-control-review.md) |
| **Governing Policy** | [Access Control Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/access-control-policy.md) |
| **Framework Alignment** | [ISO 27001:2022](https://www.iso.org/standard/82875.html) A.8.2; [NIST CSF 2.0](https://www.nist.gov/cyberframework) PR.AC-1, PR.AC-4; [ISO/IEC 27002:2022](https://www.iso.org/standard/75652.html) 8.2 |

> **Simulated Environment.** This record was developed as part of a fictional GRC portfolio for professional demonstration purposes. All personnel names, system access counts, and exception details are invented. Framework references are accurate as of the document date.

---

## 1. Purpose and Scope

This attestation record documents the completion of the Q1 2025 Quarterly User Access Review conducted under ET-CTRL-001. It constitutes audit evidence that Emyzer Nexus and Emyzer Technology access privileges across in-scope systems were reviewed, confirmed, and remediated where necessary within the review period.

**Control objective:** Ensure that user access rights remain appropriate, are granted on a least-privilege basis [VERIFY: ISO 27001:2022 A.8.2], and that accounts belonging to departed employees, transferred staff, and role-changed individuals are promptly modified or revoked.

### 1.1 Systems in Scope

| System | System Owner | User Population | Review Method |
|---|---|---|---|
| AWS Production Environment (Emyzer Technology tenancy) | CTO | IAM users and role assignments | IAM Access Analyzer export + manual review |
| GitHub Enterprise (information-security-grc-portfolio org) | ISO | Repository contributors and admin roles | GitHub audit log export |
| ServiceNow GRC Platform | GRC Lead | GRC platform users (submitters, approvers, viewers) | Platform user report export |
| Google Workspace (corporate email and collaboration) | IT Manager | All corporate accounts | Admin Console export |
| Learning Management System (LMS) | HR Director | All active accounts + completion records | LMS admin report |
| AWS Veridian AI tenancy (post-acquisition, now merged) | CTO | Legacy Veridian AI IAM accounts | IAM export; reconciled against Emyzer Nexus HR records |
| PCM-001 Application Access (Predictive Churn Model dashboard) | VP, Customer Success | Designated CS operators | Application access log |
| CRT-001 Application Access (AI-Assisted Contract Review Tool) | General Counsel | Designated Legal operators | Application access log |

### 1.2 Out of Scope

- Privileged Infrastructure access (reviewed separately under a semi-annual privilege access review cadence per the Access Control Policy)
- Third-party vendor system access (reviewed under the Third-Party Risk Management Programme)
- Physical access systems (reviewed by Facilities Management separately)

---

## 2. Methodology

### 2.1 Review Process

1. **Data extraction** (2025-03-10 to 2025-03-14): GRC Analyst extracted current user lists from each in-scope system. HR Operations provided the authoritative employee list as of 2025-03-07, including joiners, movers, and leavers in Q1 2025.

2. **Reconciliation** (2025-03-14 to 2025-03-18): Extracted user lists were reconciled against the HR record. Accounts belonging to departed employees, contractors whose engagements ended, or staff who changed roles in the period were flagged for review.

3. **System owner review** (2025-03-18 to 2025-03-25): System owners received a pre-populated review worksheet for their system. They were required to confirm, escalate, or mark for remediation each account within 5 business days.

4. **Exception handling** (2025-03-25 to 2025-03-27): Confirmed exceptions were logged in the GRC platform and assigned to system owners for remediation. Critical exceptions (active credentials for departed employees) were escalated for immediate action.

5. **Attestation** (2025-03-28): System owners and the ISO signed attestation statements confirming review completion and exception disposition.

### 2.2 Access Classification Applied

| Access Level | Definition |
|---|---|
| **Appropriate: No Action** | Account exists; user is active; access rights are commensurate with current role; no change required |
| **Appropriate: Modified** | Account confirmed appropriate after correction (access reduced, permissions adjusted) during the review cycle |
| **Exception: Remediated** | Access was inappropriate; remediation action completed within the review period |
| **Exception: Open** | Access was inappropriate; remediation in progress; scheduled completion date recorded |

---

## 3. Review Results Summary

| System | Accounts Reviewed | Appropriate: No Action | Appropriate: Modified | Exception: Remediated | Exception: Open | Exception Rate |
|---|---|---|---|---|---|---|
| AWS Production (ET tenancy) | 34 | 29 | 3 | 2 | 0 | 5.9% |
| GitHub Enterprise | 12 | 11 | 1 | 0 | 0 | 0.0% |
| ServiceNow GRC Platform | 18 | 17 | 1 | 0 | 0 | 0.0% |
| Google Workspace | 87 | 80 | 5 | 1 | 1 | 2.3% |
| Learning Management System | 91 | 88 | 3 | 0 | 0 | 0.0% |
| AWS Veridian AI tenancy | 22 | 14 | 4 | 3 | 1 | 18.2% |
| PCM-001 Application | 23 | 23 | 0 | 0 | 0 | 0.0% |
| CRT-001 Application | 8 | 8 | 0 | 0 | 0 | 0.0% |
| **TOTAL** | **295** | **270** | **17** | **6** | **2** | **2.7%** |

**Overall exception rate: 2.7%** (8 exceptions from 295 accounts reviewed; 6 remediated within review period, 2 open with scheduled remediation dates).

**Elevated exception rate: AWS Veridian AI tenancy (18.2%).** This reflects the post-acquisition integration period: Veridian AI accounts were reconciled against Emyzer Nexus HR records for the first time this quarter. See Section 5 for exception detail.

---

## 4. Material Access Changes in Q1 2025

The following material changes to access were made outside the scheduled review cycle and are documented here for completeness:

| Date | Change Type | System | Description | Authorised By |
|---|---|---|---|---|
| 2025-01-10 | Access granted | PCM-001, CRT-001 | 8 Veridian AI legacy staff granted operator access following completion of mandatory AI governance training | VP, Customer Success / General Counsel |
| 2025-01-15 | Access restricted | CRT-001 | CRT-001 use restricted to contracts containing no personal data pending DPA execution; use restriction enforced via Legal team policy and training (no technical enforcement currently in place: gap noted) | General Counsel / CISO |
| 2025-02-01 | Access revoked | AWS Production (ET tenancy) | 3 Veridian AI IT contractors' access revoked following contract end | CTO / HR |
| 2025-02-14 | Role change | ServiceNow GRC Platform | 1 staff member promoted from GRC Analyst to GRC Lead; platform permissions updated to approver role | GRC Team / ISO |
| 2025-03-01 | New joiner | Google Workspace, LMS | 4 new starters onboarded; access provisioned per role-based access matrix | IT Manager / HR |

---

## 5. Exception Register

### Exception Detail

| Exception ID | System | Account / Role | Issue | Risk Level | Action Taken | Status | Resolved By | Resolution Date |
|---|---|---|---|---|---|---|---|---|
| AR-EXC-2025-001 | AWS Production (ET) | `svc-legacy-backup` service account | Service account with S3 write permissions no longer associated with an active service: orphaned credential | **High** | Account suspended pending investigation; CTO to confirm whether account can be deleted or requires reassignment | Remediated | CTO | 2025-03-20 |
| AR-EXC-2025-002 | AWS Production (ET) | IAM user `d.marsh` | Employee D. Marsh departed 2025-01-31; IAM account not disabled within the 24-hour SLA defined in the Access Control Policy | **High** | Account disabled immediately on identification; access logs reviewed (no post-departure logins detected) | Remediated | IT Manager | 2025-03-15 |
| AR-EXC-2025-003 | Google Workspace | `c.okafor@emyzer.com` | Employee transferred to a new team 2025-02-10; retained edit access to sensitive financial folders in Google Drive from previous role | **Medium** | Drive folder permissions removed; no evidence of misuse in access logs | Remediated | IT Manager | 2025-03-19 |
| AR-EXC-2025-004 | Google Workspace | `admin-shared@emyzer.com` | Shared admin account used by 3 IT staff; cannot be attributed to a named individual: violates non-repudiation requirement [VERIFY: ISO 27001:2022 A.8.2] | **Medium** | Account flagged for retirement; individual admin accounts to be created; target retirement date 2025-06-30 | **Open** | IT Manager | Target: 2025-06-30 |
| AR-EXC-2025-005 | AWS Veridian AI | `v.chen` IAM user | Veridian AI engineer V. Chen departed pre-acquisition; account not included in Emyzer Nexus HR record; discovered through IAM export reconciliation | **Critical** | Account disabled immediately; access logs reviewed: no post-acquisition logins detected; identity verified as departed employee | Remediated | CTO | 2025-03-16 |
| AR-EXC-2025-006 | AWS Veridian AI | `v.patel`, `v.rodriguez` IAM users | Two accounts with elevated IAM permissions (PowerUser policy); roles not consistent with current job functions; overprivileged from pre-acquisition configuration | **High** | Permissions reduced to minimum required for current roles; account owners notified and acknowledged | Remediated | CTO | 2025-03-22 |
| AR-EXC-2025-007 | AWS Veridian AI | Root account MFA | AWS root account MFA not enabled; inherited configuration from Veridian AI's unmanaged AWS environment | **Critical** | MFA enabled immediately; root account usage restricted to break-glass procedure; process documented | Remediated | CTO | 2025-03-14 |
| AR-EXC-2025-008 | AWS Veridian AI | `dev-test-key` API key | Long-lived API key with broad permissions; last used pre-acquisition; no current owner identified | **High** | Key revoked; GRC incident raised to investigate whether key had been exposed; no evidence of unauthorised use | Remediated | CTO | 2025-03-18 |

**Note:** AR-EXC-2025-004 is the only open exception at attestation date (2025-03-28). Remediation target is 2025-06-30. This exception will be confirmed resolved in the Q2 2025 access review.

### Exception Analysis

Two Critical-rated exceptions were identified in the AWS Veridian AI tenancy (AR-EXC-2025-005 and AR-EXC-2025-007). Both were identified through the post-acquisition reconciliation process: they reflect the unmanaged state of Veridian AI's AWS environment prior to acquisition. Both were remediated within the review period.

The elevated exception rate in the Veridian AI tenancy (18.2%) is consistent with the integration context and is expected to normalise by Q2 2025 as the tenancy is fully brought under Emyzer Nexus IAM governance standards.

---

## 6. Observations and Improvement Actions

| Observation | Priority | Action | Owner | Target Date |
|---|---|---|---|---|
| The 24-hour leaver access revocation SLA was missed in one case (AR-EXC-2025-002). Leaver process is currently a manual HR-to-IT email notification. | **High** | Implement ServiceNow-triggered automated access suspension workflow for leavers; eliminates manual handoff. GRC to raise change request. | IT Manager / GRC Lead | 2025-06-30 |
| Shared admin account (AR-EXC-2025-004) cannot be attributed to a named individual: a non-repudiation gap. | **Medium** | Retire shared account; provision individual admin accounts with appropriately scoped permissions. | IT Manager | 2025-06-30 |
| CRT-001 use restriction (no PII contracts) has no technical enforcement; relies on operator compliance. | **High** | CTO to assess technical DLP controls preventing PII-containing contracts from being submitted to CRT-001 pipeline pending DPA execution. | CTO | 2025-09-30 |
| Veridian AI tenancy root account was unmanaged; MFA not enabled. Break-glass procedure not documented until this review. | **Medium** | Document break-glass procedure formally; add to CISO emergency runbook; schedule 6-monthly root account credential rotation reminder. | CISO | 2025-06-30 |

---

## 7. Attestation Sign-offs

By signing below, each System Owner attests that they have reviewed the access lists for their system(s) and that:

1. All accounts listed as **Appropriate: No Action** have been confirmed as belonging to active individuals with access rights commensurate with their current role
2. All accounts listed as **Appropriate: Modified** have been corrected and the corrected access is appropriate
3. All exceptions listed as **Remediated** have been resolved as described
4. All exceptions listed as **Open** have a documented remediation timeline they are committed to meeting

| System | System Owner | Signature | Attestation Date |
|---|---|---|---|
| AWS Production (ET tenancy) | CTO | *[signed]* | 2025-03-28 |
| GitHub Enterprise | ISO | *[signed]* | 2025-03-27 |
| ServiceNow GRC Platform | GRC Lead | *[signed]* | 2025-03-27 |
| Google Workspace | IT Manager | *[signed]* | 2025-03-26 |
| Learning Management System | HR Director | *[signed]* | 2025-03-25 |
| AWS Veridian AI tenancy | CTO | *[signed]* | 2025-03-28 |
| PCM-001 Application | VP, Customer Success | *[signed]* | 2025-03-25 |
| CRT-001 Application | General Counsel | *[signed]* | 2025-03-25 |

**ISO Attestation (overall review)**

I, Susan Orwell, Information Security Officer, attest that the Q1 2025 Quarterly User Access Review was conducted in accordance with ET-CTRL-001 and the [Access Control Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/access-control-policy.md); that all in-scope systems were reviewed; that exceptions were appropriately triaged and remediated or tracked to resolution; and that this record constitutes valid audit evidence of control operation.

**ISO Signature:** *[Susan Orwell: signed 2025-03-28]*

**CISO Review Confirmation**

Reviewed and approved. The Q1 2025 access review is confirmed complete. Open exception AR-EXC-2025-004 noted; remediation to be confirmed in Q2 review.

**CISO Signature:** *[signed 2025-03-28]*

---

## 8. Evidence Index

| Evidence Item | Location | Retention Period |
|---|---|---|
| This attestation record | GRC Platform / Portfolio Repository | 3 years |
| AWS IAM Access Analyzer exports (ET and Veridian AI tenancies) | GRC Platform / Secure Evidence Store | 3 years |
| GitHub audit log export (Q1 2025) | GRC Platform / Secure Evidence Store | 3 years |
| ServiceNow user report export | GRC Platform / Secure Evidence Store | 3 years |
| Google Workspace Admin Console export | GRC Platform / Secure Evidence Store | 3 years |
| LMS admin report export | GRC Platform / Secure Evidence Store | 3 years |
| System owner review worksheets (all 8 systems) | GRC Platform / Secure Evidence Store | 3 years |
| Exception remediation confirmations | GRC Platform (exception tickets AR-EXC-2025-001 through 008) | 3 years |
| CISO approval record | GRC Platform | 3 years |

---

## 9. Document Control

| Version | Date | Author | Summary of Changes |
|---|---|---|---|
| 1.0 | 2025-03-28 | GRC Analyst (J. Mirren) | Initial publication: Q1 2025 review |

- **Next Review:** Q2 2025 access review to be initiated by 2025-06-01
- **Control Reference:** [ET-CTRL-001](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/controls/et-ctrl-001-access-control-review.md): Quarterly Access Control Review
- **Framework Compliance:** [ISO 27001:2022](https://www.iso.org/standard/82875.html) A.8.2 [VERIFY]; [NIST CSF 2.0](https://www.nist.gov/cyberframework) PR.AC-1, PR.AC-4 [VERIFY]; [ISO/IEC 27002:2022](https://www.iso.org/standard/75652.html) 8.2 [VERIFY]

---

*This document was developed as part of the Emyzer Nexus Phase 2 GRC Programme and formatted for portfolio presentation. All individuals, access counts, and exception details are fictional.*

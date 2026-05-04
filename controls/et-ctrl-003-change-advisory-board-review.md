# ET-CTRL-003: Change Advisory Board (CAB) Review

| Field | Value |
|---|---|
| Control ID | ET-CTRL-003 |
| Title | Change Advisory Board (CAB) Review |
| Entity | Emyzer Technology |
| Regulatory citation | [ISO 27001:2022](https://www.iso.org/standard/27001.html) A.8.32 (Change management); [NIST SP 800-53 Rev. 5](https://csrc.nist.gov/pubs/sp/800/53/r5/upd1/final) CM-3 (Configuration Change Control), CM-4 (Impact Analyses); ITIL 4 Change Enablement practice [VERIFY: confirm current practice name and scope boundary in the ITIL 4 Foundation publication; the practice was renamed from "Change Management" in ITIL v3] |
| Control owner | Information Security Officer (Susan Orwell) |
| Control type | Preventive |
| Testing frequency | Per change request (all Normal and Major changes); Weekly CAB meeting |
| Last tested | [DATE] |
| Test result | [Pass / Fail / Exception noted] |
| Evidence reference | `evidence/[YEAR]/ET-CTRL-003/` |
| Status | Active |

---

## Control Description

The Change Advisory Board (CAB), chaired by the ISO, reviews and authorises Normal and Major changes to Emyzer Technology's information systems, configurations, and infrastructure before implementation. The CAB convenes weekly; emergency changes follow an expedited process.

**Change types under CAB governance:**

- **Standard changes**: Pre-approved, low-risk, routine changes following a documented and tested procedure. CAB review is not required unless the change deviates from the approved template. Logged in ServiceNow for the record.
- **Normal changes**: Submitted to the CAB at least 5 business days before the proposed implementation date. Require a risk assessment, test plan, rollback procedure, and business justification at the time of submission.
- **Major changes**: High-risk or high-impact changes requiring CAB review plus CISO or CTO approval. Extensive testing in a non-production environment is required before the CAB will approve implementation.
- **Emergency changes**: Implemented outside the standard cycle when a critical security or business need requires immediate action. Retrospective CAB review must be completed within 2 business days of implementation.

All changes are logged in the ServiceNow Change Management module. Authorisation records are retained for 3 years. Post-implementation reviews are required for all Major changes within 5 business days.

## Test Procedure

1. Pull the change log from ServiceNow for the review period. Confirm every Normal and Major change has an associated CAB-approved change record with a documented authorisation timestamp.
2. For a sample of Normal changes: verify that a risk assessment, test plan, and rollback procedure were present in the change record at the time of CAB review: not added after the fact.
3. For Major changes: confirm both CAB approval and CISO or CTO sign-off are on record, and that non-production testing was documented before approval.
4. For Emergency changes: confirm retrospective CAB review was completed within 2 business days and the emergency justification (business need or security risk) was documented at the time of implementation.
5. Check for unauthorised changes by cross-referencing deployment logs or configuration management system records against the CAB-approved change calendar for the period. Investigate any gaps.
6. Confirm that post-implementation reviews for all Major changes were completed within 5 business days and filed in ServiceNow.
7. File CAB meeting minutes, change records sample, and any exception documentation in `evidence/[YEAR]/ET-CTRL-003/`.

## Escalation

Unauthorised changes (implemented without a change record) are treated as potential security incidents and escalated to the CISO immediately. Repeated CAB non-compliance by a specific team is escalated to the relevant Department Head and documented in the risk register as an operational governance risk. Emergency changes where retrospective review was not completed within 2 business days are flagged to the Security Steering Committee.

## Change History

| Version | Date | Changed by | Summary of change |
|---|---|---|---|
| 1.0 | 2026-01-13 | Information Security Officer | Initial version |

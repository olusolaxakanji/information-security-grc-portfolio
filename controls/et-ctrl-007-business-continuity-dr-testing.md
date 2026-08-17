# ET-CTRL-007: Business Continuity and DR Testing

| Field | Value |
|---|---|
| Control ID | ET-CTRL-007 |
| Title | Business Continuity and Disaster Recovery Testing |
| Entity | Emyzer Technology |
| Regulatory citation | [ISO 22301:2019](https://www.iso.org/standard/75106.html) Cl. 8.5 (Exercise programme); [NIST SP 800-34 Rev. 1](https://csrc.nist.gov/pubs/sp/800/34/r1/final) Section 3.1 (Contingency Plan Testing); [ISO 27001:2022](https://www.iso.org/standard/27001.html) A.5.30 (ICT readiness for business continuity) |
| Control owner | Business Continuity Manager (Susan Orwell) |
| Control type | Detective / Corrective |
| Testing frequency | Semi-annual |
| Last tested | 2025-09-15 |
| Test result | Pass |
| Evidence reference | `evidence/2025/ET-CTRL-007/` |
| Status | Active |

---

## Control Description

The Business Continuity Manager conducts semi-annual exercises to validate that Emyzer Technology's BC/DR plans are operationally effective and that critical processes can be recovered within the RTOs and RPOs established in the Business Impact Analysis Report.

**Exercise types used in rotation:**

| Exercise Type | Description | Systems Activated |
|---|---|---|
| **Tabletop** | Structured discussion of a simulated disruption scenario. Participants walk through response and recovery steps against the BC/DR plan without activating live systems. | No |
| **Walkthrough / Technical test** | Component-level test of specific recovery procedures: for example, restoring data from backup to a non-production environment and validating data integrity and recovery time. | Partial |
| **Full interruption test** | Complete simulation of system failover to the DR environment under controlled conditions. Requires CISO and CRO approval; scheduled in advance to minimise operational impact. | Full |

The exercise schedule rotates through types to progressively test increasing levels of plan fidelity.

**Recovery objectives for Tier 1 critical processes (from the BIA):**
- RTO: 2–4 hours
- RPO: Real-time to 1 hour

Each exercise produces a formal test report covering: scenario and scope, participant list, observed recovery times, gap findings, and remediation actions with owners and target dates. BC/DR plans are updated within 30 days of any exercise that identifies material gaps.

## Test Procedure

1. Confirm two exercises were conducted in the review year (one per semi-annual cycle) and that the exercise types used were varied from the prior period.
2. For each exercise: verify a formal test report exists with the scenario, participant list, observed recovery times for Tier 1 processes, and gap findings.
3. For tabletop exercises: confirm that all critical function owners and IRT representatives participated and that the scenario tested a realistic disruption type (e.g., ransomware, data centre outage, key-person unavailability).
4. For technical tests: confirm that backup restoration was tested for at least one Tier 1 critical system and that the observed RPO was within target (≤1 hour for Tier 1). Document actual vs. target recovery times.
5. For any full interruption test conducted: confirm CISO and CRO pre-approval was obtained and a post-test debrief report was filed within 5 business days.
6. Verify that all remediation actions from the prior exercise have been resolved or have an active owner, target date, and current status update.
7. Confirm the BC/DR plan was reviewed and updated within 30 days of the most recent exercise.
8. File all exercise reports, updated plan versions, and remediation tracking records in `evidence/2025/ET-CTRL-007/`.

## Escalation

RTO or RPO exceedances discovered during testing are escalated to the CRO within 24 hours of the test result. A corrective action plan must be submitted within 5 business days. Failure to conduct either semi-annual exercise within the calendar year is escalated to the Security Steering Committee as a BC/DR programme gap. A finding that the BC/DR plan has not been updated following a prior exercise gap is escalated to the CRO as a governance risk.

## Change History

| Version | Date | Changed by | Summary of change |
|---|---|---|---|
| 1.0 | 2026-01-13 | Business Continuity Manager | Initial version |

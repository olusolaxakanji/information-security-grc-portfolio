# ET-CTRL-004 — Third-Party Vendor Risk Assessment

| Field | Value |
|---|---|
| Control ID | ET-CTRL-004 |
| Title | Third-Party Vendor Risk Assessment |
| Entity | Emyzer Technology |
| Regulatory citation | [ISO 27001:2022](https://www.iso.org/standard/27001.html) A.5.19 (Information security in supplier relationships), A.5.20 (Addressing IS in supplier agreements), A.5.21 (Managing IS in the ICT supply chain), A.5.22 (Monitoring, review and change management of supplier services); [NIST SP 800-161 Rev. 1](https://csrc.nist.gov/pubs/sp/800/161/r1/final) (C-SCRM Practices); [NIST CSF 2.0](https://www.nist.gov/cyberframework) GV.SC-4 (Suppliers are known), GV.SC-7 (Risks posed by suppliers are identified and prioritised) |
| Control owner | Information Security Officer (Susan Orwell) |
| Control type | Preventive / Detective |
| Testing frequency | Critical and High-tier: Annual; Medium-tier: Biennial; Low-tier: Triennial |
| Last tested | [DATE] |
| Test result | [Pass / Fail / Exception noted] |
| Evidence reference | `evidence/[YEAR]/ET-CTRL-004/` |
| Status | Active |

---

## Control Description

The ISO assesses all third-party vendors who access, process, store, or transmit Emyzer Technology data or systems against the security and compliance requirements defined in the Third-Party Risk Management Policy (KB-PORTFOLIO-0008).

**Vendor risk tiers and approval authority:**

| Tier | Examples | Reassessment | Approval |
|---|---|---|---|
| Critical | Cloud infrastructure, payment processors, identity management | Annual | CISO |
| High | SaaS platforms handling Confidential/Restricted data, MSSPs | Annual | ISO |
| Medium | Non-critical SaaS, professional services with limited data access | Biennial | Procurement + Business Owner |
| Low | Services with no data access | Triennial | Business Owner |

**Assessment scope:** Current security certifications (SOC 2 Type II or ISO 27001 certificate), SecurityScorecard or equivalent external rating (minimum threshold: 80), penetration testing cadence, incident notification SLAs, data handling and subprocessor practices, contractual security requirements, and regulatory compliance evidence relevant to the data being processed.

**New vendor onboarding:** No contract may be executed with a Critical or High-tier vendor without a completed risk assessment and written approval at the required authority level. The vendor register in ServiceNow is the system of record.

**Ongoing monitoring:** The ISO reviews SecurityScorecard ratings for Critical and High vendors monthly. Active SOC 2 or ISO 27001 certification is confirmed annually as part of the formal reassessment.

## Test Procedure

1. Pull the vendor register for the review period. Confirm reassessment completion rates by tier: Critical/High (annual), Medium (biennial), Low (triennial).
2. For a sample of Critical and High vendors: verify that a current security certification (SOC 2 Type II or ISO 27001) is on file, not expired, and that the scope covers services relevant to Emyzer Technology's use case.
3. For the same sample: verify the SecurityScorecard rating at last assessment met or exceeded 80. For any vendor rated below 80, confirm a remediation plan was obtained and tracked to resolution.
4. For new Critical or High vendors onboarded during the period: confirm a risk assessment was completed and approved at the required authority level before contract execution.
5. For any vendor where the risk tier changed: confirm a reassessment was triggered and completed within 30 days of the tier change.
6. For terminated vendor relationships: confirm access to Emyzer Technology systems was deprovisioned per the exit procedure and that written confirmation of data return or destruction was obtained.
7. File the vendor register, assessment records, and certification evidence in `evidence/[YEAR]/ET-CTRL-004/`.

## Escalation

Vendors rated below 80 on SecurityScorecard are placed on a 30-day remediation plan. Failure to remediate within 30 days is escalated to the CISO for a formal risk acceptance decision or contract termination review. Critical security events at a vendor — including a confirmed breach notification or loss of SOC 2 / ISO 27001 certification — are escalated to the CISO and CRO within 24 hours and trigger an emergency reassessment.

## Change History

| Version | Date | Changed by | Summary of change |
|---|---|---|---|
| 1.0 | 2026-01-13 | Information Security Officer | Initial version |

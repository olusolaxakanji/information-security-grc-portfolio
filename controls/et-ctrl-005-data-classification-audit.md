# ET-CTRL-005 — Data Classification Audit

| Field | Value |
|---|---|
| Control ID | ET-CTRL-005 |
| Title | Data Classification Audit |
| Entity | Emyzer Technology |
| Regulatory citation | [ISO 27001:2022](https://www.iso.org/standard/27001.html) A.5.12 (Classification of information), A.5.13 (Labelling of information); [NIST SP 800-60 Vol. 1 Rev. 1](https://csrc.nist.gov/pubs/sp/800/60/v1/r1/final) (Guide for Mapping Types of Information to Security Categories); [GDPR](https://gdpr.eu/) Art. 5(1)(b) (purpose limitation), Art. 5(1)(c) (data minimisation) |
| Control owner | Information Security Officer (Susan Orwell) |
| Control type | Detective |
| Testing frequency | Quarterly (Data Owner classification review); Annual (ISO-led labelling audit) |
| Last tested | [DATE] |
| Test result | [Pass / Fail / Exception noted] |
| Evidence reference | `evidence/[YEAR]/ET-CTRL-005/` |
| Status | Active |

---

## Control Description

Data Owners review and confirm the classification of information assets within their domain every quarter. The ISO conducts an annual labelling audit to verify that classification decisions are accurately reflected in applied labels and that handling controls appropriate to each tier are in force.

**Emyzer Technology data classification tiers:**

| Tier | Description | Handling Baseline |
|---|---|---|
| Public | No harm from unrestricted disclosure | No special controls required |
| Internal | Internal use; minor harm from unauthorised disclosure | Standard access controls; no external sharing without approval |
| Confidential | Business-sensitive; significant harm from disclosure | Encryption at rest and in transit; limited distribution |
| Restricted | Highest sensitivity: personal data (GDPR), legally privileged, regulated data | Strongest controls; encryption mandatory; DLP enforcement; CISO approval to share externally |

**Quarterly Data Owner review:** Each Data Owner attests to the classification of all information assets within their domain. New or modified assets are classified within 5 business days of creation or acquisition. Unclassified data discovered during a review is treated as Internal by default pending formal assessment.

**Annual labelling audit (ISO-led):** The ISO samples a cross-section of stored data, email, documents, and system outputs across at least two classification tiers. For each sample item, the audit verifies: (a) a classification label is applied; (b) the label matches the Data Owner's designation; and (c) handling controls appropriate to the classification are enforced (e.g., encryption state, DLP policy activation, access control group membership).

## Test Procedure

1. Pull the data inventory from the GRC platform and confirm that Data Owner quarterly attestations are complete for all domains in the review period.
2. Identify any new data assets created or acquired during the quarter that have not yet been classified, and confirm that the 5-business-day classification window was met.
3. For the annual audit: select a random sample of at least 20 items across at least two classification tiers from diverse storage locations (cloud storage, email, shared drives, database exports, API outputs).
4. For each sampled item: verify the applied label matches the Data Owner's designation; verify that applicable handling controls are in force (encryption at rest for Confidential and above, DLP rule active for Restricted, access group restricted to documented authorised users).
5. Document the audit sample list, per-item findings, and any exceptions in the evidence record.
6. Confirm that all classification exceptions identified in the prior period were remediated within the 5-business-day window.
7. File the Data Owner attestations, audit sample record, and findings report in `evidence/[YEAR]/ET-CTRL-005/`.

## Escalation

Misclassified Restricted data — data carrying a classification below Restricted where Restricted is warranted — is escalated to the CISO within 24 hours as a potential data handling incident. Systemic misclassification across an entire business domain is escalated to the relevant Data Owner's manager and documented in the risk register as a governance risk. Unresolved classification exceptions beyond the 5-business-day window are escalated to the ISO for review and either expedited classification or formal acceptance.

## Change History

| Version | Date | Changed by | Summary of change |
|---|---|---|---|
| 1.0 | 2026-01-13 | Information Security Officer | Initial version |

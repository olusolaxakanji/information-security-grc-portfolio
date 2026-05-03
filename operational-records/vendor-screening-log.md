# Vendor Screening Log — Q1 2025

---

## Document Metadata

| Field               | Detail                                                                                       |
|---------------------|----------------------------------------------------------------------------------------------|
| Document ID         | OPR-VS-2025-001                                                                              |
| Document Title      | Vendor Screening Log — Q1 2025 (January – March 2025)                                       |
| Period              | 1 January 2025 – 31 March 2025                                                               |
| Owner               | Vendor Risk Manager, Emyzer Nexus                                                            |
| Reviewed By         | Susan Orwell, ISO / CRO / BC Manager                                                         |
| Review Date         | 2025-04-04                                                                                   |
| Classification      | Confidential                                                                                 |
| Version             | 1.0                                                                                          |
| GitHub Reference    | https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/operational-records/vendor-screening-log.md |

---

## Purpose and Scope

This log documents all vendor security screenings initiated or completed by Emyzer Nexus during Q1 2025 (1 January to 31 March 2025). It covers both new vendor engagements and periodic reviews of existing vendors, conducted in accordance with the **Third-Party Risk Management Policy (TPRM-POL-001)** and the **Vendor Security Screening Procedure (TPRM-PROC-002)**.

Screenings are classified by vendor risk tier (Critical / High / Medium / Low) as assigned at onboarding and reviewed annually. The risk tier determines the scope of screening checks required (see TMPL-SR-001, Appendix) and the frequency of periodic review.

This period includes one screening conducted by Susan Orwell in her capacity as ISO, reflecting her ownership of vendor relationships involving access to internal GRC documentation. All other screenings were conducted by the Vendor Risk Manager or a GRC Analyst acting under delegation.

Vendor names that are third-party organisations are recorded using their actual legal or trading names where the relationship is publicly discernible from certifications or publicly disclosed contracts. Where identification would be commercially sensitive, the vendor category is recorded and the name is noted as redacted in the individual entry.

---

## Screening Log

| Screening ID | Vendor Name                    | Service Type                              | Risk Tier | Screening Date | Screened By              | Checks Completed                                                                                                     | Overall Outcome                                                         | Next Review Date | Notes                                                                                                                                                                              |
|--------------|--------------------------------|-------------------------------------------|-----------|----------------|--------------------------|----------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------|------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| SR-2025-001  | [LLM API Provider — name redacted per commercial sensitivity policy] | External AI/LLM API — integrated into CRT-001 (AI-Assisted Contract Review Tool) | Critical | 2025-01-20 | GRC Analyst (J. Mirren) | Information security assessment (vendor questionnaire + documentation review); data processing terms review; regulatory and sanctions list check (OFAC, HM Treasury, UN); sub-processor identification and review; AI-specific due diligence per AI Vendor Due Diligence Addendum | **Approved with Conditions** — Interim approval granted for use with non-PII, non-confidential documents only. Full approval contingent on DPA execution. See Open Conditions Log below. | 2025-07-20 | AI-specific due diligence applied per AI Vendor Risk Due Diligence Addendum. Vendor submitted EU AI Act Article 28 [VERIFY] compliance declaration; confirmation of technical conformity measures pending external validation. LLM API processes contract text; input filtering controls in place to prevent PII submission during interim period. CISO approval for interim use obtained 2025-01-22. |
| SR-2025-002  | Amazon Web Services (AWS)      | Cloud infrastructure — primary hosting environment (all production workloads including PCM-001 and CRT-001) | Critical | 2025-01-15 | Vendor Risk Manager (A. Patel) | SOC 2 Type II report review (issued 2024-09-30, no exceptions noted); ISO 27001:2022 certificate verification (cert. no. valid through 2026-05-14 [VERIFY with AWS Trust Center]); data processing addendum review (AWS DPA v3.2, executed 2023-11-01); BCP and DR capability review (AWS well-architected framework review completed 2024-Q4); regulatory and sanctions check; sub-processor list review | **Approved** — All checks passed. Annual renewal. No material changes from 2024 assessment. SOC 2 Type II (period ending 2024-09-30) showed no exceptions across security, availability, and confidentiality trust service criteria. | 2026-01-15 | SecurityScorecard rating: A (94/100) as of 2025-01-15. No active alerts. Continuous monitoring active — alert threshold set at score drop below 80 or Grade B. AWS is primary infrastructure provider for all Emyzer Nexus production environments. Sub-processor list reviewed: 12 sub-processors identified, all within AWS group entities. |
| SR-2025-003  | [External IR Firm — name redacted; leading UK-based cyber incident response consultancy] | Incident response retainer — surge IR capacity and specialist forensic support | High | 2025-02-05 | GRC Analyst (J. Mirren) | Information security assessment (ISO 27001 certification confirmed); professional indemnity and cyber liability insurance verification (£5M PI, £10M cyber verified); conflict-of-interest check (no current engagements with Emyzer Nexus competitors confirmed); reference checks (3 client references obtained — all satisfactory; references included one FTSE 250 financial services firm and one regulated healthcare organisation) | **Approved** — All checks passed. Retainer agreement executed 2025-02-12. | 2026-02-05 | Retainer engaged for surge IR capacity. Firm has hold on 72-hour on-site response SLA. No system access granted under retainer — access would be subject to a separate access authorisation process in the event of an incident. NDA executed 2025-01-28 prior to screening. |
| SR-2025-004  | Workday, Inc.                  | HR Information System (HCM SaaS) — processes all Emyzer Technology employee PII including payroll data, performance records, and absence data | High | 2025-02-20 | Vendor Risk Manager (A. Patel) | SOC 2 Type II report review (issued 2024-11-15; one management note regarding privileged access monitoring — no exception; note reviewed and assessed as immaterial); ISO 27001:2022 certificate verification (confirmed valid); data processing agreement review (Workday DPA, executed 2022-06-01, reviewed for continued adequacy under UK GDPR and EU GDPR); sub-processor list review (26 sub-processors identified; 3 new sub-processors added since 2024 review — assessed and approved); GDPR Article 28 [VERIFY] compliance confirmation | **Approved** — Annual renewal. No material changes from 2024 assessment. Sub-processor additions noted and assessed as low risk (all within Workday group entities or established tier-1 cloud providers). | 2026-02-20 | Workday processes employee PII for all ~5,000 Emyzer Technology staff. Classified as High tier under TPRM-POL-001 due to PII volume and processing sensitivity. Data classified Confidential under Data Classification Policy. SecurityScorecard rating: B+ (83/100) — slight decline from 86/100 in 2024 review; Vendor Risk Manager to raise with Workday account team at next QBR (scheduled 2025-04-15). |
| SR-2025-005  | [Regional Professional Services Firm — name redacted; mid-sized UK GRC consultancy] | GRC consultancy — 6-month sprint engagement to support M&A integration GRC workstream (Veridian AI integration) | Medium | 2025-03-10 | Susan Orwell (ISO / CRO / BC Manager) | Background check on lead consultant (identity verification, right to work, employment history verification 5 years, 2 professional references — all satisfactory); professional indemnity insurance verification (£2M PI confirmed); NDA executed prior to any information disclosure; conflict-of-interest declaration (no conflicts declared — confirmed no current or recent engagements with Veridian AI or related entities) | **Approved** — All checks passed. Engagement commenced 2025-03-17. | 2025-09-10 | Classified as Medium tier (professional services, no system access). Access limited to internal documentation shared on a need-to-know basis — no direct system access to ServiceNow, SIEM, or production environments. Document sharing via encrypted SharePoint site only. NDA signed 2025-03-09. Engagement scope: GRC framework gap analysis and policy harmonisation workstream for Emyzer Nexus / Veridian AI integration. End date: 2025-09-12. |

---

## Screening Summary — Q1 2025

| Metric                              | Count |
|-------------------------------------|-------|
| Total screenings completed this period | 5  |
| Approved (no conditions)            | 3     |
| Approved with Conditions            | 1     |
| Rejected                            | 0     |
| Deferred                            | 0     |
| Critical tier screenings            | 2     |
| High tier screenings                | 2     |
| Medium tier screenings              | 1     |
| Low tier screenings                 | 0     |

---

## Open Conditions Log

The following conditions were attached to "Approved with Conditions" outcomes and remain open as at 31 March 2025. Each condition must be resolved by the target date or the relevant approval will lapse and the engagement will be reviewed.

| Condition ID    | Screening ID | Vendor                        | Condition Description                                                                              | Target Date  | Owner                        | Status as at 31-Mar-2025                                |
|-----------------|--------------|-------------------------------|----------------------------------------------------------------------------------------------------|--------------|------------------------------|---------------------------------------------------------|
| COND-2025-001-A | SR-2025-001  | LLM API Provider (redacted)   | Execute Data Processing Agreement covering all processing activities related to CRT-001 integration. Until DPA is executed, use restricted to non-PII, non-confidential document content only. | 2025-03-31   | GRC Analyst (J. Mirren) / Legal (contract lead) | **Overdue** — DPA negotiations in progress. Vendor proposed amendments to standard DPA on 2025-03-18; Legal review in progress. Revised target: 2025-04-30. CISO notified of delay 2025-04-01. Non-PII restriction remains in force. |
| COND-2025-001-B | SR-2025-001  | LLM API Provider (redacted)   | Obtain confirmation from vendor of technical conformity measures under EU AI Act Article 28 [VERIFY] — specifically confirmation of logs retention, human oversight capability, and transparency obligations for downstream deployer use. | 2025-06-30   | Vendor Risk Manager (A. Patel) | In progress — vendor engaged; confirmation expected Q2 2025. |

---

## Q2 2025 Upcoming Screenings

The following vendor screenings are due during Q2 2025 (April – June 2025). Vendor Risk Manager to initiate each screening at least 4 weeks before the due date.

| Vendor / Category                          | Risk Tier | Review Type     | Due Date     | Notes                                                                 |
|--------------------------------------------|-----------|-----------------|--------------|-----------------------------------------------------------------------|
| LLM API Provider (SR-2025-001)             | Critical  | Condition closure + 6-month interim review | 2025-07-20 | Conditions from SR-2025-001 must be resolved before full approval. Interim review at 6 months as agreed at approval. |
| Veridian AI — inherited vendor list review | Critical / High | New engagement screening (post-M&A) | By 2025-06-30 | Veridian AI critical and high-tier vendors must be screened under Emyzer Nexus TPRM standards. Vendor Risk Manager to obtain inherited vendor list from Veridian AI integration workstream by 2025-04-15. |
| Penetration Testing Provider               | High      | Annual renewal  | 2025-05-15   | Annual retainer renewal due. Previous screening: SR-2024-018.        |
| [Legal Technology SaaS — contract management platform] | High | Annual renewal | 2025-06-01 | DPA review required — EU SCCs may require update following recent guidance. |

---

*Document prepared by: Vendor Risk Manager (A. Patel), 2025-04-04*
*Reviewed and approved by: Susan Orwell, ISO, 2025-04-04*
*Next quarterly log: OPR-VS-2025-002 (Q2 2025)*
*Stored in: GRC Platform (ServiceNow) — Third-Party Risk module*

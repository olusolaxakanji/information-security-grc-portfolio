# M&A Risk Assessment: Veridian AI Acquisition

**Emyzer Nexus: Integration Management Programme**

---

## Document Information

| Attribute | Value |
|---|---|
| **Document ID** | INT-RA-001 |
| **Document Type** | M&A Risk Assessment |
| **Version** | 1.1 |
| **Effective Date** | 2025-01-15 |
| **Last Updated** | 2025-07-01 |
| **Owner** | Chief Risk Officer (Susan Orwell) |
| **Classification** | Internal Use: Restricted |
| **Methodology** | [Risk Assessment Methodology](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/risk-assessments/risk-assessment-methodology.md) (5×5 matrix) extended with M&A-specific and AI-specific risk categories |

---

## 1. Purpose

This risk assessment identifies and evaluates the GRC risks arising from Emyzer Nexus's acquisition and integration of Veridian AI. It applies the Phase 1 Risk Assessment Methodology, a 5×5 likelihood × impact matrix producing scores of 1–25 (Critical ≥15, High 10–14, Medium 5–9, Low 1–4), extended with two additional risk categories relevant to the M&A context: AI-Specific Risks and Integration Governance Risks.

This assessment covers GRC risks arising from the acquisition. It excludes financial and commercial risks, which were assessed by the deal team prior to acquisition close, and technical integration risks, which are governed by a separate technical integration project.

---

## 2. Assessment Scope

| In Scope | Description |
|---|---|
| Technology risks | Risks arising from the state and governance of Veridian AI's technical assets, particularly PCM-001 and CRT-001 |
| Regulatory risks | Compliance exposure inherited through the acquisition, including EU AI Act and GDPR obligations |
| Data and privacy risks | Risks arising from inherited data assets, data processing practices, and privacy obligations |
| Personnel risks | Risks from key person dependencies, knowledge concentration, and policy compliance gaps in the Veridian AI workforce |
| Operational risks | Risks to ongoing operations arising from the integration process, vendor relationships, and capacity constraints |

| Out of Scope | Description |
|---|---|
| Financial and commercial risks | Assessed by deal team; not duplicated here |
| Technical integration risks | Governed by technical integration project; flagged here only where they create GRC exposure |

---

## 3. Risk Categories

| Category | Description |
|---|---|
| **Technology** | Risks from the state of Veridian AI's technical assets and the quality of technical governance |
| **Regulatory** | Compliance exposures inherited from Veridian AI's operations and triggered by the acquisition |
| **Data / Privacy** | Risks arising from inherited data assets and data processing practices |
| **Personnel** | Risks from key person dependencies, knowledge concentration, and staff transition |
| **Operational** | Risks to ongoing Emyzer Nexus operations from the integration process, vendor relationships, and capacity |

---

## 4. Risk Register

### INT-RISK-2025-001 | Undocumented AI System Architecture

| Field | Value |
|---|---|
| **Risk ID** | INT-RISK-2025-001 |
| **Domain** | Technology |
| **Risk Owner** | CTO |
| **Risk Description** | At the time of acquisition, technical documentation for PCM-001 (Predictive Customer Churn Model) and CRT-001 (AI-Assisted Contract Review Tool) was insufficient to support EU AI Act Article 11 [VERIFY] conformity requirements. Model architecture, training methodology, and performance metrics were partially documented in Veridian AI engineering repositories, but no formal technical documentation package existed. Without complete documentation, Emyzer Nexus cannot satisfy regulatory examination requirements, cannot fully assess the models' risk profiles, and cannot complete conformity assessments. |
| **Threat Source** | Structural: Veridian AI did not maintain formal technical documentation as a pre-IPO-stage startup |
| **Vulnerability** | No documentation governance programme existed at Veridian AI prior to acquisition |
| **Likelihood** | 4 (Likely: documentation gap is confirmed; probability refers to risk of non-remediation causing compliance failure) |
| **Impact** | 4 (High: EU AI Act enforcement; inability to complete conformity assessments) |
| **Risk Rating** | **16: Critical** |
| **Existing Controls** | Engineering documentation sprint initiated immediately post-acquisition; two Veridian AI engineers retained specifically to support documentation |
| **Control Effectiveness** | Partial: sprint underway; completion dependent on knowledge retained by departing engineers |
| **Treatment Strategy** | Mitigate |
| **Treatment Status** | In Treatment |
| **Target Date** | 2025-09-30 (PCM-001); 2025-12-31 (CRT-001) |
| **Review Date** | 2025-Q3 |
| **Comments** | PCM-001 documentation progressing well, Veridian AI ML engineer on 12-month retention contract. CRT-001 documentation is partially blocked by third-party API opacity, vendor cooperation required for full Article 11 [VERIFY] compliance. CTO and Legal Counsel managing vendor engagement. |

---

### INT-RISK-2025-002 | Shadow AI: Undiscovered AI Systems

| Field | Value |
|---|---|
| **Risk ID** | INT-RISK-2025-002 |
| **Domain** | Technology |
| **Risk Owner** | CTO / GRC Team |
| **Risk Description** | Veridian AI may have developed, tested, or operated AI systems beyond the two systems (PCM-001, CRT-001) disclosed during due diligence. If additional AI systems were deployed, even in prototype or internal-use status, they may create EU AI Act classification obligations or GDPR compliance gaps that have not been assessed. |
| **Threat Source** | Structural: AI-native startup culture; informal development practices; potential incomplete due diligence disclosure |
| **Vulnerability** | No AI system inventory existed at Veridian AI prior to acquisition |
| **Likelihood** | 3 (Possible) |
| **Impact** | 3 (Moderate: additional systems would require classification and potential conformity assessment; operational disruption if systems must be suspended) |
| **Risk Rating** | **9: Medium** |
| **Existing Controls** | Shadow AI discovery exercise completed: comprehensive code repository audit, engineering interview programme, and cloud infrastructure scan conducted Q1–Q2 2025 |
| **Control Effectiveness** | Good: systematic discovery exercise completed |
| **Treatment Strategy** | Mitigate |
| **Treatment Status** | **Closed: Discovery Exercise Complete** |
| **Target Date** | 2025-06-30 (completed) |
| **Review Date** | 2025-Q4 |
| **Comments** | Shadow AI discovery exercise completed 2025-05-31. No additional AI systems identified beyond PCM-001 and CRT-001. Three internal ML prototypes identified: assessed as non-production, non-deployed, and not requiring EU AI Act classification at this stage. Prototypes archived and documented. Risk reduced; residual risk: re-emerges if new development begins without AI Governance Committee notification. AI Governance Policy obligation addresses this going forward. |

---

### INT-RISK-2025-003 | EU AI Act Non-Compliance for Inherited High-Risk Systems

| Field | Value |
|---|---|
| **Risk ID** | INT-RISK-2025-003 |
| **Domain** | Regulatory |
| **Risk Owner** | CISO / AI Governance Committee |
| **Risk Description** | PCM-001 and CRT-001 were in active production at the time of acquisition without EU AI Act conformity assessments. Under the EU AI Act, placing a High-Risk AI system into service without a completed conformity assessment constitutes a violation [VERIFY: EU AI Act Article 16, transitional provisions for systems in service before the Act's application date]. Emyzer Nexus assumed the compliance obligation of Veridian AI upon acquisition. The systems continue to operate during the transition period, creating ongoing enforcement exposure. The EU AI Act's applicability timeline [VERIFY: confirm relevant date for High-Risk systems under Article 97 and transitional provisions] determines urgency. |
| **Threat Source** | Regulatory: EU AI Act [VERIFY]; inherited from Veridian AI pre-acquisition operations |
| **Vulnerability** | Systems in production without conformity governance; inherited compliance gap confirmed |
| **Likelihood** | 5 (Almost Certain: the gap is confirmed; probability refers to regulatory discovery if conformity assessments are not completed) |
| **Impact** | 5 (Critical: penalties up to €30M or 6% of global annual turnover for High-Risk system non-compliance [VERIFY: EU AI Act Article 99 penalty tiers]) |
| **Risk Rating** | **25: Critical** |
| **Existing Controls** | Interim human oversight protocols implemented for both systems; conformity assessments initiated 2025-06-01; AI Governance Committee oversight; Legal Counsel monitoring EU AI Act application timeline [VERIFY] |
| **Control Effectiveness** | Partial: interim controls reduce risk of harm; compliance gap remains open until conformity assessments complete |
| **Treatment Strategy** | Mitigate |
| **Treatment Status** | In Treatment: conformity assessments in progress |
| **Target Date** | PCM-001: 2025-09-30; CRT-001: 2025-12-31 |
| **Review Date** | Monthly: escalated to CISO |
| **Comments** | This is the highest-priority risk in the M&A risk register. Legal Counsel monitoring EU AI Act application dates [VERIFY] to confirm whether transitional provisions apply to systems already in service. Conformity assessment for PCM-001 progressing; CRT-001 more complex due to third-party API dependency. CISO provides monthly update to CEO. |

---

### INT-RISK-2025-004 | GDPR Compliance Gap: CRT-001 Data Transmission

| Field | Value |
|---|---|
| **Risk ID** | INT-RISK-2025-004 |
| **Domain** | Regulatory |
| **Risk Owner** | Data Protection Officer |
| **Risk Description** | CRT-001 transmits contract document text, including personal data, to an external LLM API without a Data Processing Agreement. Under GDPR Article 28 [VERIFY], personal data may only be processed by a third party under a compliant DPA. The absence of a DPA means every CRT-001 API call involving personal data is an unlawful processing operation. GDPR enforcement by the competent supervisory authority could result in penalties up to €20M or 4% of global annual turnover [VERIFY: Article 83(4) penalty scale]. The risk was inherited from Veridian AI, which did not treat the LLM API vendor as a data processor. |
| **Threat Source** | Regulatory: GDPR Article 28 [VERIFY]; inherited from Veridian AI |
| **Vulnerability** | No DPA executed; no processor assessment completed |
| **Likelihood** | 4 (Likely: the gap is confirmed; enforcement probability depends on supervisory authority scrutiny) |
| **Impact** | 4 (High: material penalties; regulatory notification requirements; reputational impact) |
| **Risk Rating** | **16: Critical** |
| **Existing Controls** | Use restriction implemented: CRT-001 restricted to contracts without personal data pending DPA; Legal Counsel leading DPA negotiation |
| **Control Effectiveness** | Moderate: use restriction reduces but does not eliminate exposure; compliance depends on operator adherence |
| **Treatment Strategy** | Mitigate |
| **Treatment Status** | In Treatment: DPA negotiation in progress; target 2025-09-30 |
| **Review Date** | Monthly |
| **Comments** | DPA negotiation underway with LLM API vendor. Vendor has provided draft DPA; Legal Counsel reviewing against Emyzer Nexus standard requirements. Key open points: sub-processor list, data retention terms, deletion-on-request obligations. Target execution: 2025-09-30. |

---

### INT-RISK-2025-005 | Unresolved Pre-Acquisition Incident Obligations

| Field | Value |
|---|---|
| **Risk ID** | INT-RISK-2025-005 |
| **Domain** | Regulatory |
| **Risk Owner** | Legal Counsel |
| **Risk Description** | Veridian AI may have experienced AI system incidents prior to acquisition that triggered, or should have triggered, reporting obligations to national market surveillance authorities under EU AI Act Article 73 [VERIFY] or data breach notifications under GDPR Article 33 [VERIFY]. If such incidents occurred and were not reported, Emyzer Nexus has inherited an ongoing regulatory notification obligation. Due diligence identified no reported incidents; however, the absence of a formal incident management programme at Veridian AI means no definitive assurance is available. |
| **Threat Source** | Regulatory: inherited unreported incidents; structural: Veridian AI had no formal incident management programme |
| **Vulnerability** | No incident records available; informal pre-acquisition operations |
| **Likelihood** | 2 (Unlikely: no specific incidents identified; but cannot be confirmed absent) |
| **Impact** | 4 (High: late regulatory notification is a compliance violation; penalties may apply [VERIFY]) |
| **Risk Rating** | **8: Medium** |
| **Existing Controls** | Legal Counsel conducted post-acquisition review of available Veridian AI records; engineering team interviewed; no incidents identified |
| **Control Effectiveness** | Moderate: review conducted; absence of records does not definitively confirm absence of incidents |
| **Treatment Strategy** | Accept (residual) |
| **Treatment Status** | Accepted: Legal Counsel review complete; no incidents identified; voluntary disclosure protocols in place if further information emerges |
| **Target Date** | N/A |
| **Review Date** | 2025-Q4 |
| **Comments** | Legal Counsel review completed 2025-03-31. No specific incidents identified. Residual risk accepted. If any evidence of pre-acquisition incidents emerges, Legal Counsel will assess notification obligations immediately. |

---

### INT-RISK-2025-006 | PCM-001 Training Data Provenance and Consent

| Field | Value |
|---|---|
| **Risk ID** | INT-RISK-2025-006 |
| **Domain** | Data / Privacy |
| **Risk Owner** | Data Protection Officer |
| **Risk Description** | PCM-001's training dataset contains personal data collected by Veridian AI from its client base over approximately 3 years. The lawful basis for collecting and using this data to train a machine learning model has not been verified. If the data was collected under a purpose that does not extend to ML training (compatibility analysis required under GDPR Article 6(4) [VERIFY]) or if adequate consent or legitimate interest assessments were not conducted, the training dataset's use is unlawful. Emyzer Nexus inherited this exposure on acquisition. |
| **Threat Source** | Regulatory: GDPR; inherited from Veridian AI data collection practices |
| **Vulnerability** | Pre-acquisition data governance documentation unavailable or incomplete |
| **Likelihood** | 3 (Possible) |
| **Impact** | 5 (Critical: unlawful processing of training data could require deletion of the dataset, making PCM-001 non-operational until retrained on lawfully collected data; regulatory penalties) |
| **Risk Rating** | **15: High** |
| **Existing Controls** | DPO-led audit in progress; training data access restricted pending review |
| **Control Effectiveness** | Partial: controls on current use; underlying legal basis question unresolved |
| **Treatment Strategy** | Mitigate |
| **Treatment Status** | In Treatment: DPO audit in progress |
| **Target Date** | 2025-09-30 |
| **Review Date** | 2025-Q3 |
| **Comments** | DPO conducting formal legal basis assessment. Options being assessed: (1) if existing data is lawful: document the basis and implement GDPR-compliant retention governance; (2) if existing data requires supplement: plan for new data collection on clear legal basis; (3) if existing data is entirely unlawful: assess model impact and plan retrain timeline. |

---

### INT-RISK-2025-007 | Unclassified Veridian AI PII Assets

| Field | Value |
|---|---|
| **Risk ID** | INT-RISK-2025-007 |
| **Domain** | Data / Privacy |
| **Risk Owner** | Data Protection Officer |
| **Risk Description** | Veridian AI's data assets, client records, employee data, operational logs, and other PII, were not classified under any formal data classification scheme at the time of acquisition. Without classification, appropriate handling controls (encryption, access restriction, retention limits) cannot be systematically applied. Unclassified PII creates GDPR compliance gaps and potential for inadvertent exposure. |
| **Threat Source** | Structural: absence of data governance programme at Veridian AI |
| **Vulnerability** | No data inventory; no classification applied; handling controls inconsistent |
| **Likelihood** | 4 (Likely: absence of classification is confirmed) |
| **Impact** | 3 (Moderate: GDPR compliance gaps; potential for inadvertent exposure; operationally manageable) |
| **Risk Rating** | **12: High** |
| **Existing Controls** | Emyzer Technology Data Classification Policy applied to all Veridian AI data from 2025-01-15; classification exercise in progress |
| **Control Effectiveness** | Partial: policy applies; classification exercise not yet complete |
| **Treatment Strategy** | Mitigate |
| **Treatment Status** | In Treatment |
| **Target Date** | 2025-09-30 |
| **Review Date** | 2025-Q3 |
| **Comments** | DPO-led data classification exercise underway for all inherited Veridian AI data assets. Priority: client data (highest sensitivity), employee data (GDPR employee context), operational logs (retention assessment). Target: initial classification complete 2025-09-30. |

---

### INT-RISK-2025-008 | Key Person Dependency: AI System Knowledge

| Field | Value |
|---|---|
| **Risk ID** | INT-RISK-2025-008 |
| **Domain** | Personnel |
| **Risk Owner** | CTO |
| **Risk Description** | The architectural knowledge of PCM-001 and CRT-001 is concentrated in two Veridian AI engineers who joined Emyzer Nexus post-acquisition. If either or both depart before the documentation sprint is complete, critical knowledge of model architecture, training decisions, and system dependencies will be lost, significantly impeding conformity assessment completion and future model governance. The risk is elevated because post-acquisition talent retention in AI engineering is challenging, particularly where compensation structures change. |
| **Threat Source** | Structural: key person dependency; talent retention risk in competitive AI engineering market |
| **Vulnerability** | Knowledge not yet documented; retention contracts have limited tenure |
| **Likelihood** | 3 (Possible) |
| **Impact** | 4 (High: loss of technical knowledge would delay or prevent conformity assessment completion; EU AI Act compliance timeline at risk) |
| **Risk Rating** | **12: High** |
| **Existing Controls** | Both engineers on 12-month retention contracts (to 2025-Q4); knowledge transfer sessions in progress; documentation sprint underway |
| **Control Effectiveness** | Moderate: retention contracts reduce near-term risk; documentation sprint is the permanent solution |
| **Treatment Strategy** | Mitigate |
| **Treatment Status** | In Treatment |
| **Target Date** | 2025-09-30 (documentation complete; knowledge dependency resolved) |
| **Review Date** | 2025-Q3 |
| **Comments** | Documentation sprint on track for PCM-001. CRT-001 documentation partially dependent on vendor cooperation for API aspects. If either engineer indicates intention to depart before documentation completion, immediate escalation to CTO and IMC for retention negotiation. |

---

### INT-RISK-2025-009 | Veridian AI Staff: Policy Compliance Gap

| Field | Value |
|---|---|
| **Risk ID** | INT-RISK-2025-009 |
| **Domain** | Personnel |
| **Risk Owner** | HR / ISO (Susan Orwell) |
| **Risk Description** | All 212 Veridian AI staff became subject to Emyzer Nexus and Emyzer Technology policies from acquisition close. Staff accustomed to a startup operating model, without formal information security requirements, access control governance, or acceptable use restrictions, may inadvertently or deliberately operate outside policy requirements during the transition period. |
| **Threat Source** | Structural: cultural adjustment required; policy obligations newly imposed |
| **Vulnerability** | Staff unfamiliar with policies; no previous GRC programme culture |
| **Likelihood** | 4 (Likely: policy violations during transition periods are common) |
| **Impact** | 2 (Low: isolated violations unlikely to cause material harm if detection controls are in place) |
| **Risk Rating** | **8: Medium** |
| **Existing Controls** | Mandatory security awareness and AI governance training completed by all 212 staff by 2025-03-31 (100% completion); policy acknowledgements signed; line manager responsibility for team compliance |
| **Control Effectiveness** | Good: training and acknowledgement completed; ongoing compliance monitored |
| **Treatment Strategy** | Mitigate |
| **Treatment Status** | Monitoring |
| **Target Date** | N/A: ongoing |
| **Review Date** | 2025-Q4 |
| **Comments** | Training completion confirmed (see OPR-TC-2025-001). Ongoing monitoring via access logs, incident reporting, and quarterly access reviews. Minor policy query rate higher than ET average in first 90 days: expected during transition. No significant policy violations identified. |

---

### INT-RISK-2025-010 | LLM API Contract Non-Novation

| Field | Value |
|---|---|
| **Risk ID** | INT-RISK-2025-010 |
| **Domain** | Operational |
| **Risk Owner** | Legal Counsel / Vendor Risk Manager |
| **Risk Description** | The LLM API vendor contract for CRT-001 was in Veridian AI's name and was not formally novated to Emyzer Nexus at acquisition close. Emyzer Nexus's continued API access is therefore on informal terms: the vendor may not be under any contractual obligation to Emyzer Nexus, and there is no SLA, no breach notification obligation running to Emyzer Nexus, and no contractual basis for the data processing relationship. This creates both a legal exposure and a practical risk that the vendor could revoke access. |
| **Threat Source** | Contractual: novation not completed; structural: acquisition close without full contract novation |
| **Vulnerability** | No novated contract; vendor relationship on informal basis |
| **Likelihood** | 3 (Possible: vendor has been informally cooperative; but has no contractual obligation) |
| **Impact** | 4 (High: access revocation would render CRT-001 non-functional; no contractual remedies available) |
| **Risk Rating** | **12: High** |
| **Existing Controls** | Informal vendor cooperation maintained; Legal Counsel in active negotiation for novation |
| **Control Effectiveness** | Low: informal cooperation is not a control |
| **Treatment Strategy** | Mitigate |
| **Treatment Status** | In Treatment: novation negotiation in progress |
| **Target Date** | 2025-06-30 |
| **Review Date** | 2025-Q2 (urgent) |
| **Comments** | This is the second-highest priority vendor remediation item after the DPA. Legal Counsel has engaged vendor; combined novation + DPA + SLA negotiation being conducted in a single engagement to reduce vendor fatigue. Target: novated contract with DPA and service continuity provisions executed by 2025-09-30 (joint deadline with GAP-003). |

---

### INT-RISK-2025-011 | Unassessed Veridian AI Third-Party Vendor Portfolio

| Field | Value |
|---|---|
| **Risk ID** | INT-RISK-2025-011 |
| **Domain** | Operational |
| **Risk Owner** | Vendor Risk Manager |
| **Risk Description** | Veridian AI maintained vendor relationships across cloud infrastructure, development tooling, and business operations that were not assessed under the Emyzer Technology Third-Party Risk Management Programme prior to acquisition close. Post-acquisition, these vendors are now supply chain dependencies for Emyzer Nexus operations, but their security posture, contractual obligations, and compliance status have not been evaluated. |
| **Threat Source** | Structural: vendor portfolio acquired without prior due diligence |
| **Vulnerability** | Vendor risk assessments not completed; contractual security requirements not verified |
| **Likelihood** | 3 (Possible) |
| **Impact** | 3 (Moderate: vendor portfolio is not large; most relationships are commercial SaaS tools with standard terms) |
| **Risk Rating** | **9: Medium** |
| **Existing Controls** | Vendor inventory completed Q1 2025; risk tiering applied; Critical and High-tier vendors prioritised for assessment |
| **Control Effectiveness** | Moderate: inventory complete; assessments in progress |
| **Treatment Strategy** | Mitigate |
| **Treatment Status** | In Treatment |
| **Target Date** | 2025-09-30 |
| **Review Date** | 2025-Q3 |
| **Comments** | Vendor inventory identified 12 active Veridian AI vendor relationships: 1 Critical (LLM API: being assessed), 3 High (cloud providers, HRIS), 8 Medium/Low (SaaS tools). Critical and High assessments in progress. Medium/Low vendors to be assessed by 2025-09-30 via the standard TPRM cycle. |

---

### INT-RISK-2025-012 | GRC Integration Capacity Constraint

| Field | Value |
|---|---|
| **Risk ID** | INT-RISK-2025-012 |
| **Domain** | Operational |
| **Risk Owner** | Chief Risk Officer (Susan Orwell) |
| **Risk Description** | The volume of GRC integration workstreams, AI governance, policy application, data governance, vendor due diligence, risk register integration, and policy rationalization, exceeds the current GRC team's capacity to execute all workstreams simultaneously to schedule. Without sufficient capacity, lower-priority workstreams will slip, potentially creating compliance gaps if a deferred item turns out to be more critical than assessed. |
| **Threat Source** | Structural: resource constraint; integration complexity underestimated at planning stage |
| **Vulnerability** | GRC team of 3 people managing 8 simultaneous workstreams; no contingency capacity |
| **Likelihood** | 3 (Possible) |
| **Impact** | 2 (Low: delays to non-critical workstreams are manageable; critical workstreams (AI conformity, DPA) have dedicated resource) |
| **Risk Rating** | **6: Medium** |
| **Existing Controls** | External GRC consultant engaged for 6-month sprint (contract start 2025-03-10); workstream priority framework applied; IMC monthly oversight |
| **Control Effectiveness** | Good: external consultant provides material capacity augmentation |
| **Treatment Strategy** | Accept (residual after external consultant engagement) |
| **Treatment Status** | Monitoring |
| **Target Date** | N/A |
| **Review Date** | 2025-Q4 |
| **Comments** | External GRC consultant (SR-2025-005) engaged and productive. Consultant focused on policy rationalization and vendor assessment documentation. Capacity position improved from Critical constraint to manageable. Reassess at consultant contract end (2025-09-10): extend if critical workstreams remain open. |

---

## 5. Risk Distribution

### By Risk Level

| Risk Level | Count | % of Total |
|---|---|---|
| Critical (≥15) | 3 | 25% |
| High (10–14) | 5 | 42% |
| Medium (5–9) | 4 | 33% |
| Low (1–4) | 0 | 0% |
| **Total** | **12** | **100%** |

### By Category

| Category | Critical | High | Medium | Total |
|---|---|---|---|---|
| Technology | 1 | 0 | 1 | 2 |
| Regulatory | 2 | 1 | 0 | 3 |
| Data / Privacy | 0 | 2 | 0 | 2 |
| Personnel | 0 | 1 | 1 | 2 |
| Operational | 0 | 1 | 2 | 3 |

### By Treatment Status

| Status | Count | Risk IDs |
|---|---|---|
| In Treatment | 8 | 001, 003, 004, 006, 007, 008, 010, 011 |
| Monitoring | 2 | 009, 012 |
| Accepted (residual) | 1 | 005 |
| Closed | 1 | 002 |

---

## 6. Governance and Treatment Monitoring

### Review Cadence

| Activity | Frequency | Responsible |
|---|---|---|
| Critical risk status | Monthly | IMC / CISO |
| High risk status | Monthly | CRO / Risk Owners |
| Full register review | Quarterly (IMC meeting) | CRO / GRC Team |
| Full reassessment | At charter renewal (2026-01-15) | GRC Team |

### Escalation Thresholds

- New Critical risk identified: Immediate CISO and CRO notification; IMC emergency session within 5 business days
- Risk escalates to Critical: CEO notification within 24 hours
- Treatment deadline missed by >30 days: IMC escalation; revised treatment plan required

---

## 7. Framework Alignment

| Framework | Application |
|---|---|
| **[ISO 31000:2018](https://www.iso.org/standard/65694.html)** | M&A risk identification and treatment methodology; risk categories |
| **[ISO 27005:2022](https://www.iso.org/standard/80585.html)** [VERIFY] | Information security risk management extended to acquisition context |
| **[NIST CSF 2.0](https://www.nist.gov/cyberframework): ID.RA** [VERIFY] | Risk assessment: identification of assets, vulnerabilities, and threat actors relevant to acquisition |
| **[EU AI Act (Regulation 2024/1689)](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32024R1689)** [VERIFY] | Regulatory risk category: Article 9, Article 16, Article 99 obligations for High-Risk systems |
| **[GDPR (Regulation 2016/679)](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32016R0679)** [VERIFY] | Data and privacy risk category: Article 28, Article 33, Article 83 obligations |

---

## 8. Document Control

| Version | Date | Author | Changes |
|---|---|---|---|
| 1.0 | 2025-01-15 | GRC Team | Initial publication at acquisition close |
| 1.1 | 2025-07-01 | GRC Team | Closed INT-RISK-2025-002 (shadow AI discovery complete); updated treatment statuses; added comments on DPA negotiation progress |

- **Document ID:** INT-RA-001
- **Classification:** Internal Use: Restricted
- **Next Review:** 2025-Q4 (quarterly review per Section 6)

---

*This document was developed as part of the Emyzer Nexus Phase 2 GRC programme and formatted for portfolio presentation.*

# Veridian AI: Inherited AI System Risk Assessment

**Emyzer Nexus: M&A Due Diligence and Integration Risk Programme**

---

> **Simulated Environment**
>
> Emyzer Nexus is a fictional organisation created for this GRC portfolio. All entities, personnel, systems, risk findings, and regulatory scenarios are invented for professional demonstration purposes. Framework and regulatory references, [EU AI Act (Regulation 2024/1689)](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32024R1689), [NIST AI RMF 1.0](https://www.nist.gov/artificial-intelligence/ai-risk-management-framework), [ISO 31000:2018](https://www.iso.org/standard/65694.html), [NIST SP 800-30 Rev. 1](https://csrc.nist.gov/publications/detail/sp/800-30/rev-1/final), are accurate as of the document dates. No real organisation, individual, or AI system is represented.

---

## Document Information

| Attribute | Value |
|---|---|
| **Document ID** | VDA-RA-2025-001 |
| **Document Type** | M&A Due Diligence AI System Risk Assessment |
| **Version** | 1.0 |
| **Assessment Period** | 2025-01-15 to 2025-05-30 |
| **Effective Date** | 2025-05-30 |
| **Owner** | Chief Risk Officer (Susan Orwell) |
| **Prepared By** | GRC Team + External GRC Consultant (engaged 2025-03-10) |
| **Reviewed By** | CISO; Legal Counsel; AI Governance Committee (inaugural meeting 2025-06-01) |
| **Classification** | Internal Use: Restricted |
| **Status** | Final: Presented to AI Governance Committee 2025-06-01 |
| **Superseded By** | For ongoing operational risk assessments, see [AI System Risk Assessments](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/ai-governance/risk-assessments.md) |

---

## 1. Purpose and Context

### 1.1 Purpose

This document is the formal risk assessment of the artificial intelligence systems inherited by Emyzer Nexus through its Q4 2024 acquisition of Veridian AI. It was prepared as a required input to the AI Governance Committee's inaugural meeting (2025-06-01), where formal EU AI Act risk tier classification decisions were made for both inherited systems.

This assessment serves four functions:

1. **Classification input**: provides the risk evidence base for EU AI Act Annex III [VERIFY] risk tier classification of PCM-001 and CRT-001
2. **Gap record**: documents the governance deficiencies inherited at acquisition against Emyzer Nexus's AI governance standards
3. **Remediation baseline**: establishes the starting state against which the AI Governance Programme's progress will be measured
4. **Audit trail**: creates a permanent record of the due diligence conducted on inherited AI systems, demonstrating that Emyzer Nexus did not assume the systems' risks unknowingly

This assessment is a **one-time due diligence document**. For ongoing operational risk assessments of PCM-001 and CRT-001 under the established AI Governance Programme, see the [AI System Risk Assessments](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/ai-governance/risk-assessments.md).

### 1.2 Acquisition Context

Emyzer Technology acquired Veridian AI in Q4 2024, forming Emyzer Nexus as the post-acquisition parent entity. Veridian AI was an AI-native startup with two operational production AI systems: a Predictive Customer Churn Model (PCM-001) and an AI-Assisted Contract Review Tool (CRT-001).

At the time of acquisition close, both systems were in active production and neither had been assessed against EU AI Act requirements. Veridian AI operated without a formal GRC programme: no risk assessments, no documented governance controls, and no compliance posture for either system. The GRC obligations for both systems transferred to Emyzer Nexus on acquisition close.

The [M&A GRC Integration Charter](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/integration-management/m%26a-grc-integration-charter.md) established the governance framework for this integration. The [M&A Risk Assessment](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/integration-management/ma-risk-assessment.md) catalogues the broader GRC risks arising from the acquisition. This document focuses specifically on the AI systems.

---

## 2. Assessment Methodology

### 2.1 Base Methodology

This assessment applies the [Emyzer Technology Risk Assessment Methodology](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/risk-assessments/risk-assessment-methodology.md): a 5×5 likelihood × impact matrix producing risk scores of 1–25, with thresholds:

| Score | Rating |
|---|---|
| ≥15 | Critical |
| 10–14 | High |
| 5–9 | Medium |
| 1–4 | Low |

### 2.2 AI-Specific Methodology Extensions

The Phase 1 methodology was extended with AI-specific risk categories and assessment dimensions drawn from [NIST AI RMF 1.0](https://www.nist.gov/artificial-intelligence/ai-risk-management-framework) (MAP function) and [ISO/IEC 23894:2023](https://www.iso.org/standard/77304.html):

| AI-Specific Dimension | Description |
|---|---|
| **Regulatory compliance** | Current compliance posture against EU AI Act [VERIFY] and GDPR [VERIFY] obligations |
| **Model governance maturity** | Quality of documentation, testing, monitoring, and human oversight at time of assessment |
| **Training data governance** | Provenance, quality, consent basis, and GDPR compliance of training data |
| **Third-party dependency** | Exposure arising from reliance on external AI vendors or model APIs |
| **Explainability** | Ability of the system to provide meaningful explanations of its outputs |
| **Adversarial resilience** | Known vulnerabilities to adversarial inputs or manipulation |

### 2.3 Assessment Sources

The assessment drew on:
- Veridian AI engineering documentation obtained during due diligence
- Technical interviews with Veridian AI's former CTO, Head of Engineering, and lead ML engineer (January–February 2025)
- Review of Veridian AI's internal operational documentation (Confluence wiki, GitHub repositories)
- Legal review of Veridian AI contracts, data processing terms, and regulatory correspondence
- Output testing of both systems conducted by the external GRC consultant and Emyzer Nexus CTO (March–April 2025)

### 2.4 Governance Standards Applied

Gap analysis was conducted against Emyzer Nexus's intended AI governance standard, which is anchored to:

| Standard | Basis for Application |
|---|---|
| **[EU AI Act (Regulation 2024/1689)](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32024R1689)** [VERIFY] | Regulatory obligation; High-Risk system obligations (Articles 9–15); post-market monitoring (Article 72) |
| **[NIST AI RMF 1.0](https://www.nist.gov/artificial-intelligence/ai-risk-management-framework)** | Programme structure reference: Govern, Map, Measure, Manage |
| **[ISO/IEC 42001:2023](https://www.iso.org/standard/81230.html)** | AI management system requirements: Clause 8 operational controls |
| **[GDPR (Regulation 2016/679)](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32016R0679)** [VERIFY] | Training data governance; data processor obligations (Article 28 [VERIFY]) |
| **[AI Governance Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/enterprise-policies/ai-governance-policy.md)** | Emyzer Nexus internal standard; applied from acquisition close |

---

## 3. Inherited System Inventory

### 3.1 Systems Identified

The shadow AI discovery exercise completed 2025-05-31 confirmed that Veridian AI operated exactly two production AI systems at acquisition. Three internal ML prototypes were identified in development repositories; all were assessed as non-production and non-deployed (see Section 8).

| System ID | System Name | Type | Deployment Status at Acquisition | Business Domain |
|---|---|---|---|---|
| PCM-001 | Predictive Customer Churn Model | Traditional ML (Random Forest ensemble) | Active production | Sales and Customer Success |
| CRT-001 | AI-Assisted Contract Review Tool | LLM-based NLP | Active production | Legal: Contract Review |

### 3.2 System Profile: PCM-001 at Acquisition

| Attribute | State at Acquisition (Q4 2024) |
|---|---|
| **Architecture** | Random Forest ensemble (500 trees); supervised ML; quarterly retraining |
| **Training Data** | ~48,000 Veridian AI B2B client records; types: usage telemetry, support history, billing records, contract metadata |
| **Input Data** | Real-time client usage metrics, support ticket counts, billing status, contract tenure |
| **Output** | Churn probability score (0.00–1.00); risk tier (Low / Medium / High / Critical) |
| **Users** | ~23 Customer Success team members |
| **EU AI Act Status** | Unclassified: no conformity assessment conducted |
| **Technical Documentation** | Partial: model architecture notes in Confluence; no formal Annex IV package [VERIFY] |
| **Human Oversight** | Informal: CS managers could disregard scores but no formal override process documented |
| **Training Data Provenance** | Incomplete: original data collection consent and lawful basis not documented |
| **Monitoring** | Informal: quarterly retraining on calendar schedule; no formal drift detection |
| **Risk Assessments** | None conducted by Veridian AI |
| **Access Controls** | Veridian AI AWS tenancy; IAM access: 4 undocumented service accounts identified |
| **Third-Party Dependencies** | AWS infrastructure only; no external AI API |

### 3.3 System Profile: CRT-001 at Acquisition

| Attribute | State at Acquisition (Q4 2024) |
|---|---|
| **Architecture** | Third-party LLM API (vendor redacted) + Veridian AI custom prompting and preprocessing layer |
| **Input Data** | Contract documents (PDF/DOCX); may contain personal data and commercially sensitive information |
| **Output** | Clause-by-clause analysis; flagged anomalies; negotiation suggestions; compliance risk flags |
| **Users** | 8 Legal team members |
| **EU AI Act Status** | Unclassified: no conformity assessment conducted |
| **Technical Documentation** | Not available: Veridian AI's documentation covered only the custom prompting layer; no documentation on the underlying LLM |
| **Human Oversight** | Informal: outputs described as advisory but no formal mandatory review process documented |
| **LLM API Contract** | Contract signed with Veridian AI corporate entity only; not novated to Emyzer Nexus at acquisition close: legal basis for continued access unclear |
| **Data Processing Agreement (GDPR Art.28 [VERIFY])** | Not executed with LLM API vendor |
| **Training Data** | Unknown: entirely dependent on third-party LLM vendor's training data; provenance not available |
| **Third-Party Dependencies** | Critical: tool entirely non-functional without external LLM API; no fallback |
| **Sub-processor List** | Not obtained from LLM API vendor |
| **Monitoring** | Informal output quality review by Legal team members; no structured programme |
| **Hallucination Rate** | Not measured at acquisition; Legal team informally estimated ~5% clause-level inaccuracies |

---

## 4. Due Diligence Risk Findings

### 4.1 Risk Finding: VDA-RISK-001, EU AI Act Non-Compliance, Both Systems

| Field | Value |
|---|---|
| **Risk ID** | VDA-RISK-001 |
| **System(s)** | PCM-001 and CRT-001 |
| **Risk Category** | Regulatory Compliance |
| **Risk Owner** | CISO / Legal Counsel |
| **Risk Description** | Both systems were in active production at acquisition close without EU AI Act conformity assessments. Both exhibit characteristics consistent with High-Risk AI system classification under EU AI Act Annex III [VERIFY]. PCM-001 produces outputs that influence ongoing service access decisions for B2B clients; CRT-001 supports legal decisions with material financial consequences. Under the EU AI Act transitional provisions [VERIFY: Article 97 application timeline for systems already in service], Emyzer Nexus is now the responsible operator and must remediate the compliance deficit. Penalties for placing a High-Risk AI system in service without conformity assessment can reach €30M or 6% of global annual turnover [VERIFY: EU AI Act Article 99 penalty tiers]. |
| **Likelihood** | 4 (Likely: the non-compliance is current and confirmed; regulatory attention to AI Act implementation is increasing) |
| **Impact** | 5 (Critical: maximum penalty tier; reputational damage; potential operational suspension) |
| **Inherent Risk Rating** | **20: Critical** |
| **Interim Controls Applied** | Human oversight protocols implemented for both systems from acquisition close; formal classification process initiated |
| **Post-Control Rating** | **15: Critical** (controls reduce but do not eliminate regulatory exposure until conformity assessments are complete) |
| **Remediation Plan** | Initiate conformity assessments for both systems; target PCM-001 completion 2025-09-30; CRT-001 2025-12-31. See [EU AI Act Control Mapping](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/ai-governance/eu-ai-act-mapping.md) for detailed obligation mapping. |

---

### 4.2 Risk Finding: VDA-RISK-002, Absent Technical Documentation, Both Systems

| Field | Value |
|---|---|
| **Risk ID** | VDA-RISK-002 |
| **System(s)** | PCM-001 (partial gap); CRT-001 (critical gap) |
| **Risk Category** | Regulatory Compliance / Model Governance |
| **Risk Owner** | CTO |
| **Risk Description** | EU AI Act Article 11 [VERIFY] and Annex IV [VERIFY] require High-Risk AI systems to have complete technical documentation before deployment. Neither system had documentation meeting Annex IV standards at acquisition. PCM-001 had partial engineering notes in Confluence; CRT-001 had only the custom prompting layer documented, with no documentation of the underlying LLM's architecture, training methodology, or performance characteristics: information that is not available from the third-party API vendor. CRT-001's gap is potentially irremediable without vendor cooperation. |
| **Likelihood** | 5 (Certain: the absence of documentation is confirmed fact, not a probabilistic risk) |
| **Impact** | 4 (High: regulatory examination failure; inability to demonstrate compliance; conformity assessment blocked) |
| **Inherent Risk Rating** | **20: Critical** |
| **Interim Controls Applied** | Documentation sprint initiated; partial Veridian AI engineering documentation extracted and secured |
| **Post-Control Rating** | **15: Critical** (for CRT-001; PCM-001 reducing to High as documentation sprint progresses) |
| **Remediation Plan** | PCM-001: document sprint targeting Annex IV compliance by 2025-09-30. CRT-001: engage LLM API vendor for technical documentation cooperation; if unavailable, document the limitation with compensating controls as interim regulatory position. See [AI System Inventory](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/ai-governance/ai-system-inventory.md): CRT-001 Governance Status table. |

---

### 4.3 Risk Finding: VDA-RISK-003, GDPR Data Processing Agreement Absent, CRT-001

| Field | Value |
|---|---|
| **Risk ID** | VDA-RISK-003 |
| **System(s)** | CRT-001 |
| **Risk Category** | Data Privacy / Regulatory Compliance |
| **Risk Owner** | Data Protection Officer / Legal Counsel |
| **Risk Description** | CRT-001 transmits contract document text to an external LLM API for processing. Contract documents contain personal data (names, roles, contact details of contract parties) and commercially sensitive third-party information. Under GDPR Article 28 [VERIFY], transmission of personal data to a third-party processor requires a Data Processing Agreement (DPA) specifying processing scope, security requirements, and data subject rights support obligations. No DPA exists with the LLM API vendor. Each API call made since the tool's deployment constitutes a potentially unlawful transfer of personal data to an uncontracted processor, exposing Emyzer Nexus (as the successor entity) to enforcement action under GDPR Article 83 [VERIFY]. |
| **Likelihood** | 5 (Certain: the DPA gap is a current, confirmed compliance failure, not a future risk) |
| **Impact** | 4 (High: GDPR Article 83(4) [VERIFY] penalties up to €10M or 2% global turnover for Article 28 violations; Article 83(5) [VERIFY] up to €20M or 4% for data protection principles violations) |
| **Inherent Risk Rating** | **20: Critical** |
| **Interim Controls Applied** | Use restriction implemented 2025-01-15: CRT-001 may only process contracts containing no personal data pending DPA execution |
| **Post-Control Rating** | **16: Critical** (use restriction reduces but does not eliminate exposure; depends on operator compliance) |
| **Remediation Plan** | Execute DPA with LLM API vendor by 2025-09-30; Legal Counsel leading negotiation. Assess PII scrubbing technical feasibility as interim measure. See [AI System Risk Assessment AI-RISK-2025-007](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/ai-governance/risk-assessments.md). |

---

### 4.4 Risk Finding: VDA-RISK-004, Training Data Provenance Undocumented, PCM-001

| Field | Value |
|---|---|
| **Risk ID** | VDA-RISK-004 |
| **System(s)** | PCM-001 |
| **Risk Category** | Data Privacy / Training Data Governance |
| **Risk Owner** | Data Protection Officer |
| **Risk Description** | PCM-001's training dataset (~48,000 B2B client records) contains personal data: contact identities traceable through account IDs, individual usage behaviour records, and billing contacts. This data was collected by Veridian AI under its pre-acquisition privacy programme. No documentation was found specifying: (a) the lawful basis under GDPR Article 6 [VERIFY] for collecting this data; (b) whether the data was collected for a purpose compatible with ML model training under GDPR Article 6(4) [VERIFY]; (c) the retention schedule for the training dataset; (d) access controls on the training data store. Under GDPR Article 5(1)(b) [VERIFY], personal data must be processed for specified, explicit, and legitimate purposes. Using personal data for ML model training requires a lawful basis and compatible purpose assessment. |
| **Likelihood** | 4 (Likely: the provenance documentation does not exist; gap is confirmed) |
| **Impact** | 4 (High: regulatory enforcement; data subject rights implications; potential requirement to retrain model on compliant dataset) |
| **Inherent Risk Rating** | **16: Critical** |
| **Interim Controls Applied** | Training data access restricted to named ML engineers; DPO review initiated |
| **Post-Control Rating** | **12: High** |
| **Remediation Plan** | DPO-led data audit of PCM-001 training dataset by 2025-09-30; document lawful basis, purpose compatibility, retention schedule, and access controls; conduct DPIA before next retraining cycle. See [AI System Risk Assessment AI-RISK-2025-004](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/ai-governance/risk-assessments.md). |

---

### 4.5 Risk Finding: VDA-RISK-005, LLM API Contract Not Novated, CRT-001

| Field | Value |
|---|---|
| **Risk ID** | VDA-RISK-005 |
| **System(s)** | CRT-001 |
| **Risk Category** | Third-Party / Contractual |
| **Risk Owner** | Legal Counsel / Vendor Risk Manager |
| **Risk Description** | The LLM API contract was signed between the vendor and Veridian AI's corporate entity, which no longer exists as a separate contracting party post-acquisition. No contract novation to Emyzer Nexus was completed at acquisition close. Emyzer Nexus is therefore accessing the LLM API on informal terms: there is no enforceable contractual relationship between Emyzer Nexus and the API vendor. This means Emyzer Nexus has no contractual SLA, no right to audit, no data protection obligations on the vendor's part, no defined incident notification requirements, and no model continuity commitment. Access could be revoked at any time. |
| **Likelihood** | 2 (Unlikely: vendor is operational and the service continues; but the legal exposure is immediate) |
| **Impact** | 4 (High: tool becomes entirely non-functional if access revoked; legal exposure from no-contract operation; no remedies available if vendor fails) |
| **Inherent Risk Rating** | **8: Medium** |
| **Interim Controls Applied** | Manual contract review fallback available (Legal team) |
| **Post-Control Rating** | **8: Medium** |
| **Remediation Plan** | Complete contract novation from Veridian AI to Emyzer Nexus by 2025-03-31 (urgent). Negotiate formal SLA including API availability commitment and model continuity notice period. See [AI System Risk Assessment AI-RISK-2025-006](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/ai-governance/risk-assessments.md). |

---

### 4.6 Risk Finding: VDA-RISK-006, No Formal Human Oversight Protocol, Both Systems

| Field | Value |
|---|---|
| **Risk ID** | VDA-RISK-006 |
| **System(s)** | PCM-001 and CRT-001 |
| **Risk Category** | Model Governance / Regulatory Compliance |
| **Risk Owner** | AI System Owners (VP Customer Success; General Counsel) |
| **Risk Description** | EU AI Act Article 14 [VERIFY] requires High-Risk AI systems to incorporate human oversight measures enabling operators to monitor, understand, intervene, override, and halt the system. At acquisition, neither system had a documented human oversight protocol. For PCM-001, CS managers informally reviewed scores before acting, but there was no documented override procedure, no escalation path, and no training on the system's limitations. For CRT-001, Legal team members informally treated outputs as advisory, but there was no formal mandatory review procedure, no documentation of the advisory-only status, and no training covering hallucination risk or override obligations. |
| **Likelihood** | 4 (Likely: the absence of formal oversight protocols creates ongoing non-compliance) |
| **Impact** | 3 (Moderate: operational risk from over-reliance on AI outputs; regulatory risk from missing Article 14 controls) |
| **Inherent Risk Rating** | **12: High** |
| **Interim Controls Applied** | Informal review practices in place |
| **Post-Control Rating** | **9: Medium** |
| **Remediation Plan** | Document formal human oversight protocols for both systems; complete operator training incorporating override requirements; deploy training through LMS before Q2 2025. |

---

### 4.7 Risk Finding: VDA-RISK-007, Absent Performance Monitoring, Both Systems

| Field | Value |
|---|---|
| **Risk ID** | VDA-RISK-007 |
| **System(s)** | PCM-001 and CRT-001 |
| **Risk Category** | Model Governance / Post-Market Monitoring |
| **Risk Owner** | CTO / AI System Owners |
| **Risk Description** | EU AI Act Article 72 [VERIFY] requires providers and deployers of High-Risk AI systems to maintain a post-market monitoring system collecting, documenting, and analysing data on performance in deployment. At acquisition, Veridian AI had no formal post-market monitoring programme for either system. PCM-001 was retrained quarterly on a calendar schedule with no formal drift detection. CRT-001 had no output quality tracking, no hallucination rate measurement, and no structured feedback collection from Legal team users. The absence of baseline performance data means Emyzer Nexus cannot demonstrate regulatory compliance for the period before the AI Governance Programme was established. |
| **Likelihood** | 5 (Certain: the monitoring gap is confirmed) |
| **Impact** | 3 (Moderate: regulatory non-compliance for pre-programme period; operational risk from undetected model degradation) |
| **Inherent Risk Rating** | **15: Critical** |
| **Interim Controls Applied** | Informal monitoring practices partially fill the gap |
| **Post-Control Rating** | **12: High** |
| **Remediation Plan** | Establish formal post-market monitoring plans for both systems as first action of AI Governance Programme; create performance baselines by 2025-07-01; retroactively document pre-programme monitoring limitations for regulatory record. |

---

### 4.8 Risk Finding: VDA-RISK-008: Shadow AI Discovery Required

| Field | Value |
|---|---|
| **Risk ID** | VDA-RISK-008 |
| **System(s)** | Veridian AI estate (all systems) |
| **Risk Category** | Integration Governance / Regulatory Compliance |
| **Risk Owner** | CTO / CISO |
| **Risk Description** | Veridian AI had no AI system inventory. Due diligence identified PCM-001 and CRT-001 as the primary operational systems, but without a comprehensive inventory, the possibility of additional deployed or semi-deployed AI systems creating undisclosed EU AI Act obligations could not be excluded at acquisition close. Veridian AI's engineering culture was rapid-iteration: prototype ML tools were commonly built and sometimes deployed to production without formal registration. |
| **Likelihood** | 3 (Possible: Veridian AI's culture was consistent with undisclosed prototypes; probability decreasing as engineering documentation reviewed) |
| **Impact** | 4 (High: undisclosed High-Risk AI systems would create immediate conformity obligations and could materially change the acquisition risk profile) |
| **Inherent Risk Rating** | **12: High** |
| **Interim Controls Applied** | Engineering repository review underway; former Veridian AI engineers interviewed |
| **Post-Control Rating** | **6: Medium** (reducing as review progresses) |
| **Remediation Plan** | Complete shadow AI discovery exercise by 2025-05-31; review all Veridian AI engineering repositories, AWS deployment records, and SaaS subscriptions. Establish mandatory AI system registration process going forward under AI Governance Policy. |
| **Resolution** | Discovery exercise completed 2025-05-31. Three internal ML prototypes identified: assessed as non-production, non-deployed, and not requiring EU AI Act classification. Prototypes archived and documented. **Risk closed.** |

---

## 5. Gap Analysis Against Emyzer Nexus AI Governance Standards

### 5.1 Gap Summary Matrix

The following matrix maps each EU AI Act High-Risk system obligation against the state found at acquisition for both systems.

| Obligation | Standard | PCM-001 State at Acquisition | CRT-001 State at Acquisition | Gap Severity |
|---|---|---|---|---|
| Risk management system (Art.9 [VERIFY]) | Documented, implemented, maintained | Not established | Not established | Critical |
| Data governance (Art.10 [VERIFY]) | Training data documented; provenance verified; bias examined | Partial documentation; provenance incomplete; no bias testing | Training data unknown (third-party LLM) | Critical |
| Technical documentation (Art.11 [VERIFY]) | Complete Annex IV package | Engineering notes only; Annex IV not met | Prompting layer only; LLM technical docs unavailable | Critical |
| Transparency to deployers (Art.13 [VERIFY]) | Instructions for use; accuracy disclosure; limitation disclosure | Informal operator guides; no accuracy disclosure | Informal guidance; no structured limitation disclosure | High |
| Human oversight (Art.14 [VERIFY]) | Documented override procedure; halt capability; operator training | Informal practice; no documentation; no formal training | Informal advisory use; no documented procedure | High |
| Accuracy and robustness (Art.15 [VERIFY]) | Declared performance; adversarial resilience assessed | Performance not formally declared; no adversarial testing | Performance not declared; third-party LLM not testable | High |
| Post-market monitoring (Art.72 [VERIFY]) | Monitoring plan; data collection; anomaly reporting | Calendar retraining only; no monitoring programme | No monitoring programme | Critical |
| Serious incident reporting (Art.73 [VERIFY]) | Reporting procedure; records maintained | No procedure | No procedure | High |
| EU AI Act risk classification | Formal classification with documented rationale | None | None | Critical |
| GDPR data processor agreement (Art.28 [VERIFY]) | DPA with all data processors | N/A (no external processor) | DPA absent | Critical |
| AI system inventory | Registered in AI system inventory | Not registered | Not registered | High |

**Critical gaps: 6 (across both systems). High gaps: 5.** No obligations were partially or fully met at acquisition.

### 5.2 Governance Maturity Assessment

Veridian AI's AI governance maturity was assessed using a five-level model:

| Level | Description | Assessment |
|---|---|---|
| 5: Optimising | Continuous improvement; proactive compliance; leading practice | — |
| 4: Managed | Quantitative management; metrics-driven; audit-ready | — |
| 3: Defined | Documented processes; training; consistent application | — |
| 2: Developing | Some documented processes; inconsistent application | — |
| **1: Initial** | Ad hoc; undocumented; reliant on individual knowledge | **PCM-001 and CRT-001** |

**Overall maturity: Level 1: Initial.** Both systems relied entirely on informal practices and individual knowledge within Veridian AI's small team. No documented controls, no formal compliance posture, no risk management programme.

The Emyzer Nexus AI Governance Programme is designed to advance both systems to Level 3 (Defined) by end of 2025 and Level 4 (Managed) by mid-2026.

---

## 6. EU AI Act Risk Tier Classification Recommendation

Based on the due diligence findings above, the GRC Team recommends **High-Risk classification under EU AI Act Annex III** for both PCM-001 and CRT-001 on the following basis:

### 6.1 PCM-001: Recommended: High-Risk

PCM-001 produces outputs that influence ongoing service access decisions for B2B clients. Clients scoring in the High and Critical churn risk tiers are subject to proactive outreach that may include contract renegotiation and pricing adjustment. The system's outputs therefore materially influence business decisions affecting clients' continued access to services. The AI Governance Committee is invited to assess applicability of Annex III §5(b) [VERIFY: B2B creditworthiness / service access context] and confirm classification rationale.

**[VERIFY: Legal Counsel to confirm Annex III category and whether B2B service access decisions fall within the spirit of §5(b) or another applicable category. Classification to be revisited if implementing acts provide clarifying guidance.]**

### 6.2 CRT-001: Recommended: High-Risk (Precautionary)

CRT-001 supports legal decisions with material financial and operational consequences. The tool's outputs directly inform contract acceptance and negotiation positions worth potentially hundreds of thousands of euros. The AI Governance Committee may elect voluntary High-Risk classification under the precautionary principle if Annex III does not directly apply [VERIFY: EU AI Act Article 6 treatment of voluntary High-Risk classification]. Note: voluntary High-Risk classification triggers the full conformity obligation suite.

**[VERIFY: Legal Counsel to assess whether CRT-001 falls within an Annex III category or whether the High-Risk classification is precautionary under Article 6.]**

Both recommendations were presented to the AI Governance Committee at its inaugural meeting (2025-06-01). Both systems were formally classified as High-Risk at that meeting (see [AI System Inventory and Classification Register](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/ai-governance/ai-system-inventory.md), Section 5: Classification History).

---

## 7. Remediation Plan

The following remediation plan translates the gap analysis into an action programme. Ownership and target dates reflect commitments confirmed by the Integration Management Committee.

| Action ID | Action | Gap Addressed | Owner | Target Date | Status (as of 2025-05-30) |
|---|---|---|---|---|---|
| REM-001 | Formally classify PCM-001 and CRT-001 under EU AI Act | VDA-RISK-001 | AI Governance Committee | 2025-06-01 | On track: inaugural AI Governance Committee meeting scheduled |
| REM-002 | Implement formal human oversight protocols and operator training for both systems | VDA-RISK-006 | VP Customer Success / General Counsel | 2025-06-30 | In Progress: protocols drafted; training module in development |
| REM-003 | Initiate PCM-001 technical documentation sprint (Annex IV) | VDA-RISK-002 | CTO / VP Customer Success | 2025-07-01 | In Progress: documentation sprint commenced |
| REM-004 | Complete contract novation of LLM API agreement to Emyzer Nexus | VDA-RISK-005 | Legal Counsel | 2025-03-31 | **Overdue**: vendor unresponsive; escalated to CRO |
| REM-005 | Execute GDPR Article 28 DPA with LLM API vendor | VDA-RISK-003 | Legal Counsel | 2025-09-30 | In Progress: DPA negotiation linked to novation; delayed |
| REM-006 | Implement CRT-001 use restriction (no PII contracts) pending DPA | VDA-RISK-003 | General Counsel | 2025-01-15 | **Complete**: restriction implemented 2025-01-15 |
| REM-007 | DPO audit of PCM-001 training data (provenance, lawful basis, retention, access) | VDA-RISK-004 | Data Protection Officer | 2025-09-30 | In Progress: DPO review initiated |
| REM-008 | Establish formal post-market monitoring plans for PCM-001 and CRT-001 | VDA-RISK-007 | CTO / AI System Owners | 2025-07-01 | In Progress: monitoring framework being designed |
| REM-009 | Complete shadow AI discovery exercise | VDA-RISK-008 | CTO | 2025-05-31 | **Complete**: no additional systems found; prototypes archived |
| REM-010 | Engage LLM API vendor for technical documentation cooperation (Art.11 compliance) | VDA-RISK-002 | General Counsel / CTO | 2025-09-30 | In Progress: vendor engagement initiated |
| REM-011 | Establish AI Governance Programme and AI Governance Committee | All gaps | CISO | 2025-06-01 | On track |

---

## 8. Shadow AI Discovery: Summary of Findings

The shadow AI discovery exercise identified three internal ML prototypes in Veridian AI's engineering repositories. None required EU AI Act classification action:

| Prototype ID | Description | Deployment Status | EU AI Act Classification Required | Disposition |
|---|---|---|---|---|
| PROTO-001 | Internal sales lead scoring model | Development only: never deployed | No: not in service | Archived; not to be deployed without AI Governance Committee review |
| PROTO-002 | Automated email categorisation for support tickets | Tested internally; never deployed to production | No: not in service | Archived; redeployment would trigger classification review |
| PROTO-003 | Exploratory NLP model for contract clause extraction | Prototype stage; used by one engineer for research | No: single-user research tool | Archived; not to be deployed without AI Governance Committee review |

**Conclusion:** No additional EU AI Act classification obligations arise from the shadow AI discovery exercise beyond PCM-001 and CRT-001.

---

## 9. Risk Summary

| Risk ID | System | Risk Title | Rating (Inherent) | Rating (Post-Control) | Treatment Status |
|---|---|---|---|---|---|
| VDA-RISK-001 | Both | EU AI Act Non-Compliance | 20: Critical | 15: Critical | In Treatment (conformity assessments initiated) |
| VDA-RISK-002 | Both | Absent Technical Documentation | 20: Critical | 15, Critical (CRT-001) / 10, High (PCM-001) | In Treatment |
| VDA-RISK-003 | CRT-001 | GDPR DPA Absent | 20: Critical | 16: Critical | In Treatment (use restriction in place; DPA negotiation) |
| VDA-RISK-004 | PCM-001 | Training Data Provenance Undocumented | 16: Critical | 12: High | In Treatment (DPO review) |
| VDA-RISK-005 | CRT-001 | LLM API Contract Not Novated | 8: Medium | 8: Medium | In Treatment (overdue) |
| VDA-RISK-006 | Both | No Formal Human Oversight Protocol | 12: High | 9: Medium | In Treatment |
| VDA-RISK-007 | Both | Absent Performance Monitoring | 15: Critical | 12: High | In Treatment |
| VDA-RISK-008 | Estate | Shadow AI Discovery Required | 12: High | — | **Closed** (discovery complete; no additional systems) |

**Critical risks at assessment close: 4.** All critical risks are in active treatment with assigned owners and target dates. Risk VDA-RISK-008 is closed.

These risks transition to the [AI System Risk Assessments](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/ai-governance/risk-assessments.md) programme for ongoing tracking under the established AI Governance Programme. The ongoing assessments reflect post-classification risk ratings and current treatment progress.

---

## 10. Document Control

| Version | Date | Author | Changes |
|---|---|---|---|
| 1.0 | 2025-05-30 | GRC Team + External GRC Consultant | Initial publication: presented to AI Governance Committee 2025-06-01 |

- **Document ID:** VDA-RA-2025-001
- **Classification:** Internal Use: Restricted
- **Retention:** Indefinite (acquisition due diligence record)
- **Related Documents:** [AI System Inventory](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/ai-governance/ai-system-inventory.md) | [AI System Risk Assessments](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/ai-governance/risk-assessments.md) | [EU AI Act Control Mapping](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/ai-governance/eu-ai-act-mapping.md) | [M&A Risk Assessment](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/integration-management/ma-risk-assessment.md)

---

*This document was developed as part of the Emyzer Nexus Phase 2 GRC Programme and formatted for portfolio presentation. All individuals, systems, and risk findings are fictional.*

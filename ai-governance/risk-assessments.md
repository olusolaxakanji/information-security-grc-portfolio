# AI System Risk Assessments

**Emyzer Nexus: AI Governance Programme**

---

## Document Information

| Attribute | Value |
|---|---|
| **Document ID** | AI-RA-2025-001/002 |
| **Document Type** | AI System Risk Assessment |
| **Version** | 1.0 |
| **Effective Date** | 2025-07-01 |
| **Owner** | AI Governance Committee / CISO |
| **Classification** | Internal Use |
| **Systems Assessed** | PCM-001 (Predictive Customer Churn Model); CRT-001 (AI-Assisted Contract Review Tool) |

---

## 1. Methodology

These assessments apply the [Emyzer Technology Risk Assessment Methodology](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/risk-assessments/risk-assessment-methodology.md) (5×5 likelihood × impact matrix; scores 1–25; Critical ≥15, High 10–14, Medium 5–9, Low 1–4) extended with AI-specific risk categories not addressed in the Phase 1 methodology.

### AI-Specific Risk Extensions

| AI Risk Category | Description |
|---|---|
| **Model Drift** | Degradation in model performance over time due to changes in underlying data distribution; predictions or outputs no longer reflect current conditions |
| **Training Data Bias** | Systematic errors in outputs caused by imbalances, exclusions, or historical prejudices in training data |
| **Explainability Gap** | Inability to provide meaningful explanations of individual outputs to affected parties; governance and regulatory risk |
| **Third-Party Model Dependency** | Risk of service disruption, quality degradation, or compliance failure arising from reliance on an external AI vendor's model |
| **Adversarial Manipulation** | Deliberate manipulation of model inputs to produce incorrect or malicious outputs; includes prompt injection for LLM-based systems |
| **Data Privacy (AI-specific)** | Privacy risks specific to AI system operation: training data containing PII, inference data transmitted to external vendors, outputs that reveal training data |

---

## 2. Risk Assessment: PCM-001: Predictive Customer Churn Model

### AI-RISK-2025-001 | Model Drift

| Field | Value |
|---|---|
| **Risk ID** | AI-RISK-2025-001 |
| **Asset / System** | PCM-001: Predictive Customer Churn Model |
| **Risk Category** | Model Drift |
| **Asset Owner** | VP, Customer Success |
| **Risk Owner** | VP, Customer Success |
| **Risk Description** | The PCM-001 model is retrained on a quarterly cycle. In the intervals between retraining cycles, changes in client behavior patterns, driven by product updates, market conditions, or the integration of Emyzer Technology's legacy client base, may cause model predictions to degrade without detection. If CS teams act on degraded predictions, high-churn-risk clients may be missed while low-risk clients receive unnecessary outreach, reducing retention programme effectiveness and wasting CS capacity. |
| **Threat Source** | Structural: data distribution shift; environmental: post-acquisition client mix change |
| **Vulnerability** | Quarterly retraining cycle creates a detection lag; drift monitoring thresholds may not be sensitive enough to catch gradual degradation |
| **Likelihood** | 3 (Possible) |
| **Impact** | 4 (High): missed churn could result in material revenue loss from churned accounts; reputational impact if systematic drift is discovered in retrospect |
| **Risk Rating** | **12: High** |
| **Existing Controls** | Quarterly retraining; performance monitoring against held-out validation set; CS manager review of flagged accounts before action |
| **Control Effectiveness** | Moderate: retraining addresses drift after the fact; validation set may not reflect new client segments |
| **Treatment Strategy** | Mitigate |
| **Treatment Status** | In Treatment |
| **Target Date** | 2025-09-30 |
| **Review Date** | 2025-Q4 |
| **Comments** | Remediation: (1) implement real-time drift detection metrics (PSI: Population Stability Index) with alert threshold set at PSI >0.2; (2) expand validation set to include representative Emyzer Technology legacy client records; (3) add drift detection trigger to retraining criteria (current: calendar-only; target: calendar + drift threshold). Estimated timeline: PSI monitoring implementation by 2025-09-30. |

---

### AI-RISK-2025-002 | Training Data Bias

| Field | Value |
|---|---|
| **Risk ID** | AI-RISK-2025-002 |
| **Asset / System** | PCM-001: Predictive Customer Churn Model |
| **Risk Category** | Training Data Bias |
| **Asset Owner** | VP, Customer Success |
| **Risk Owner** | AI Governance Committee |
| **Risk Description** | PCM-001 was trained entirely on Veridian AI's historical client base, approximately 48,000 B2B records from Veridian AI's SaaS-native clients. Emyzer Technology's existing client base spans hardware, managed services, and enterprise support, materially different purchasing behaviors, support patterns, and churn drivers. The model has not been validated on Emyzer Technology client data and may systematically misclassify clients in these segments. Overestimating churn risk for hardware clients (higher support ticket rates are normal for their profile) or underestimating it for managed services clients could both cause harm. |
| **Threat Source** | Structural: training data scope; historical: Veridian AI client base not representative of full Emyzer Nexus population |
| **Vulnerability** | Training data does not represent full intended deployment population; no cross-segment validation completed |
| **Likelihood** | 3 (Possible) |
| **Impact** | 3 (Moderate): retention programme misdirection; operational efficiency loss; potential reputational impact if misclassification pattern identified by clients |
| **Risk Rating** | **9: Medium** |
| **Existing Controls** | CS manager review before outreach; managers can override scores based on client knowledge |
| **Control Effectiveness** | Moderate: human review compensates but relies on CS manager familiarity with each client |
| **Treatment Strategy** | Mitigate |
| **Treatment Status** | In Treatment |
| **Target Date** | 2025-12-31 |
| **Review Date** | 2025-Q4 |
| **Comments** | Remediation: (1) cross-segment performance analysis: compare PCM-001 predictions against actual churn outcomes for Emyzer Technology legacy clients over the next two quarters; (2) if material bias confirmed, supplement training data with Emyzer Technology client records at next retraining cycle; (3) in the interim, CS managers for Emyzer Technology legacy accounts are briefed on coverage limitation. Bias audit to be completed by AI Governance Committee Q3 2025. |

---

### AI-RISK-2025-003 | Explainability Gap

| Field | Value |
|---|---|
| **Risk ID** | AI-RISK-2025-003 |
| **Asset / System** | PCM-001: Predictive Customer Churn Model |
| **Risk Category** | Explainability Gap |
| **Asset Owner** | VP, Customer Success |
| **Risk Owner** | AI Governance Committee / Legal Counsel |
| **Risk Description** | PCM-001's Random Forest ensemble architecture cannot generate per-client explanations for assigned churn scores. A CS manager who calls an at-risk client cannot explain why the client was flagged: they can only say "our systems identified you as at risk." If a client requests an explanation (which would be reasonable given the potential impact on contract negotiations), Emyzer Nexus cannot provide one. Under GDPR Article 22 [VERIFY], if the model's outputs are considered to constitute automated decision-making with significant effects on individuals (in a B2B context, this applies to the company representatives affected by the decisions), there may be an obligation to provide meaningful information about the logic involved. This regulatory risk is uncertain pending Legal Counsel assessment. |
| **Threat Source** | Technical: model architecture; regulatory: GDPR automated decision-making provisions [VERIFY] |
| **Vulnerability** | Random Forest ensemble is inherently non-explainable at individual prediction level; no SHAP or similar interpretability layer implemented |
| **Likelihood** | 4 (Likely: clients can reasonably ask; regulatory scrutiny is increasing) |
| **Impact** | 3 (Moderate: reputational; regulatory risk uncertain but real) |
| **Risk Rating** | **12: High** |
| **Existing Controls** | Operator training includes acknowledgement of explainability limitation; GDPR Article 22 [VERIFY] assessment initiated with DPO |
| **Control Effectiveness** | Partial: awareness exists; structural gap remains |
| **Treatment Strategy** | Mitigate |
| **Treatment Status** | In Treatment |
| **Target Date** | 2025-12-31 |
| **Review Date** | 2025-Q4 |
| **Comments** | Remediation options: (1) implement SHAP (SHapley Additive exPlanations) analysis layer to generate approximate per-prediction feature importance scores at inference time: technical feasibility confirmed, development estimate 6–8 weeks; (2) pending SHAP implementation, document a client-facing narrative template explaining the general factors the model uses; (3) Legal Counsel to confirm GDPR Article 22 [VERIFY] applicability and, if applicable, the appropriate legal basis for automated processing. SHAP implementation targeted Q4 2025. |

---

### AI-RISK-2025-004 | Training Data PII Governance

| Field | Value |
|---|---|
| **Risk ID** | AI-RISK-2025-004 |
| **Asset / System** | PCM-001: Predictive Customer Churn Model |
| **Risk Category** | Data Privacy (AI-specific) |
| **Asset Owner** | VP, Customer Success |
| **Risk Owner** | Data Protection Officer |
| **Risk Description** | PCM-001 training data includes client account records containing personal data: individual contact names (via account IDs traceable to named contacts), usage behavior attributable to named individuals within client organisations, and billing records linked to named account managers. This personal data was collected by Veridian AI under its pre-acquisition privacy programme. The lawful basis for using this data to train a machine learning model, the retention schedule for training data, and the access controls on the training dataset have not been reviewed since acquisition. Under GDPR Article 5 [VERIFY], personal data must be processed lawfully and for a specified, explicit, and legitimate purpose. Training data re-use must be assessed for compatibility with the original collection purpose [VERIFY: GDPR Article 6(4) compatibility assessment]. |
| **Threat Source** | Regulatory: GDPR obligations; structural: inherited data governance gap |
| **Vulnerability** | Pre-acquisition data governance documentation not reviewed; retention schedule not documented; access controls not audited |
| **Likelihood** | 3 (Possible) |
| **Impact** | 4 (High: GDPR enforcement action possible; reputational damage; data subject rights implications) |
| **Risk Rating** | **12: High** |
| **Existing Controls** | Training data stored in secured AWS environment; access restricted to ML engineering team |
| **Control Effectiveness** | Partial: security controls exist; legal basis and governance documentation gaps unaddressed |
| **Treatment Strategy** | Mitigate |
| **Treatment Status** | In Treatment |
| **Target Date** | 2025-09-30 |
| **Review Date** | 2025-Q3 |
| **Comments** | Remediation: (1) DPO-led data audit of PCM-001 training dataset: document data types, legal basis, retention schedule, and access controls; (2) where legal basis is uncertain, assess anonymisation or pseudonymisation options for training data; (3) where personal data cannot be justified, plan for dataset refresh using appropriately governed data collection; (4) DPIA to be completed before next retraining cycle. Target completion: 2025-09-30. Interim: training data access restricted to named ML engineers only. |

---

## 3. Risk Assessment: CRT-001: AI-Assisted Contract Review Tool

### AI-RISK-2025-005 | LLM Hallucination Risk

| Field | Value |
|---|---|
| **Risk ID** | AI-RISK-2025-005 |
| **Asset / System** | CRT-001: AI-Assisted Contract Review Tool |
| **Risk Category** | Model Accuracy / AI-specific |
| **Asset Owner** | General Counsel |
| **Risk Owner** | General Counsel |
| **Risk Description** | CRT-001 is powered by a third-party large language model that can generate confident, fluent, and plausible but factually incorrect legal analysis, commonly known as hallucination. The model may mischaracterise contract clauses, invent legal obligations not present in the contract, miss obligations that are present, or suggest negotiation positions inconsistent with applicable law. If Legal team members rely on CRT-001 analysis without adequate scrutiny, material contracts could be mischaracterised, creating financial exposure, unmet obligations, or regulatory risk. The risk is elevated because the model's outputs are syntactically authoritative, they do not look uncertain even when incorrect. |
| **Threat Source** | Technical: LLM architecture inherent limitation; operational: over-reliance on AI-generated analysis |
| **Vulnerability** | Third-party LLM architecture prone to confident hallucination; no hallucination detection mechanism; reliance risk if operators become complacent |
| **Likelihood** | 3 (Possible: hallucinations occur in LLMs even with careful prompting; Legal team using tool under workload pressure) |
| **Impact** | 5 (Critical: material contract mischaracterisation could result in significant financial loss, legal liability, or regulatory breach) |
| **Risk Rating** | **15: Critical** |
| **Existing Controls** | Mandatory solicitor review of all CRT-001 outputs; operator training includes hallucination awareness; all outputs explicitly labelled as draft/advisory in the tool interface |
| **Control Effectiveness** | Moderate: mandatory review is the primary control; effectiveness depends on reviewer attentiveness and time available |
| **Treatment Strategy** | Mitigate |
| **Treatment Status** | In Treatment |
| **Target Date** | Ongoing: control is the mandatory review; additional mitigations by 2025-12-31 |
| **Review Date** | 2025-Q4 |
| **Comments** | Primary control: mandatory solicitor review before acting on any CRT-001 output: this control must be maintained indefinitely and is non-negotiable. Secondary mitigations: (1) implement structured review checklist prompting reviewers to cross-check flagged clauses against contract source text; (2) establish hallucination rate tracking through quarterly random output audits (20 contracts per quarter, reviewed by senior solicitor against source documents); (3) explore vendor-provided hallucination mitigation features (grounding, retrieval-augmented generation); (4) assess whether prompting improvements can reduce hallucination frequency. Current tracked hallucination rate: 4.2% of clauses per quarterly audit Q1 2025. |

---

### AI-RISK-2025-006 | Third-Party Model Dependency

| Field | Value |
|---|---|
| **Risk ID** | AI-RISK-2025-006 |
| **Asset / System** | CRT-001: AI-Assisted Contract Review Tool |
| **Risk Category** | Third-Party Model Dependency |
| **Asset Owner** | General Counsel |
| **Risk Owner** | Vendor Risk Manager |
| **Risk Description** | CRT-001 is entirely dependent on an external LLM API. If the API vendor discontinues the service, changes its pricing to an uneconomic level, suffers an extended outage, or revokes Emyzer Nexus's API access, CRT-001 becomes entirely non-functional. There is currently no contractual SLA guaranteeing model continuity, and the API contract was not novated from Veridian AI to Emyzer Nexus at acquisition: creating a further risk that Emyzer Nexus's continued API access is on informal terms only. |
| **Threat Source** | Structural: single vendor dependency; contractual: novation not completed |
| **Vulnerability** | No contractual continuity guarantee; no fallback AI service identified; contract novation outstanding |
| **Likelihood** | 2 (Unlikely: vendor is operational and the service is commercial; but novation gap is immediately remedied) |
| **Impact** | 4 (High: Legal team would revert to fully manual contract review, significantly increasing turnaround time and cost) |
| **Risk Rating** | **8: Medium** |
| **Existing Controls** | Legal team has manual review capability as fallback; tool disruption would be operationally painful but not a compliance risk in itself |
| **Control Effectiveness** | Moderate: fallback exists but is costly |
| **Treatment Strategy** | Mitigate |
| **Treatment Status** | In Treatment |
| **Target Date** | 2025-06-30 (novation); 2025-09-30 (SLA) |
| **Review Date** | 2025-Q3 |
| **Comments** | Remediation: (1) complete contract novation from Veridian AI to Emyzer Nexus: urgent; (2) negotiate SLA covering API availability (target: 99.5% monthly) and model continuity notice period (target: 6 months notice before discontinuation); (3) identify alternative LLM API provider as contingency option; (4) document manual contract review fallback procedure. Priority: novation is the most urgent action (legal exposure risk if access is on informal basis). |

---

### AI-RISK-2025-007 | Data Privacy: External API Transmission

| Field | Value |
|---|---|
| **Risk ID** | AI-RISK-2025-007 |
| **Asset / System** | CRT-001: AI-Assisted Contract Review Tool |
| **Risk Category** | Data Privacy (AI-specific) |
| **Asset Owner** | General Counsel |
| **Risk Owner** | Data Protection Officer |
| **Risk Description** | CRT-001 ingests contract documents and transmits their text to an external LLM API for processing. Contract documents contain commercially sensitive information (financial terms, strategic commitments, party details) and personal data (names, roles, and contact details of individuals named in contracts). Transmitting this data to an external third party requires a Data Processing Agreement (DPA) meeting GDPR Article 28 [VERIFY] requirements. No DPA has been executed with the LLM API vendor. Without a DPA, each API call constitutes an unlawful transfer of personal data to a data processor, potentially triggering GDPR enforcement under Article 83 [VERIFY]. |
| **Threat Source** | Regulatory: GDPR enforcement; contractual: no DPA in place |
| **Vulnerability** | No DPA with external API vendor; personal data transmitted without adequate processor agreement |
| **Likelihood** | 4 (Likely: the absence of a DPA is not a probabilistic risk; it is a current compliance gap with ongoing enforcement exposure) |
| **Impact** | 4 (High: GDPR enforcement up to €20M or 4% global annual turnover for Article 83(4) [VERIFY] violations; regulatory notification obligation if breach occurs) |
| **Risk Rating** | **16: Critical** |
| **Existing Controls** | Use restriction implemented: CRT-001 may only process contracts containing no personal data or commercially sensitive third-party information pending DPA execution; operator training includes the use restriction |
| **Control Effectiveness** | Moderate: use restriction reduces but does not eliminate exposure; compliance depends on operator adherence |
| **Treatment Strategy** | Mitigate |
| **Treatment Status** | In Treatment: DPA negotiation in progress |
| **Target Date** | 2025-09-30 |
| **Review Date** | 2025-Q3 |
| **Comments** | Remediation: (1) execute DPA with LLM API vendor: Legal Counsel leading negotiation; target 2025-09-30; (2) pending DPA, maintain and enforce use restriction; (3) assess whether PII scrubbing (removing names and contact details from contract text before API submission) is technically feasible as an interim measure: CTO assessment requested; (4) review vendor sub-processor list upon receipt to assess adequacy of sub-processor controls. This is the highest-priority remediation item in the CRT-001 risk profile. |

---

### AI-RISK-2025-008 | Prompt Injection

| Field | Value |
|---|---|
| **Risk ID** | AI-RISK-2025-008 |
| **Asset / System** | CRT-001: AI-Assisted Contract Review Tool |
| **Risk Category** | Adversarial Manipulation |
| **Asset Owner** | General Counsel |
| **Risk Owner** | CTO / Information Security Officer |
| **Risk Description** | A sophisticated counterparty could embed instructions within a contract document designed to manipulate CRT-001's LLM outputs. For example, a contract might contain hidden text (white-on-white, micro-font, or metadata-embedded) instructing the LLM to mark all clauses as acceptable, suppress risk flags, or generate analysis favourable to the counterparty. Because CRT-001's preprocessing pipeline ingests document text and submits it to the LLM as part of the prompt context, malicious content within the document could interfere with the system prompt and override intended behavior. This is a known class of LLM vulnerability (indirect prompt injection). The probability is currently assessed as low, it requires a sophisticated and deliberate counterparty, but the impact of a successful attack would be high. |
| **Threat Source** | Adversarial: sophisticated counterparty deliberately embedding prompt injection instructions in contract documents |
| **Vulnerability** | Input sanitisation not yet implemented; document text submitted to LLM in full without malicious instruction screening |
| **Likelihood** | 2 (Unlikely: requires deliberate, sophisticated attack by a counterparty aware of Emyzer Nexus's use of AI contract review) |
| **Impact** | 3 (Moderate: manipulated output would be caught by mandatory solicitor review in most cases; risk of bypass if reviewer is under time pressure) |
| **Risk Rating** | **6: Medium** |
| **Existing Controls** | Mandatory solicitor review provides primary protection: a reviewer comparing AI output to source contract would typically detect implausible analysis; operator awareness training |
| **Control Effectiveness** | Moderate: mandatory review catches most attacks; sophisticated attacks designed to be subtle may evade detection |
| **Treatment Strategy** | Mitigate |
| **Treatment Status** | In Treatment |
| **Target Date** | 2025-09-30 |
| **Review Date** | 2025-Q4 |
| **Comments** | Remediation: (1) implement input sanitisation in the preprocessing pipeline: scan for anomalous text patterns (ultra-low-opacity text, metadata embedding, instruction-like language in unusual positions); (2) implement a system prompt hardening approach isolating document content from instruction context; (3) include prompt injection awareness in operator training refresh (already planned for Q3 2025); (4) CTO to assess vendor-provided injection mitigation capabilities. Input sanitisation development in progress; target: 2025-09-30. |

---

## 4. Risk Summary

| Risk ID | System | Risk Title | Category | Rating | Treatment Status |
|---|---|---|---|---|---|
| AI-RISK-2025-001 | PCM-001 | Model Drift | Model Drift | **12: High** | In Treatment |
| AI-RISK-2025-002 | PCM-001 | Training Data Bias | Training Data Bias | **9: Medium** | In Treatment |
| AI-RISK-2025-003 | PCM-001 | Explainability Gap | Explainability Gap | **12: High** | In Treatment |
| AI-RISK-2025-004 | PCM-001 | Training Data PII Governance | Data Privacy | **12: High** | In Treatment |
| AI-RISK-2025-005 | CRT-001 | LLM Hallucination Risk | Model Accuracy | **15: Critical** | In Treatment |
| AI-RISK-2025-006 | CRT-001 | Third-Party Model Dependency | Third-Party Dependency | **8: Medium** | In Treatment |
| AI-RISK-2025-007 | CRT-001 | Data Privacy: External API Transmission | Data Privacy | **16: Critical** | In Treatment: DPA negotiation |
| AI-RISK-2025-008 | CRT-001 | Prompt Injection | Adversarial Manipulation | **6: Medium** | In Treatment |

**Critical risks (≥15):** 2: both CRT-001, both in active treatment. CISO notified; AI Governance Committee reviewing monthly pending remediation.

---

## 5. Governance

### Review Cadence

| Activity | Frequency | Responsible |
|---|---|---|
| Critical risk status check | Monthly | AI Governance Committee |
| High risk status check | Monthly | AI System Owners |
| Treatment progress review | Quarterly (AI Governance Committee meeting) | AI System Owners + GRC Team |
| Full risk reassessment | Annual or upon material system change | GRC Team |

### Escalation Thresholds

- New Critical AI risk: Immediate CISO notification
- AI risk increases to Critical: Notification to CISO within 24 hours; AI Governance Committee emergency convened within 5 business days
- Treatment milestone missed by >30 days: Escalation to AI Governance Committee
- AI incident confirming a risk scenario: Immediate reassessment of associated risk entry

### Integration with Enterprise Risk Register

All eight AI risks above are integrated into the Emyzer Nexus enterprise risk register. AI-RISK-2025-005 (LLM hallucination) and AI-RISK-2025-007 (data privacy / DPA gap) are flagged for monthly executive reporting as Critical risks.

---

## 6. Document Control

| Version | Date | Author | Changes |
|---|---|---|---|
| 1.0 | 2025-07-01 | GRC Team | Initial publication |

- **Document ID:** AI-RA-2025-001/002
- **Classification:** Internal Use
- **Next Review:** 2026-07-01 or upon material change to PCM-001 or CRT-001

---

*This document was developed as part of the Emyzer Nexus Phase 2 AI Governance Programme and formatted for portfolio presentation.*

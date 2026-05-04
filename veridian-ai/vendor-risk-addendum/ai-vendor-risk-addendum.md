# AI Vendor Risk Due Diligence Addendum

**Emyzer Nexus: Third-Party Risk Management Programme**

---

> **Simulated Environment**
>
> Emyzer Nexus is a fictional organisation created for this GRC portfolio. All entities, personnel, vendor relationships, and regulatory scenarios are invented for professional demonstration purposes. Framework and regulatory references, [EU AI Act (Regulation 2024/1689)](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32024R1689), [GDPR (Regulation 2016/679)](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32016R0679), [NIST AI RMF 1.0](https://www.nist.gov/artificial-intelligence/ai-risk-management-framework), [ISO 27001:2022](https://www.iso.org/standard/82875.html), are accurate as of the document dates. No real organisation, individual, or vendor relationship is represented.

---

## Document Metadata

| Attribute | Value |
|---|---|
| **Document ID** | INT-VEND-AI-001 |
| **Document Title** | AI Vendor Risk Due Diligence Addendum |
| **Document Type** | Policy Addendum |
| **Version** | 1.0 |
| **Effective Date** | 2025-06-01 |
| **Owner** | Information Security Officer (Susan Orwell) |
| **Approver** | Chief Information Security Officer |
| **Reviewers** | Legal Counsel; Data Protection Officer; Vendor Risk Manager |
| **Classification** | Internal |
| **Parent Policy** | [Third-Party Risk Management Policy (KB-PORTFOLIO-0008)](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/third-party-risk-management-policy.md) |
| **Review Cadence** | Annual; updated when EU AI Act implementing acts are published or material changes occur to the AI vendor landscape |

---

## 1. Purpose and Relationship to Parent Policy

### 1.1 Purpose

This addendum extends the [Third-Party Risk Management Policy (KB-PORTFOLIO-0008)](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/third-party-risk-management-policy.md) with AI-specific due diligence requirements applicable to vendors providing artificial intelligence products, services, or capabilities.

The Phase 1 TPRM Policy was written for Emyzer Technology's hardware and managed services business model. It addresses security posture, data protection, and service continuity: requirements that remain fully applicable to AI vendors. This addendum does not replace any TPRM Policy requirement; it adds obligations specific to the risk profile of AI vendor relationships that the base policy does not address.

The addendum was prompted by the acquisition of Veridian AI (Q4 2024) and the discovery that CRT-001's external LLM API relationship lacked a Data Processing Agreement, contract novation, and EU AI Act compliance evaluation: all gaps that an AI-specific vendor due diligence framework would have identified and required remediation of before approval.

### 1.2 Relationship to Parent Policy

All requirements of the [TPRM Policy](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/third-party-risk-management-policy.md) apply to AI vendors in full. This addendum layers additional requirements on top of those. Where this addendum specifies a stricter or more specific requirement than the base policy, the addendum takes precedence for AI vendor relationships.

### 1.3 Governing Frameworks

| Framework | Application to This Addendum |
|---|---|
| **[EU AI Act (Regulation 2024/1689)](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32024R1689)** [VERIFY] | Deployer obligations for High-Risk AI systems; provider transparency requirements; contractual obligations on deployers using High-Risk systems; post-market monitoring obligations |
| **[NIST AI Risk Management Framework (AI RMF 1.0)](https://www.nist.gov/artificial-intelligence/ai-risk-management-framework)** | MAP function: identifying and assessing AI-specific risks in third-party AI relationships; GOVERN function: establishing AI vendor governance requirements |
| **[ISO/IEC 42001:2023](https://www.iso.org/standard/81230.html)** | AI management system standard; Annex A controls for AI supplier management |
| **[ISO 27001:2022](https://www.iso.org/standard/82875.html)** A.5.19–A.5.23 | Supplier relationship security requirements: extended by this addendum for AI-specific obligations |
| **[GDPR (Regulation 2016/679)](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32016R0679)** [VERIFY] | Data processing obligations for AI systems handling personal data; Article 28 processor requirements; Article 35 DPIA for high-risk processing; Article 22 automated decision-making [VERIFY] |
| **[ISO/IEC 23894:2023](https://www.iso.org/standard/77304.html)** | AI risk management guidance: AI-specific threat identification relevant to vendor relationships |

---

## 2. Scope

### 2.1 When This Addendum Applies

This addendum applies to any vendor relationship involving:

1. AI or machine learning model APIs, platforms, or services where the AI component processes Emyzer Nexus data or produces outputs that inform Emyzer Nexus decisions
2. AI Foundation Model providers (large language models, multimodal models, embedding models) accessed via API
3. AI-native SaaS applications where an AI component performs a core function (e.g., AI-driven contract review, AI-assisted hiring tools, AI-based fraud detection)
4. AI model development tools, training infrastructure, or MLOps platforms with access to training data containing personal or confidential information
5. Third parties providing AI consulting, integration, or development services who develop, train, or deploy AI systems on Emyzer Nexus's behalf
6. AI systems embedded in otherwise standard vendor products where the AI component processes personal data or supports regulated decisions

### 2.2 When This Addendum Does Not Apply

This addendum does not apply to:

- Vendor products that use AI purely for internal optimisation (e.g., AI-powered spam filtering in an email service) where Emyzer Nexus data is not processed by the AI component and AI outputs do not inform Emyzer Nexus decisions
- AI-powered analytics or business intelligence tools that process only anonymised or aggregated data
- Standard software tools with AI-assisted code completion or documentation features (e.g., IDE plugins) where no business-critical data is processed

**When in doubt, the ISO determines whether this addendum applies.**

### 2.3 AI Vendor Types

| AI Vendor Type | Description | Example |
|---|---|---|
| **Foundation Model Provider** | Provides general-purpose large AI models (LLMs, multimodal) via API | CRT-001's external LLM API vendor |
| **Task-Specific AI Vendor** | Provides AI tools or services designed for a specific business task | AI-powered contract analysis, AI-assisted recruiting tools |
| **AI Infrastructure Provider** | Provides compute, storage, or MLOps platforms for AI development or deployment | Cloud ML training platforms |
| **AI Integration / Development Partner** | Builds, trains, or deploys AI systems for Emyzer Nexus | External AI development consultants |

---

## 3. AI Vendor Risk Tier Classification

AI vendors shall be classified under the TPRM Policy risk tier framework (Critical / High / Medium / Low). The following AI-specific factors modify the standard classification criteria:

| Factor | Criteria Adjustment |
|---|---|
| **AI system risk classification** | Any vendor whose AI system or component is classified (or classifiable) as High-Risk under EU AI Act Annex III [VERIFY] is automatically classified as **Critical** or **High** tier, never below High, regardless of data access scope |
| **Foundation model providers** | Foundation Model API vendors are automatically **High** tier minimum due to the opacity of training data, hallucination risk, and inability to independently verify model behaviour |
| **Personal data in AI processing** | Any AI vendor that processes personal data as part of AI inference (not just transit), including contract text, behavioural data, or biometric data, is escalated by one risk tier |
| **Decision support for regulated outcomes** | AI vendors whose outputs inform regulated decisions (credit, employment, healthcare, legal compliance) are automatically **Critical** tier |
| **Single-system dependency** | Where Emyzer Nexus is entirely dependent on a single AI vendor for a business-critical function (as with CRT-001's LLM API), the vendor is **Critical** tier |

---

## 4. Additional Due Diligence Requirements for AI Vendors

AI vendor due diligence shall include all requirements in the parent [TPRM Policy Section F.2](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/third-party-risk-management-policy.md) plus the following AI-specific assessments.

### 4.1 Model Transparency Assessment

The ISO shall obtain from the vendor, prior to contract execution, the following model transparency documentation:

| Requirement | Expected Evidence | Minimum Acceptable Position |
|---|---|---|
| **Model card or technical data sheet** | Published model card describing architecture, intended use, known limitations, and evaluated performance | Model card or equivalent technical summary; verbal-only assertions not acceptable |
| **Intended use disclosure** | Vendor's statement of intended and foreseeable uses; prohibited use cases | Written disclosure; must be evaluated against Emyzer Nexus's proposed use case |
| **Known limitations disclosure** | Documented performance limitations, failure modes, and known biases | Written disclosure; must address the specific use case |
| **Output uncertainty characterisation** | How the model communicates confidence or uncertainty in its outputs | For LLMs: disclosure of hallucination characteristics; for classification models: confidence scores or equivalent |
| **Model versioning and change management** | How model updates are managed, communicated, and tested before deployment | Change notification process with advance notice period (minimum 30 days for material changes) |
| **Explainability capability** | Whether the model can provide explanations of individual outputs | Must be documented; absence of explainability capability is a risk finding requiring AI Governance Committee review |

**Minimum passing threshold:** A vendor unable to provide a model card or equivalent, or unwilling to disclose known limitations, shall not be approved for engagement with AI systems that inform material business decisions without CISO exception approval and documented compensating controls.

### 4.2 Training Data Provenance Assessment

The ISO and DPO shall jointly assess the following training data questions prior to contract execution:

| Requirement | Assessment Questions | Risk Flags |
|---|---|---|
| **Training data categories** | What data types and sources were used to train the model? Does training data include personal data? Does it include data from Emyzer Nexus's sector? | Training on personal data without GDPR-compliant consent basis; training data from sectors with materially different distributions than Emyzer Nexus's use case |
| **Data provenance documentation** | Can the vendor provide documentation of data sources, consent or licensing basis, and data cleaning methodology? | Inability to provide provenance documentation for systems processing personal data is a Critical risk finding |
| **Consent and licensing basis** | Were training data sources used under appropriate licences, consent, or statutory authority? | Vendor reliance on "scraped" public data without clear legal basis for training data including personal data [VERIFY: Article 6 GDPR lawful basis for training data] |
| **Bias examination** | Has the training data been examined for representation gaps, historical biases, or demographic skews? Is bias testing documentation available? | No bias examination conducted; bias examination results not available for review |
| **Data minimisation** | Was personal data in training sets minimised, pseudonymised, or anonymised where technically feasible? | Training on identifiable personal data where anonymisation was feasible but not applied |
| **Ongoing data governance** | How is training data managed post-training? Can Emyzer Nexus data be excluded from future training? | Vendor uses inference data (including Emyzer Nexus's data submissions) to retrain without opt-out mechanism |

**[VERIFY: Whether GDPR Article 10 [VERIFY] (training data quality obligations) applies to Emyzer Nexus as a deployer when using a third-party AI system, or whether this obligation rests entirely with the provider. Legal Counsel to advise on deployer obligations for inherited training data risks.]**

### 4.3 Bias and Fairness Testing Assessment

The ISO shall obtain bias and fairness testing evidence from AI vendors whose systems influence decisions affecting individuals or groups.

| Requirement | Evidence to Obtain | Minimum Standard |
|---|---|---|
| **Bias testing methodology** | Documentation of how the vendor tests for demographic or group-based bias in model outputs | Written testing methodology; outputs reviewed for protected characteristic impact |
| **Protected characteristics assessed** | Which protected characteristics were included in bias testing? | For EU deployments: assessment must cover age, sex, racial or ethnic origin, religion, disability, sexual orientation at minimum [VERIFY: EU equality law applicable characteristics] |
| **Bias testing results** | Results of bias evaluations; known disparate impact findings; remediation actions taken | Vendor must disclose material disparate impact findings; refusal to disclose is a High risk finding |
| **Fairness metric definitions** | Which fairness metrics does the vendor use? (e.g., demographic parity, equalised odds, individual fairness) | Vendor must define the fairness metrics applied; "we test for fairness" without metrics is not acceptable |
| **Ongoing bias monitoring** | Is bias monitored in production? How are bias regressions detected and reported? | Continuous or periodic bias monitoring with defined thresholds; regression reporting mechanism |

**Specific requirement for AI systems in regulated decision contexts (credit, employment, healthcare, legal):** Bias testing results must be obtained and reviewed by the AI Governance Committee before the vendor relationship is approved. Any finding of material disparate impact against a protected characteristic is a Critical risk finding requiring treatment plan before approval.

### 4.4 EU AI Act Compliance Status Assessment

The ISO and Legal Counsel shall assess the AI vendor's EU AI Act compliance status as part of due diligence.

| Assessment Area | Questions | Risk Flags |
|---|---|---|
| **Risk tier classification** | Has the vendor classified their AI system under the EU AI Act? What risk tier do they claim? Is the classification documented? | Vendor has not assessed their EU AI Act obligations; vendor claims Minimal Risk for a system that appears High-Risk by Annex III criteria [VERIFY] |
| **Provider obligations** | For High-Risk systems: has the vendor completed a conformity assessment? Is a Declaration of Conformity available? Is the system registered in the EU AI database [VERIFY: Article 71 database requirement]? | Missing conformity assessment or Declaration of Conformity for an apparent High-Risk system |
| **Technical documentation** | For High-Risk systems: does the vendor make Annex IV [VERIFY] technical documentation available to deployers on request? | Refusal to provide technical documentation to deployers is a regulatory non-compliance finding |
| **Human oversight features** | Has the vendor implemented the human oversight measures required under Article 14 [VERIFY]? Are override capabilities and halt mechanisms available? | No override capability for High-Risk AI system outputs |
| **Post-market monitoring** | For High-Risk systems: does the vendor have an Article 72 [VERIFY] post-market monitoring plan? How is serious incident reporting handled under Article 73 [VERIFY]? | No post-market monitoring plan for High-Risk system |
| **GPAI model obligations** | For General Purpose AI model providers: has the vendor complied with the GPAI model transparency obligations in EU AI Act Chapter V [VERIFY: applicability threshold and obligations]? | Foundation Model API provider with no compliance documentation for Chapter V obligations |

**[VERIFY: EU AI Act implementation timeline for providers; confirm which obligations are in force as of this addendum's effective date (2025-06-01) and which are subject to transitional provisions. Legal Counsel to maintain current implementation status.]**

**Risk finding classification for EU AI Act gaps:**

| Finding | Classification |
|---|---|
| Vendor has no EU AI Act assessment for an apparent High-Risk system | Critical |
| Missing Declaration of Conformity for High-Risk system | Critical |
| No conformity assessment for High-Risk system | Critical |
| Incomplete technical documentation for High-Risk system | High |
| No post-market monitoring plan for High-Risk system | High |
| Vendor EU AI Act assessment not current (>12 months old) | Medium |

### 4.5 Operational Risk Assessment

AI-specific operational risks shall be assessed in addition to the standard TPRM operational risk evaluation.

| Risk Area | Assessment |
|---|---|
| **Hallucination / model error rate** | For LLM-based systems: obtain or establish empirical hallucination rate for the proposed use case. Risk rating is proportionate to the consequence of erroneous outputs. |
| **Model availability and continuity** | Is there an API SLA? What is the vendor's model continuity commitment (notice period before model discontinuation)? Is a fallback model or service available? |
| **API version management** | What is the vendor's policy for deprecating API versions? Minimum advance notice required: 90 days. |
| **Sub-processor chains** | Has the vendor disclosed its sub-processors? Is the sub-processor list current? Emyzer Nexus must review sub-processor obligations for GDPR Article 28(4) [VERIFY] compliance. |
| **Concentration risk** | Is Emyzer Nexus dependent on this vendor for multiple AI capabilities? Critical tier if single vendor provides >50% of AI processing capability. |
| **Export controls** | Are there export control restrictions on the AI technology that could affect Emyzer Nexus's use? [VERIFY: applicable export control regimes for AI technology] |

---

## 5. Contractual Safeguards for AI Vendors

In addition to the standard contract provisions required by [TPRM Policy Section F.3](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/third-party-risk-management-policy.md), all AI vendor contracts shall include the following provisions. Requirements marked **[MANDATORY]** must appear in all AI vendor contracts. Requirements marked **[HIGH/CRITICAL TIER]** apply to High and Critical tier vendors.

### 5.1 Transparency and Documentation Obligations [MANDATORY]

| Obligation | Requirement |
|---|---|
| Model card or technical summary | Vendor shall provide and maintain a current model card or technical data sheet covering architecture, intended use, known limitations, and evaluated performance |
| Change notification | Vendor shall provide minimum 30 days' advance written notice of material changes to the AI model, including retraining, architectural changes, and known capability or limitation changes |
| Limitation disclosure | Vendor shall disclose known failure modes, accuracy limitations, and performance boundaries relevant to Emyzer Nexus's use case |
| EU AI Act documentation (High-Risk systems) | For systems classified as High-Risk: vendor shall make Annex IV technical documentation available to Emyzer Nexus on written request within 30 business days |

### 5.2 Training Data and Bias Obligations [MANDATORY]

| Obligation | Requirement |
|---|---|
| Training data disclosure | Vendor shall disclose the categories and sources of training data used to develop the AI system and provide documentation of the consent or licensing basis |
| Inference data non-use | Vendor shall not use data submitted by Emyzer Nexus during inference (including document content, queries, and outputs) to train or fine-tune AI models without Emyzer Nexus's express prior written consent |
| Bias testing disclosure | Vendor shall disclose bias testing methodology, protected characteristics assessed, and material findings; material disparate impact findings discovered post-contract must be notified to Emyzer Nexus within 30 days |
| Bias remediation | Vendor shall provide a remediation timeline for material disparate impact findings; failure to remediate within agreed timeframes is grounds for contract termination |

### 5.3 EU AI Act Compliance Warranties [HIGH/CRITICAL TIER]

| Obligation | Requirement |
|---|---|
| Compliance warranty | Vendor warrants that its AI system complies with all applicable EU AI Act obligations for providers as of the effective date and shall maintain compliance throughout the contract term |
| Classification accuracy warranty | Vendor warrants that its EU AI Act risk tier classification is accurate and was conducted with reasonable care |
| Conformity assessment | For High-Risk systems: vendor warrants that a conformity assessment has been completed and shall provide a copy of the Declaration of Conformity on request |
| Compliance change notification | Vendor shall notify Emyzer Nexus within 30 days of any EU AI Act compliance status change, including regulatory investigation, serious incident report, or conformity assessment withdrawal |
| Post-market monitoring | For High-Risk systems: vendor shall maintain an Article 72 [VERIFY] post-market monitoring plan and share summary results with Emyzer Nexus annually |

### 5.4 GDPR Data Processing Obligations [MANDATORY where personal data is processed]

| Obligation | Requirement |
|---|---|
| Data Processing Agreement | A GDPR-compliant Data Processing Agreement (DPA) meeting Article 28 [VERIFY] requirements shall be executed before any personal data is transmitted to the AI vendor |
| Sub-processor list | Vendor shall provide and maintain a current list of sub-processors; new sub-processors shall be notified to Emyzer Nexus with 30 days' advance notice and right to object |
| Data residency | Vendor shall specify and maintain the data residency location for all data processing; transfers outside the EEA require appropriate transfer mechanisms [VERIFY: GDPR Chapter V transfer requirements] |
| Inference data minimisation | Vendor shall not retain inference data (Emyzer Nexus data submissions) beyond the period necessary to return the AI output, unless Emyzer Nexus has provided explicit written consent for retention |
| Data processing restriction | Vendor shall process Emyzer Nexus personal data only for the specified purpose documented in the DPA; purpose limitation applies to all sub-processors |

### 5.5 Liability and Accountability for AI Errors [HIGH/CRITICAL TIER]

| Obligation | Requirement |
|---|---|
| Liability for material AI errors | Vendor acknowledges that AI system errors, hallucinations, or discriminatory outputs may cause material harm to Emyzer Nexus; the contract shall include provisions allocating liability for losses caused by AI system failures outside declared performance parameters |
| Indemnification for compliance failures | Vendor shall indemnify Emyzer Nexus against regulatory penalties arising from vendor's EU AI Act compliance failures for the AI system provided |
| Error notification | Vendor shall notify Emyzer Nexus within 24 hours of discovery of any AI system defect or error that could cause material harm in Emyzer Nexus's use case |
| Insurance | Vendor shall maintain professional indemnity insurance covering AI system errors at a minimum level proportionate to Emyzer Nexus's exposure (to be specified in the contract schedule) |

### 5.6 Continuity and Exit Requirements [HIGH/CRITICAL TIER]

| Obligation | Requirement |
|---|---|
| Service continuity commitment | Vendor shall provide minimum 6 months' written notice before discontinuing the AI system or API service |
| API version continuity | Vendor shall support the contracted API version for minimum 12 months following notification of deprecation |
| Alternative service | Vendor shall identify and, where feasible, provide migration assistance to an alternative AI system if the contracted service is discontinued |
| Exit assistance | Vendor shall provide 90 days of exit assistance including data export, transition support, and documentation of any fine-tuning or customisation applied to the model for Emyzer Nexus's use |

---

## 6. Ongoing Monitoring of AI Vendors

In addition to the standard monitoring requirements in [TPRM Policy Section F.5](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/third-party-risk-management-policy.md), AI vendors are subject to the following ongoing monitoring activities.

### 6.1 AI Performance Monitoring

| Activity | Frequency | Responsible |
|---|---|---|
| Output quality sampling: LLM-based systems | Quarterly (minimum 20 samples per system) | AI System Owner |
| Drift monitoring: traditional ML systems | Monthly (automated) + quarterly review | AI System Owner / CTO |
| Bias regression check | Semi-annual | AI Governance Committee |
| Vendor EU AI Act compliance status review | Annual | ISO / Legal Counsel |
| Sub-processor list review | Annual or on notification of change | DPO |
| Model card / technical documentation currency review | Annual | ISO |

### 6.2 AI Incident Reporting

AI vendors shall report the following AI-specific incident types to Emyzer Nexus within the timeframes specified:

| Incident Type | Notification Timeframe | Recipient |
|---|---|---|
| Serious incident under EU AI Act Article 73 [VERIFY] (death, serious harm, fundamental rights breach, critical infrastructure disruption) | Within 24 hours of vendor's discovery | CISO + Legal Counsel |
| Confirmed hallucination or material AI error affecting Emyzer Nexus's use case | Within 24 hours of discovery | AI System Owner + ISO |
| Bias or discriminatory output affecting protected characteristics | Within 24 hours of discovery | CISO + DPO |
| Security incident affecting model integrity or Emyzer Nexus data | Within 24 hours (per TPRM Policy) | ISO + AI System Owner |
| Material change to model behaviour outside change management process | Within 24 hours of discovery | AI System Owner + CTO |
| EU AI Act compliance investigation or enforcement action against vendor | Within 5 business days of vendor receiving regulatory contact | CISO + Legal Counsel |

### 6.3 AI Vendor Reassessment Triggers

In addition to the standard tier-based reassessment schedule, AI vendor relationships shall be reassessed when:

- A material EU AI Act compliance change occurs (e.g., conformity assessment withdrawn, Declaration of Conformity updated)
- Vendor discloses a material bias or disparate impact finding
- An AI serious incident occurs involving the vendor's system
- The vendor releases a major new model version replacing the contracted version
- A regulatory enforcement action is taken against the vendor in any jurisdiction
- Emyzer Nexus's use case changes materially (e.g., the system is used for a new decision type)

---

## 7. AI Governance Committee Referral

The following situations require referral to the [AI Governance Committee](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/ai-governance/readme.md) before an AI vendor relationship is approved:

1. The vendor's AI system appears classifiable as High-Risk under EU AI Act Annex III [VERIFY], regardless of the vendor's own classification
2. The vendor's AI system will be used to support decisions in a regulated domain (credit, employment, healthcare, legal compliance, law enforcement)
3. The vendor's bias testing discloses material disparate impact against a protected characteristic
4. The AI system processes significant volumes of personal data without a clearly established GDPR legal basis
5. The vendor is unwilling to provide training data provenance documentation and the AI system will process personal data
6. A Critical risk finding is identified during AI vendor due diligence and the business owner wishes to proceed

AI Governance Committee referrals shall be documented in the GRC platform. Approval requires a quorum of the AI Governance Committee and a documented risk acceptance rationale.

---

## 8. Application to Existing Vendor Relationships

### 8.1 Retrospective Application

This addendum applies to all new AI vendor engagements from its effective date (2025-06-01). For AI vendor relationships in existence before 2025-06-01, the following retrospective schedule applies:

| Relationship | Priority | Assessment Target |
|---|---|---|
| CRT-001 LLM API vendor | **Critical: immediate** | DPA execution: 2025-09-30; full addendum assessment: 2025-12-31 |
| Any future AI vendor relationships | Standard | Full addendum assessment before contract execution |

### 8.2 CRT-001 LLM API Vendor: Current Status

The CRT-001 LLM API vendor relationship is the only AI vendor relationship in scope at this addendum's effective date. It was assessed during the Veridian AI due diligence exercise ([Veridian AI Risk Assessment VDA-RA-2025-001](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/veridian-ai/ai-risk-assessments/veridian-ai-risk-assessment.md)) and found to have the following critical gaps:

| Gap | Status | Addendum Requirement | Target |
|---|---|---|---|
| No GDPR Article 28 DPA | In remediation | Section 5.4 (Mandatory) | 2025-09-30 |
| Contract not novated to Emyzer Nexus | In remediation | Section 5.6 basis | 2025-06-30 |
| Training data provenance unavailable | Blocked: vendor cooperation required | Section 4.2 | 2025-12-31 |
| No Declaration of Conformity | In remediation | Section 5.3 | 2025-12-31 |
| Sub-processor list not obtained | In remediation | Section 5.4 | 2025-09-30 |
| Model card not provided | In remediation | Section 5.1 | 2025-09-30 |

The use restriction on CRT-001 (contracts containing no personal data only) remains in effect until the DPA is executed. See the [AI System Inventory](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/ai-governance/ai-system-inventory.md), CRT-001 profile, for current governance status.

---

## 9. Roles and Responsibilities

| Role | AI Vendor Due Diligence Responsibilities |
|---|---|
| **ISO (Susan Orwell)** | Leads AI vendor due diligence; applies this addendum; approves High tier AI vendors; escalates Critical tier to CISO; maintains AI vendor risk assessments in GRC platform |
| **CISO** | Approves Critical tier AI vendors; chairs AI Governance Committee referral decisions; receives quarterly AI vendor risk reporting |
| **Legal Counsel** | Reviews AI vendor contracts for EU AI Act compliance warranties, liability provisions, and GDPR DPA adequacy; advises on vendor EU AI Act compliance assessment |
| **Data Protection Officer** | Reviews training data provenance assessments; co-leads inference data non-use and sub-processor assessments; executes or reviews DPAs |
| **AI Governance Committee** | Receives referrals for High-Risk AI system approvals and bias finding decisions; approves AI vendor risk acceptance in cases meeting referral criteria |
| **Vendor Risk Manager** | Maintains AI vendor inventory; coordinates due diligence documentation collection; tracks reassessment schedules; escalates incomplete assessments |
| **Business Owner** | Identifies business need; manages vendor relationship; monitors AI output quality in deployment; reports anomalies to ISO |
| **CTO** | Provides technical assessment of AI system architecture, API security, and operational risk; assesses hallucination mitigation and bias testing technical validity |

---

## 10. Evidence Requirements

The following evidence shall be maintained for AI vendor relationships:

| Evidence Type | When Produced | Retention | System of Record |
|---|---|---|---|
| AI vendor due diligence assessment (this addendum applied) | Before contract execution | Contract + 5 years | GRC Platform |
| Model card / technical data sheet | At onboarding and annually | Contract + 5 years | GRC Platform |
| Training data provenance documentation | At onboarding | Contract + 5 years | GRC Platform |
| Bias testing results | At onboarding and on update | Contract + 5 years | GRC Platform |
| EU AI Act compliance assessment | At onboarding and annually | Contract + 5 years | GRC Platform |
| Executed Data Processing Agreement | Before personal data transmission | Contract + 7 years | Legal Repository |
| Sub-processor list (current) | At onboarding and on update | Contract + 5 years | GRC Platform / Legal Repository |
| AI vendor contract with addendum provisions | At execution | Contract + 7 years | Legal Repository |
| AI performance monitoring records | Ongoing (per Section 6.1) | 3 years | GRC Platform |
| AI incident notifications | Per incident | 7 years | GRC Platform |
| AI Governance Committee referral decisions | On referral | 7 years | GRC Platform |
| Vendor reassessment records | Per reassessment | 3 years | GRC Platform |

---

## 11. Framework Alignment

| Framework | Addendum Section |
|---|---|
| **[EU AI Act (Regulation 2024/1689)](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32024R1689): Deployer obligations** [VERIFY] | Sections 4.4, 5.3, 6.2 |
| **[EU AI Act Article 9](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32024R1689): Risk management** [VERIFY] | Sections 3, 4 |
| **[EU AI Act Article 13](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32024R1689): Transparency** [VERIFY] | Section 4.1 (model transparency) |
| **[EU AI Act Article 14](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32024R1689): Human oversight** [VERIFY] | Section 4.4, 5.3 |
| **[EU AI Act Article 72](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32024R1689): Post-market monitoring** [VERIFY] | Sections 5.3, 6.1 |
| **[EU AI Act Article 73](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32024R1689): Serious incident reporting** [VERIFY] | Section 6.2 |
| **[NIST AI RMF 1.0: MAP](https://www.nist.gov/artificial-intelligence/ai-risk-management-framework)** | Sections 4, 5 (mapping AI-specific risks in vendor relationships) |
| **[NIST AI RMF 1.0: GOVERN](https://www.nist.gov/artificial-intelligence/ai-risk-management-framework)** | Sections 7, 9 (governance roles; documentation) |
| **[ISO 27001:2022](https://www.iso.org/standard/82875.html) A.5.19–A.5.23** | Sections 4–6 (AI-extended supplier relationship requirements) |
| **[ISO/IEC 42001:2023](https://www.iso.org/standard/81230.html) Annex A** | Sections 4.2 (training data), 5.2 (bias) |
| **[GDPR Article 28](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32016R0679)** [VERIFY] | Section 5.4 (processor obligations) |
| **[GDPR Article 35](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32016R0679): DPIA** [VERIFY] | Section 4.2 (training data with personal data) |

---

## 12. Document Control

| Version | Date | Author | Changes |
|---|---|---|---|
| 1.0 | 2025-06-01 | ISO (Susan Orwell) + Legal Counsel | Initial publication: effective from AI Governance Programme launch date |

- **Document ID:** INT-VEND-AI-001
- **Parent Policy:** [Third-Party Risk Management Policy KB-PORTFOLIO-0008](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/third-party-risk-management-policy.md)
- **Classification:** Internal
- **Next Review:** 2026-06-01 or upon publication of EU AI Act implementing acts affecting deployer or supplier obligations

---

*This document was developed as part of the Emyzer Nexus Phase 2 GRC Programme and formatted for portfolio presentation. All vendor relationships and risk scenarios are fictional.*

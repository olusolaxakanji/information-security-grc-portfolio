# Model Risk Policy

**Emyzer Nexus – Governance, Risk, and Compliance**

---

## Policy Metadata

| Attribute | Value |
|-----------|-------|
| **Policy Name** | Model Risk Policy |
| **Type** | Policy |
| **Version** | 1.0 |
| **Parent Policy** | AI Governance Policy (KB-PORTFOLIO-0011) |
| **Owner** | Chief Risk Officer |
| **Owning Group** | App Engine Admins |
| **State** | Published |
| **Valid From** | 2025-09-01 |
| **Valid To** | 2026-09-01 |
| **Approvers** | Chief Executive Officer |
| **Reviewers** | Chief Information Security Officer; GRC Analyst; Legal Counsel; Chief Technology Officer |
| **Knowledge Base** | Governance, Risk, and Compliance |
| **Published Policy** | KB-PORTFOLIO-0012 |

---

## Description

This policy governs the identification, development, validation, approval, deployment, ongoing monitoring, and retirement of models across Emyzer Nexus and its subsidiaries. It establishes minimum standards for model risk management proportionate to each model's complexity, materiality, and potential for harm: including AI and machine learning models governed at the strategic level by the AI Governance Policy.

**Impact:** Unmanaged model risk exposes Emyzer Nexus to material financial loss, flawed business decisions, regulatory breach, and harm to customers and counterparties. This policy operationalises a structured model lifecycle, independent validation function, and tiered monitoring regime to ensure models perform as intended throughout their operational life. It is essential to managing risk inherited through the Veridian AI acquisition, where model documentation, validation status, and ongoing monitoring practices require formal assessment and remediation.

**Relevant Standards:** SR 11-7 (Federal Reserve / OCC Supervisory Guidance on Model Risk Management), NIST AI Risk Management Framework (AI RMF 1.0), EU AI Act (Regulation 2024/1689), ISO/IEC 42001:2023, ISO/IEC 23894:2023

---

## Policy Snapshot

| Dimension | Summary |
|-----------|---------|
| **Applies to** | All Emyzer Nexus business units, subsidiaries (including Emyzer Technology), acquired entities (Veridian AI models), employees, contractors, and third parties involved in model development, validation, deployment, or operation |
| **Covers** | All quantitative and AI/ML models used to support business decisions, including predictive models, scoring models, statistical models, simulation models, and AI systems classified under the AI Governance Policy |
| **Model Tiers** | Tier 1 (High), Tier 2 (Medium), Tier 3 (Low): based on materiality, complexity, and potential for harm |
| **Validation Requirement** | Independent validation required for all Tier 1 and Tier 2 models before deployment and following material change |
| **Review Cadence** | Annual policy review; model inventory reviewed quarterly; Tier 1 performance reviewed monthly; Tier 2 quarterly; Tier 3 annually |
| **Key Governance** | CRO owns the program; Model Risk Committee provides oversight; Model Owners manage lifecycle; Model Validation Function conducts independent review |
| **Exceptions Process** | ServiceNow workflow with CRO approval; maximum 90 days; quarterly review |
| **Evidence Maintained** | Model inventory, development documentation, validation reports, approval records, performance monitoring logs, limitation disclosures, retirement records (all with defined retention periods) |

---

## A. Purpose

To establish the governance framework, minimum standards, and control requirements for model risk management across Emyzer Nexus, ensuring that models are developed with rigour, validated independently, deployed with documented limitations, monitored continuously, and retired in a controlled manner. This policy operationalises the model-specific obligations referenced in the AI Governance Policy and provides the detailed lifecycle controls that govern the Predictive Customer Churn Model and AI-Assisted Contract Review Tool inherited through the Veridian AI acquisition, as well as any models developed or procured thereafter.

Model risk is the risk of adverse outcomes arising from errors in model development, inappropriate use of models, use of models outside their intended scope, failure to account for model limitations, or inadequate monitoring of model performance over time. This policy treats model risk as a distinct and material risk category requiring dedicated governance structures, proportionate controls, and continuous oversight: not as a subset of general operational risk.

The policy aligns with SR 11-7 (the Federal Reserve and OCC supervisory guidance on model risk management), the NIST AI Risk Management Framework, and the technical documentation, accuracy, and post-market monitoring obligations of the EU AI Act applicable to AI and machine learning models in scope of the AI Governance Policy.

---

## B. Scope

### B.1 In-Scope Models

This policy applies to all quantitative models and AI/ML systems used by Emyzer Nexus to inform business decisions, generate customer-facing outputs, support risk management, or fulfil regulatory obligations. A **model**, for the purposes of this policy, is any quantitative method, system, or approach, including statistical, mathematical, machine learning, or AI-based methods, that processes input data to generate outputs used to support business decisions or generate outputs with real-world consequences.

Model types in scope include, but are not limited to:

- **Predictive and scoring models:** Systems that produce probability estimates, scores, or classifications used in decision-making (e.g., customer churn prediction, credit risk scoring, fraud detection)
- **AI and machine learning models:** Systems governed by the AI Governance Policy that also meet the definition of a model under this policy; for these systems, this policy provides the operational model lifecycle requirements subordinate to AI Governance Policy strategic governance obligations
- **Contract and document analysis models:** NLP-based systems used to review, classify, or extract information from legal or commercial documents
- **Simulation and optimisation models:** Systems that model scenarios, forecast outcomes, or optimise allocations for business or risk management purposes
- **Vendor and third-party models:** Models developed or maintained by external parties and used by Emyzer Nexus, including models accessed via API

**Models currently in scope at time of publication:**

| Model Name | Origin | Classification | Tier | Status |
|------------|--------|----------------|------|--------|
| Predictive Customer Churn Model | Veridian AI (acquired) | AI/ML: EU AI Act High-Risk | Tier 1 | Under validation |
| AI-Assisted Contract Review Tool | Veridian AI (acquired) | AI/ML: EU AI Act High-Risk | Tier 1 | Under validation |

### B.2 Exclusions

The following are excluded from this policy unless they meet the model definition above:

- Rule-based systems executing deterministic logic with no statistical or learned components
- Standard financial calculations embedded in accounting or ERP systems (e.g., interest accrual, depreciation)
- Spreadsheet calculations that are fully transparent, auditable, and involve no statistical inference

Exclusion determinations shall be made by the Model Risk Committee and documented in the Model Inventory. When in doubt, the system shall be treated as in-scope.

### B.3 Third-Party Applicability

Third parties developing, supplying, or operating models on behalf of Emyzer Nexus shall comply with model governance requirements through contractual obligations. Emyzer Nexus shall retain the right to request validation documentation, model performance reports, limitation disclosures, and audit access for all material third-party models. Third-party model due diligence is governed by the AI Vendor Risk Due Diligence Addendum and the Third-Party Risk Management Policy.

---

## C. Definitions

| Term | Definition |
|------|------------|
| **Model** | Any quantitative method, system, or approach, including statistical, mathematical, machine learning, or AI-based methods, that processes input data to generate quantitative outputs used to inform business decisions or produce outputs with real-world consequences. Adapted from SR 11-7. |
| **Model Risk** | The risk of adverse outcomes, including financial loss, flawed decisions, regulatory breach, or harm to customers, arising from errors in model development, inappropriate use, use outside intended scope, failure to account for limitations, or inadequate ongoing monitoring. |
| **Model Tier** | A classification (Tier 1: High, Tier 2: Medium, Tier 3: Low) assigned to a model based on its materiality, complexity, and potential for harm, determining the level of validation and monitoring required. |
| **Model Owner** | The individual accountable for a model's lifecycle governance, including development oversight, documentation, use management, monitoring, and retirement. |
| **Model Developer** | The individual or team responsible for designing, building, and initially testing a model. |
| **Model User** | Any individual or business unit that applies model outputs to inform decisions, whether or not they built the model. |
| **Independent Validation** | A structured review of a model conducted by personnel with no involvement in model development, assessing conceptual soundness, data quality, testing rigour, and performance. Required for Tier 1 and Tier 2 models under this policy. |
| **Model Validation Function** | The internal team or qualified external party responsible for conducting independent model validation. Must be organisationally independent of model development functions. |
| **Conceptual Soundness** | The degree to which a model's theoretical basis, design choices, and assumptions are appropriate for the model's intended use and supported by established knowledge and evidence. |
| **Model Limitations** | Known constraints, boundary conditions, assumptions, or scenarios in which a model's outputs may be less reliable, less accurate, or invalid. |
| **Model Drift / Data Drift** | Degradation in model performance over time due to changes in the underlying data distribution or real-world conditions that differ from those represented in training data. |
| **Backtesting** | Applying a model to historical data to evaluate how it would have performed, used to assess predictive accuracy and identify systematic errors. |
| **Benchmarking** | Comparing a model's outputs or methodology to those of alternative models or established industry approaches to assess relative performance and conceptual validity. |
| **Champion-Challenger Testing** | An evaluation method in which a deployed model (champion) is compared against one or more alternative models (challengers) operating on live or test data to assess relative performance. |
| **Model Inventory** | The formal register of all models within scope of this policy, including tier classification, owner, status, validation history, and monitoring schedule. |
| **Material Change** | Any modification to a model's inputs, outputs, algorithms, training data, intended use, deployment environment, or scope that may alter the model's behaviour, performance, or risk profile. |
| **Model Retirement** | The formal, controlled process of decommissioning a model, including cessation of use, documentation archival, and data disposition. |
| **Overlay / Adjustment** | A manual modification applied to model outputs by qualified personnel to correct for known model limitations, changed conditions, or expert judgement. |
| **SR 11-7** | Supervisory Guidance on Model Risk Management issued by the Federal Reserve Board and Office of the Comptroller of the Currency (2011), the foundational supervisory framework for model risk management in regulated financial institutions. Applied by Emyzer Nexus as a leading-practice standard. |
| **Post-Market Monitoring** | As used in the EU AI Act (Article 72): systematic collection and analysis of data on deployed AI/ML model performance and impacts. Operationalised under this policy as ongoing model monitoring. |

---

## D. Policy Statement

Emyzer Nexus recognises that models are integral to business operations, risk management, and customer outcomes, and that model failures can cause material harm if not governed appropriately. The organisation shall:

1. Maintain a complete and current **Model Inventory**, with all in-scope models identified, registered, and tiered **within 30 days** of development initiation, procurement, acquisition, or material change.

2. Apply **tiered governance** proportionate to each model's complexity, materiality, and potential for harm, with Tier 1 models subject to the most rigorous validation, approval, and monitoring requirements.

3. Require **independent validation** for all Tier 1 and Tier 2 models before deployment authorisation is granted, and following any material change. Validation shall be conducted by the Model Validation Function, which must be organisationally independent from model development.

4. Ensure all models are **documented comprehensively** from development through retirement, with documentation sufficient to enable a knowledgeable third party to understand the model's purpose, design, assumptions, limitations, validation status, and appropriate use without assistance from the original developer.

5. Ensure model outputs are used only for their **intended purposes** within their documented scope of applicability. Use of a model outside its validated scope requires Model Risk Committee approval and updated validation.

6. Require all models to disclose **known limitations** to users and decision-makers before operational use. No model shall be presented as limitation-free.

7. Implement **ongoing performance monitoring** for all deployed models at frequencies calibrated to their tier, with defined triggers for escalation, revalidation, or suspension when performance deteriorates.

8. Govern model **overlays and adjustments** through a structured approval process, ensuring all modifications to model outputs are documented, justified, time-limited, and subject to regular review.

9. Maintain a **Model Risk Committee** with cross-functional representation to provide oversight of the model lifecycle, approve tier classifications, review validation findings, and escalate model-related risks to executive leadership.

10. Govern the **retirement of all models** through a formal process that ensures decisions based on the model's outputs are appropriately reconciled and that documentation is archived for the required retention period.

11. Review and update this policy **annually** or following a significant model-related incident, a material change in the organisation's model portfolio, or relevant changes to applicable guidance or regulation.

---

## E. Model Tiering Framework

All models shall be assigned a tier based on the assessment criteria below. Tier assignments shall be proposed by the Model Owner, reviewed by the GRC Team, and approved by the Model Risk Committee.

### E.1 Tier Assignment Criteria

| Criterion | Tier 1 (High) | Tier 2 (Medium) | Tier 3 (Low) |
|-----------|--------------|-----------------|--------------|
| **Financial Materiality** | Outputs influence decisions with significant financial impact (e.g., revenue, credit, pricing at scale) | Outputs influence decisions with moderate financial impact | Outputs have limited or indirect financial impact |
| **Regulatory Relevance** | Model outputs or practices subject to regulatory scrutiny, including EU AI Act High-Risk classification | Model supports compliance or reporting functions | No direct regulatory relevance |
| **Complexity** | Complex architecture (e.g., deep learning, ensemble methods, multi-stage ML pipelines); non-linear relationships; limited inherent explainability | Moderate complexity; some transparency; established methodology | Simple, transparent methodology; easily interpretable |
| **Customer / Third-Party Impact** | Outputs affect customers or counterparties in material ways (e.g., decisions affecting service access, contractual terms, pricing) | Outputs inform internal decisions that may indirectly affect customers | Primarily internal; limited or no external impact |
| **Data Sensitivity** | Processes personal data, sensitive categories, or proprietary data at scale | Processes some personal or sensitive data | Minimal or no sensitive data inputs |
| **Breadth of Use** | Used by multiple business units or customer-facing functions; embedded in automated or semi-automated decision pipelines | Used by a defined team or function; outputs reviewed by humans before action | Narrow, isolated use; outputs always reviewed by qualified personnel |
| **Consequence of Failure** | Model failure could result in regulatory breach, significant financial loss, harm to customers, or reputational damage | Model failure could result in operational disruption, suboptimal decisions, or moderate financial impact | Model failure has limited operational consequence and is quickly detectable |

### E.2 Tier Governance Requirements Summary

| Requirement | Tier 1 | Tier 2 | Tier 3 |
|-------------|--------|--------|--------|
| Model Inventory registration | Required | Required | Required |
| Full development documentation | Required | Required | Simplified |
| Independent validation before deployment | Required | Required | Not required (self-assessment) |
| Model Risk Committee approval before deployment | Required | Required (delegated approval permitted) | GRC Team notification |
| Performance monitoring | Monthly | Quarterly | Annually |
| Bias testing | Quarterly | Semi-annually | On material change |
| Drift assessment | Quarterly | Semi-annually | Annually |
| Formal revalidation | On material change or ≥24 months | On material change or ≥36 months | On material change |
| Limitation disclosure to users | Required before use | Required before use | Required before use |
| Model Risk Committee quarterly review | Required | Required | Aggregate summary |

### E.3 Tiering of Acquired Veridian AI Models

The Predictive Customer Churn Model and AI-Assisted Contract Review Tool inherited through the Veridian AI acquisition are classified as **Tier 1** based on:
- EU AI Act High-Risk classification under the AI Governance Policy
- Customer-facing outputs with potential to influence service decisions and contractual terms
- Complex ML architecture with limited inherent explainability
- Processing of personal and commercially sensitive data at scale
- Absence of completed Emyzer Nexus independent validation at time of acquisition

Both models are operating under **interim monitoring arrangements** pending completion of full independent validation. Deployment continuation is subject to quarterly Model Risk Committee review until validation is complete.

---

## F. Roles and Responsibilities

### F.1 Chief Executive Officer (CEO)
Approves the Model Risk Policy and material amendments. Receives **quarterly** executive briefings on model risk posture from the Chief Risk Officer. Provides board-level accountability for model risk management outcomes.

### F.2 Chief Risk Officer (CRO)
Owns the Model Risk Policy and the model risk management program. Chairs the Model Risk Committee. Approves Tier 1 model deployment authorisations and exception requests. Escalates unresolvable model risk issues to the CEO. Reports model risk posture to executive leadership **monthly** and to the Board **quarterly**.

### F.3 Chief Information Security Officer (CISO)
Ensures model risk governance is integrated with the ISMS and the AI Governance Policy. Reviews model risk findings that intersect with information security obligations, including data governance, third-party AI security, and EU AI Act technical documentation requirements. Joint authority with the CRO over AI/ML models classified under both this policy and the AI Governance Policy.

### F.4 Model Risk Committee
A cross-functional governance body chaired by the CRO, comprising the CISO, Chief Technology Officer, Legal Counsel, Chief Financial Officer, and heads of affected business units. The committee shall:
- Meet **quarterly** to review the Model Inventory, approve tier classifications, review validation findings, and assess emerging model risks
- Approve Tier 1 model deployment and retirement decisions
- Review the status of acquired Veridian AI models **quarterly** until independent validation is complete
- Convene within **5 business days** of a Tier 1 model incident or significant performance deterioration
- Report model risk posture to executive leadership **quarterly**

### F.5 Model Validation Function
An independent team or qualified external party responsible for conducting independent model validation. The Model Validation Function shall be:
- Organisationally independent from model development functions, with no shared reporting lines below the CRO or CISO
- Staffed by individuals with sufficient quantitative, technical, and domain expertise to evaluate the models assigned to them
- Empowered to access all model documentation, data, code, and personnel necessary to conduct a complete validation

The Model Validation Function shall issue validation reports with findings classified by severity, recommend approval conditions or outright rejection, and escalate unresolved findings to the Model Risk Committee. The function shall not be responsible for model development or remediation.

### F.6 Model Owners
Each model in the inventory shall have a designated Model Owner accountable for that model's lifecycle governance. Model Owners shall:
- Maintain comprehensive and current model documentation throughout the lifecycle
- Submit models for validation and coordinate with the Model Validation Function
- Manage model use to ensure outputs are applied only within validated scope
- Monitor model performance against defined metrics and escalate anomalies **within 48 hours** of detection
- Disclose model limitations to all users and decision-makers in writing before operational use
- Obtain Model Risk Committee approval before implementing any material change
- Initiate and execute retirement procedures upon model decommissioning

### F.7 Model Developers
Shall design and build models in accordance with this policy's development standards. Shall document all design decisions, data choices, assumptions, and limitations during development. Shall cooperate fully with the Model Validation Function and not impede or influence validation findings. Shall not conduct their own independent validation.

### F.8 Model Users
Shall use model outputs only for the documented intended purpose and within validated scope. Shall complete model-specific user training before accessing outputs for decision-making. Shall report unexpected outputs, anomalies, or concerns to the Model Owner **within 24 hours**. Shall not modify model outputs through undocumented adjustments.

### F.9 GRC Team
Shall maintain the Model Inventory in the GRC platform, coordinate the tier assessment process, track validation status and open findings, produce compliance reporting, and manage the exceptions log. Shall conduct **quarterly** inventory completeness reviews.

### F.10 Legal Counsel
Shall advise on regulatory obligations applicable to specific models, including EU AI Act conformity requirements for AI/ML models. Shall review validation reports for Tier 1 AI/ML models before deployment authorisation. Shall ensure contractual model governance obligations are embedded in third-party agreements.

---

## G. Model Lifecycle Requirements

### G.1 Model Identification and Registration

- Any employee, contractor, or third party initiating development, procurement, or integration of an in-scope model shall notify the GRC Team **within 5 business days** of project initiation.
- The GRC Team shall register the model in the Model Inventory with an initial tier designation within **10 business days** of notification.
- Tier designation proposals shall be submitted to the Model Risk Committee for approval at the next quarterly meeting, or within **15 business days** for Tier 1 models given the need for pre-deployment validation.
- Models inherited through acquisition (including the Veridian AI models) shall be registered **within 30 days** of acquisition close and treated as requiring validation unless independent validation documentation meeting this policy's standards can be produced for CRO review.

### G.2 Model Development Standards

All in-scope models shall be developed in accordance with the following minimum standards:

**G.2.1 Conceptual Soundness**
- The model's theoretical basis shall be grounded in established academic or industry knowledge, with documented justification for design choices where alternative approaches exist.
- Key assumptions shall be identified, explicitly documented, and tested for sensitivity: including the consequences of assumption violations on model outputs.
- The model's intended use, scope, and boundaries shall be defined before development begins and maintained as a controlled document throughout the lifecycle.

**G.2.2 Data Requirements**
- Training, validation, and test datasets shall be documented for provenance, coverage, completeness, and known limitations before model development commences.
- Data selection decisions shall be documented, including what data was excluded and why.
- Training data shall be assessed for representativeness of the intended deployment population and evaluated for historical bias that may propagate to model outputs.
- For AI/ML models, datasets shall comply with the data governance requirements of the AI Governance Policy Section F.3 (Conformity Assessment: Data Governance) in addition to the requirements of this section.
- Data used in model development shall be stored, classified, and protected in accordance with the Data Classification Policy.

**G.2.3 Model Testing**
- Models shall be tested before validation submission using held-out data not used in training, with test results documented in the development documentation package.
- Developers shall conduct sensitivity analysis to assess how outputs change under varying input assumptions.
- For AI/ML models, developers shall conduct bias testing across relevant demographic subgroups and document findings, including any limitations that could not be fully resolved.
- Testing shall cover both expected operating conditions and plausible stress or edge case conditions.

**G.2.4 Development Documentation Package**
The Model Owner shall assemble a development documentation package before submitting the model for validation. For Tier 1 and Tier 2 models, the package shall include:
- Model purpose, intended use, and scope of applicability
- Theoretical and conceptual basis with references
- Data documentation (provenance, selection rationale, known gaps, bias assessment)
- Model architecture or methodology description (sufficient for a knowledgeable third party to reconstruct the model)
- Developer testing results, including performance metrics and stress testing outcomes
- Known limitations and conditions under which outputs may be less reliable
- Proposed monitoring metrics and thresholds
- Proposed user training requirements
- For AI/ML models: EU AI Act Article 11 technical documentation where applicable

Tier 3 models shall complete a simplified self-assessment documentation form approved by the Model Risk Committee.

### G.3 Independent Validation

**G.3.1 Validation Scope**
Independent validation shall be required for all Tier 1 and Tier 2 models before deployment authorisation. Validation shall cover:

1. **Conceptual soundness review:** Assessment of the model's theoretical basis, design choices, assumptions, and their appropriateness for the intended use.
2. **Data review:** Evaluation of training and test data quality, representativeness, bias exposure, and governance practices.
3. **Replication and testing:** Independent replication of key developer tests and conduct of additional validation-specific tests, including benchmarking against alternative approaches and backtesting where applicable.
4. **Performance evaluation:** Assessment of model accuracy, robustness, stability, and sensitivity across defined operating conditions, including stress conditions.
5. **Limitation assessment:** Independent identification of model limitations and evaluation of whether the developer's limitation disclosures are complete and accurate.
6. **Monitoring adequacy review:** Assessment of whether proposed monitoring metrics and thresholds are sufficient to detect performance deterioration.
7. **Documentation review:** Evaluation of whether the development documentation package is complete, accurate, and sufficient for informed use and governance.
8. **For AI/ML Tier 1 models:** Assessment of explainability adequacy, human oversight mechanism design, and alignment with EU AI Act conformity requirements.

**G.3.2 Validation Findings Classification**

| Finding Severity | Description | Deployment Implication |
|-----------------|-------------|----------------------|
| **Critical** | Fundamental flaw in conceptual soundness, data integrity, or performance that renders the model unfit for deployment | Deployment blocked; model returned for remediation |
| **High** | Significant limitation or gap that must be resolved or formally accepted with compensating controls before deployment | Deployment conditional on remediation or formal risk acceptance by CRO |
| **Medium** | Notable limitation that should be addressed; deployment may proceed with documented compensating controls and remediation timeline | Deployment permitted with Model Risk Committee-approved remediation plan |
| **Low** | Minor observation or enhancement opportunity; no deployment restriction | Documented for tracking; resolved at next validation cycle |

**G.3.3 Validation Report and Approval**
The Model Validation Function shall issue a validation report within **30 business days** of receiving a complete documentation package (Tier 1) or **20 business days** (Tier 2). The report shall include findings by severity, a summary opinion on model fitness for deployment, and recommended approval conditions.

Validation reports shall be reviewed by Legal Counsel (Tier 1 AI/ML models) and submitted to the Model Risk Committee for deployment authorisation decision.

**G.3.4 Revalidation Triggers**
Formal revalidation shall be required when:
- A material change is made to the model's inputs, outputs, algorithms, training data, intended use, or deployment environment
- The periodic revalidation schedule is reached (Tier 1: ≤24 months; Tier 2: ≤36 months)
- Post-market monitoring detects performance deterioration exceeding defined thresholds
- A model-related incident reveals a potential validation gap
- The Model Risk Committee determines that changed conditions warrant revalidation

### G.4 Model Deployment Authorisation

No Tier 1 or Tier 2 model shall be deployed into production without written deployment authorisation from the Model Risk Committee. The authorisation process requires:

1. Completed development documentation package (GRC Team confirms completeness)
2. Completed independent validation report with no unresolved Critical findings
3. CRO review and formal risk acceptance for any High findings proceeding with compensating controls
4. Legal Counsel sign-off for AI/ML Tier 1 models (EU AI Act conformity alignment)
5. Model Risk Committee deployment authorisation decision
6. Completed user training for all designated Model Users
7. Monitoring infrastructure confirmed operational before go-live

For Tier 3 models, the GRC Team shall issue deployment notification within **10 business days** of receiving the completed self-assessment documentation.

Models operated by Emyzer Nexus under interim arrangements (including inherited Veridian AI models) shall be subject to enhanced quarterly monitoring by the Model Risk Committee until full deployment authorisation under this policy is obtained.

### G.5 Model Use Management

- Model outputs shall be used only for their documented intended purpose and within the validated scope of applicability.
- Any proposed use of a model outside its validated scope requires written Model Risk Committee approval and updated validation before such use commences.
- Model limitations disclosed in the validation report and development documentation shall be communicated to all Model Users in writing before they access model outputs. Model Owners shall maintain records of limitation disclosure **for each user**.
- Model Users shall complete model-specific training, covering the model's purpose, scope, limitations, and interpretation of outputs, before operational access is granted. Training completion shall be recorded in the Learning Management System.
- Decisions informed by model outputs shall retain meaningful human review for Tier 1 models. Fully automated decision pipelines based on Tier 1 model outputs require explicit Model Risk Committee approval and shall be documented as a high-risk automation in the AI System Inventory.

### G.6 Overlays and Adjustments

When Model Users or Owners determine that model outputs require adjustment due to known limitations, changed conditions, or expert judgement, the following requirements apply:

- All overlays and adjustments shall be **documented** at the time of application, including the basis for the adjustment, the magnitude, and the name of the approving authority.
- Overlays shall be **time-limited**, with a defined review date not exceeding **90 days** from application. Overlays persisting beyond 90 days require renewed approval.
- The Model Owner shall maintain an **overlay log** and submit a summary to the Model Risk Committee **quarterly**.
- Recurring overlays in the same direction may indicate systematic model bias or drift and shall trigger a formal investigation by the Model Validation Function.
- Overlays shall not be used to mask model failures. Where a model consistently requires adjustment to produce acceptable outputs, the Model Owner shall initiate a formal model review.

### G.7 Ongoing Model Monitoring

**G.7.1 Monitoring Cadence**

| Monitoring Activity | Tier 1 | Tier 2 | Tier 3 |
|--------------------|--------|--------|--------|
| Performance metric review | Monthly | Quarterly | Annually |
| Statistical drift assessment | Quarterly | Semi-annually | Annually |
| Bias testing | Quarterly | Semi-annually | On material change |
| Override and overlay log review | Monthly | Quarterly | Annually |
| Limitation disclosure currency review | Quarterly | Annually | Annually |
| Full revalidation (maximum interval) | 24 months | 36 months | On material change |

**G.7.2 Performance Metrics**
Model Owners shall define, document, and obtain Model Risk Committee approval for:
- Primary performance metrics relevant to the model's purpose (e.g., accuracy, F1 score, AUC, calibration for predictive models)
- Amber alert thresholds triggering enhanced monitoring and Model Owner investigation
- Red alert thresholds triggering escalation to the CRO and Model Risk Committee review within **5 business days**
- Input data quality metrics monitoring for data drift relative to training distribution

Performance metrics and thresholds shall be defined at deployment and reviewed **annually** or upon material change.

**G.7.3 Escalation Requirements**
The Model Owner shall escalate to the CRO and Model Risk Committee within the following timeframes:

| Condition | Escalation Timeframe |
|-----------|---------------------|
| Red alert threshold breached | 5 business days |
| Unexpected outputs detected by Model Users | 48 hours of report receipt |
| Data supply disruption affecting model inputs | 48 hours of detection |
| Third-party model provider incident notification received | 24 hours |
| Regulatory inquiry or enforcement action related to model | 24 hours |
| Model-related customer complaint indicating potential harm | 48 hours |

**G.7.4 Monitoring Reports**
Model Owners shall submit monitoring reports to the Model Risk Committee on the schedule defined in G.7.1. Monitoring reports shall include: performance metrics vs. thresholds, drift assessment findings, bias testing results, overlay log summary, open finding status, and any escalations since the last report. The GRC Team shall consolidate monitoring reports into a portfolio-level summary for the Model Risk Committee quarterly review.

### G.8 Model Incident Management

AI/ML model incidents shall be managed through the Incident Management Policy and AI Governance Policy Section F.7 (Incident Management for AI Systems). Non-AI model incidents shall be managed through the Incident Management Policy with the following model-specific requirements:

- Model incidents include: outputs that are materially inaccurate and influenced a business decision; detection of systematic bias in model outputs; unexpected model behaviour; data supply failures affecting model reliability; and third-party model provider failures.
- Model incidents shall be classified using the standard severity framework with model-specific context: a Tier 1 model producing materially inaccurate outputs that influenced a customer-facing decision shall be classified as **High** at minimum.
- Post-incident reviews for High and Critical model incidents shall include root cause analysis specific to model failure modes, conceptual error, data quality failure, out-of-scope use, monitoring failure, or operator error, completed **within 5 business days** of incident resolution.
- Lessons learned from model incidents shall be reviewed by the Model Risk Committee and incorporated into validation standards and monitoring protocols where relevant.

### G.9 Model Retirement

Models shall be formally retired through a documented process approved by the Model Risk Committee. No model shall be decommissioned without completed retirement documentation. The retirement process shall include:

1. **Business justification:** Model Owner documents the reason for retirement (replacement, decommission, scope elimination) and confirms no ongoing business use.
2. **Stakeholder notification:** Affected business units, Model Users, and, where outputs have informed customer-facing decisions, relevant stakeholders are notified **no less than 30 days** before retirement, unless operational circumstances require emergency retirement.
3. **Decision reconciliation:** Model Owner assesses whether decisions based on model outputs have ongoing implications that require disclosure, review, or correction. Findings documented and submitted to the CRO.
4. **Data disposition:** Training data, model artefacts, test datasets, and operational data are disposed of in accordance with the Data Classification Policy and applicable retention schedules. Disposition certificates are retained.
5. **Documentation archival:** Development documentation, validation reports, performance monitoring history, overlay logs, and incident records are archived for the retention periods defined in Section N (Evidence of Compliance).
6. **Inventory update:** The model is transferred to the retired model record in the Model Inventory within **5 business days** of retirement completion.

Emergency retirement, required when a model poses immediate risk of material harm, may be authorised by the CRO without prior Model Risk Committee approval, with full documentation and committee review completed **within 10 business days** of retirement.

---

## H. Third-Party Model Governance

Third-party models (including vendor-developed models, open-source models, and models accessed via API) shall be subject to the following requirements in addition to standard Third-Party Risk Management Policy obligations:

- **Pre-procurement assessment:** Before procuring or integrating any third-party model, the AI Governance Committee and Model Risk Committee shall jointly assess: intended use alignment, tier classification, available validation documentation, vendor transparency practices, data handling obligations, and contractual liability for model errors.
- **Tier assignment:** Third-party models shall be tiered using the same criteria as internally developed models. The unavailability of vendor validation documentation is itself a Tier 1 risk indicator.
- **Vendor validation documentation:** For Tier 1 and Tier 2 third-party models, Emyzer Nexus shall require vendors to provide validation documentation meeting this policy's standards, or shall conduct its own independent validation before deployment.
- **Contractual requirements:** Agreements with third-party model providers shall include: performance warranty provisions, incident notification obligations (within 24 hours of detection), audit and documentation access rights, data processing terms, liability provisions for model errors, and the right to terminate if the provider fails to meet governance obligations.
- **Ongoing monitoring:** Third-party models shall be subject to post-deployment monitoring at frequencies determined by their tier. Monitoring shall include vendor performance reporting, independent performance testing on Emyzer Nexus data, and annual vendor due diligence refresh.
- **API-based models (LLMs):** Large language model APIs classified as High-Risk under the EU AI Act shall be managed under both this policy and the AI Governance Policy. Emyzer Nexus shall document LLM-specific limitations, including hallucination rates, output variability, training data cutoffs, and restricted explainability, and implement compensating controls including human review of all outputs informing material decisions.

---

## I. Compliance and Monitoring

### I.1 Monitoring Activities

| Activity | Frequency | Owner |
|----------|-----------|-------|
| Model Inventory completeness review | Quarterly | GRC Team |
| Tier 1 model performance report review | Monthly | Model Risk Committee |
| Tier 2 model performance report review | Quarterly | Model Risk Committee |
| Tier 1 bias testing review | Quarterly | Model Risk Committee |
| Open validation finding status review | Quarterly | GRC Team / Model Risk Committee |
| Overlay log review | Quarterly | Model Risk Committee |
| Exception register review | Quarterly | CRO |
| Policy compliance audit (as part of ISMS audit) | Annual | Internal Audit |

### I.2 Key Performance Indicators

| KPI | Target | Frequency |
|-----|--------|-----------|
| Model Inventory completeness | 100% | Quarterly |
| Tier 1 models with current independent validation | 100% | Quarterly |
| Tier 2 models with current independent validation | 100% | Quarterly |
| Models deployed without deployment authorisation | 0 | Continuous |
| Model Users without completed training | 0 | Monthly (Tier 1); Quarterly (Tier 2) |
| Red alert escalations reviewed within 5 business days | 100% | Per event |
| Tier 1 monitoring reports submitted on schedule | 100% | Monthly |
| Open Critical validation findings | 0 | Continuous |
| Open High validation findings with approved remediation plan | 100% | Quarterly |
| Overlay log submissions on schedule | 100% | Quarterly |

### I.3 Non-Compliance

Deployment of a Tier 1 or Tier 2 model without completed validation and Model Risk Committee authorisation constitutes a critical compliance failure, triggering immediate escalation to the CRO and model suspension. Other non-compliance shall be addressed through documented corrective action plans within **30 days** of identification. Persistent or wilful non-compliance may result in model suspension, removal of model access rights, and disciplinary action.

---

## J. Policy Exceptions

### J.1 Exception Process
Exceptions to this policy require:
1. Submission of a completed exception request via **ServiceNow GRC workflow**, including business justification, model-specific risk assessment, and proposed compensating controls.
2. CRO approval. Exceptions affecting Tier 1 models require Model Risk Committee review before CRO approval.
3. Exceptions are valid for a maximum of **90 days** and may be renewed once with updated justification and reassessment.
4. No exception shall permit continued deployment of a Tier 1 model with an unresolved Critical validation finding.

### J.2 Exception Governance
- Active exceptions reviewed **quarterly** by the Model Risk Committee.
- Each exception shall include a remediation plan with a target closure date not exceeding **180 days** from initial approval.
- Exception register maintained in the GRC platform with monthly status updates to executive leadership.

---

## K. Related Policies

1. [**AI Governance Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/ai-governance-policy.md) *(KB-PORTFOLIO-0011)*: Parent strategic framework for AI and ML systems. The Model Risk Policy provides the operational model lifecycle controls subordinate to the AI Governance Policy for all AI/ML systems that also meet the definition of a model.

2. [**Information Security Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/information-security-policy.md): Grandparent policy establishing the ISMS framework and governance structure within which this policy operates.

3. [**Risk Management Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/risk-management-policy.md): Defines the enterprise risk framework applied to model risk as a distinct risk category. Model risk findings feed the enterprise risk register under the ownership of the CRO.

4. [**Third-Party Risk Management Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/third-party-risk-management-policy.md): Governs vendor risk management requirements extended by the AI Vendor Risk Due Diligence Addendum for third-party model-specific obligations.

5. [**Data Classification Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/data-classification-policy.md): Governs the classification, handling, and protection of training data, model artefacts, validation data, and model outputs.

6. [**Incident Management Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/incident-management-policy.md): Defines incident response procedures extended to cover model-specific failure modes.

---

## L. Related Documents

1. Model Inventory and Tiering Register
2. Model Development Documentation Template (Tier 1/2)
3. Model Self-Assessment Form (Tier 3)
4. Independent Validation Report Template
5. Model Deployment Authorisation Checklist
6. Model Monitoring Procedures
7. Overlay and Adjustment Log Template
8. Model Incident Response Runbook
9. Model Retirement Checklist
10. Third-Party Model Due Diligence Checklist
11. AI Vendor Risk Due Diligence Addendum
12. Model Risk Committee Terms of Reference

---

## M. Review and Revision

This policy shall be reviewed **annually** or upon: a significant model-related incident revealing governance gaps; material changes to the organisation's model portfolio; relevant changes to SR 11-7 guidance, EU AI Act implementing acts, or ISO/IEC 42001; or changes to the AI Governance Policy that affect model-level obligations. All revisions require CEO approval. Changes affecting Tier 1 model obligations shall be communicated to Model Owners and the Model Validation Function **within 14 days** of revision.

---

## N. Framework Alignment

| Framework | Alignment |
|-----------|-----------|
| **SR 11-7 (Federal Reserve / OCC)** | Section I (Model Risk Management Framework), Section II (Model Development, Implementation, and Use, conceptual soundness, data quality, testing), Section III (Model Validation, independence, scope, findings classification), Section IV (Governance, Policies, and Controls, inventory, tiering, oversight, vendor models) |
| **NIST AI RMF 1.0** | GOVERN 1.1–1.7 (model risk governance culture and structures), MAP 1.5–3.5 (model risk identification and context), MEASURE 2.1–2.13 (model performance measurement, bias, drift), MANAGE 1.3–4.2 (model risk treatment, monitoring, incident response, retirement) |
| **EU AI Act (Regulation 2024/1689)** | Article 9 (Risk Management System), Article 10 (Data Governance for training data), Article 11 (Technical Documentation), Article 15 (Accuracy, Robustness, Cybersecurity), Article 72 (Post-Market Monitoring operationalised as ongoing model monitoring) |
| **ISO/IEC 42001:2023** | Clause 8.4 (AI system lifecycle: design, development, testing), Clause 8.6 (AI system operation monitoring), Annex A Controls A.6 (AI risk management operationalisation), A.7 (AI system impact assessment) |
| **ISO/IEC 23894:2023** | Risk identification (model failure modes), Risk treatment (validation, monitoring, overlay governance), Risk communication (limitation disclosure) |
| **ISO/IEC 27001:2022** | A.8.25–A.8.28 (Secure development lifecycle extended to model development), A.5.19–A.5.22 (Supplier relationships extended to third-party model vendors) |

---

## O. Organisational Benefit

| Benefit Area | Description |
|--------------|-------------|
| **Decision Quality** | Ensures models informing business decisions are validated, fit for purpose, and operating within known performance bounds: reducing the risk of decisions based on systematically flawed outputs |
| **Acquisition Risk Control** | Provides a structured mechanism for assessing, validating, and governing the Veridian AI models operating under interim arrangements, converting an unquantified inherited risk into a managed one |
| **Regulatory Compliance** | Operationalises EU AI Act technical documentation, monitoring, and accuracy obligations at the model level; SR 11-7 alignment demonstrates governance maturity to regulated-industry clients and partners |
| **Customer Protection** | Bias testing, performance monitoring, limitation disclosure, and human oversight requirements reduce the risk of model outputs causing harm to customers or counterparties |
| **Auditability** | Comprehensive documentation, validation records, and evidence retention requirements ensure the organisation can demonstrate model governance to internal audit, external auditors, and regulators |
| **Talent and Credibility** | A structured model risk program positions Emyzer Nexus as a sophisticated operator capable of governing advanced AI systems: a differentiator when competing for regulated-industry contracts or enterprise partnerships |
| **Incident Containment** | Clear escalation triggers, monitoring thresholds, and retirement procedures reduce the time between model failure detection and response, limiting the blast radius of model-related incidents |
| **Third-Party Confidence** | Contractual model governance requirements and due diligence standards reduce dependency on undocumented vendor model quality claims |

---

## P. Evidence of Compliance

The organisation shall maintain the following compliance evidence with defined retention periods:

| Evidence Type | System of Record | Owner | Retention Period |
|---------------|------------------|-------|------------------|
| Model Inventory and Tiering Register | GRC Platform | GRC Team | Indefinite (with full history) |
| Tier Assignment Decisions | GRC Platform | Model Risk Committee | Life of model + 7 years |
| Development Documentation Packages | Document Repository | Model Owner | Life of model + 7 years |
| Independent Validation Reports | Document Repository | Model Validation Function | Life of model + 7 years |
| Deployment Authorisation Records | GRC Platform | Model Risk Committee | Life of model + 7 years |
| Model User Training Records | Learning Management System | Human Resources | 3 years |
| Limitation Disclosure Records | GRC Platform | Model Owner | Life of model + 3 years |
| Model Performance Monitoring Reports | GRC Platform | Model Owner | 5 years |
| Drift and Bias Testing Records | Document Repository | Model Owner | 5 years |
| Overlay and Adjustment Logs | GRC Platform | Model Owner | 3 years |
| Model Risk Committee Minutes | Document Repository | CRO | 7 years |
| Model Incident Reports | ServiceNow ITSM | Information Security Team | 10 years |
| Post-Incident Review Reports | Document Repository | Information Security Team | 10 years |
| Third-Party Model Due Diligence Records | GRC Platform | Procurement / GRC Team | Contract + 5 years |
| Third-Party Model Contracts | Legal Repository | Legal Counsel | Contract + 7 years |
| Model Retirement Records | Document Repository | Model Owner | 7 years |
| Exception Records | GRC Platform | CRO | Exception duration + 3 years |
| Annual Compliance Audit Reports | GRC Platform | Internal Audit | 7 years |
| Policy Acknowledgements | GRC Platform / HR System | Human Resources | Employment + 3 years |

---

## Approval History

| Date | Approver | Status | Comments |
|------|----------|--------|----------|
| 2025-09-01 | Chief Executive Officer | Approved | "The tiering framework and validation independence requirements are appropriate for the scale and nature of models we're operating, including those inherited from Veridian AI. The SR 11-7 alignment demonstrates the governance standard expected by our enterprise and regulated-sector clients. Approved." |

---

## Document Control

- **Document ID:** KB-PORTFOLIO-0012
- **Version:** 1.0
- **Classification:** Internal
- **Last Updated:** 2025-09-01
- **Next Review Date:** 2026-09-01

---

*This policy document was developed as part of the Emyzer Nexus Phase 2 GRC program and formatted for portfolio presentation. It is subordinate to the AI Governance Policy (KB-PORTFOLIO-0011) and operates within the ISMS established by the Information Security Policy.*

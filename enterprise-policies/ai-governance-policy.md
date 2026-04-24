# AI Governance Policy

**Emyzer Nexus – Governance, Risk, and Compliance**

---

## Policy Metadata

| Attribute | Value |
|-----------|-------|
| **Policy Name** | AI Governance Policy |
| **Type** | Policy |
| **Version** | 1.0 |
| **Parent Policy** | Information Security Policy |
| **Owner** | Chief Information Security Officer |
| **Owning Group** | App Engine Admins |
| **State** | Published |
| **Valid From** | 2025-06-01 |
| **Valid To** | 2026-06-01 |
| **Approvers** | Chief Executive Officer |
| **Reviewers** | Chief Risk Officer; GRC Analyst; Legal Counsel |
| **Knowledge Base** | Governance, Risk, and Compliance |
| **Published Policy** | KB-PORTFOLIO-0011 |

---

## Description

This policy establishes the governance framework for the responsible development, acquisition, deployment, monitoring, and retirement of artificial intelligence and machine learning systems across Emyzer Nexus and its subsidiaries.

**Impact:** Ensures AI systems operated by Emyzer Nexus are developed and deployed responsibly, with appropriate human oversight, transparency, and accountability. Supports compliance with the EU AI Act, protects against model-related risks inherited through the acquisition of Veridian AI, and positions the organization to meet emerging regulatory obligations as the global AI governance landscape matures.

**Relevant Standards:** EU AI Act (Regulation 2024/1689), NIST AI Risk Management Framework (AI RMF 1.0), ISO/IEC 42001:2023, ISO/IEC 27001:2022

---

## Policy Snapshot

| Dimension | Summary |
|-----------|---------|
| **Applies to** | All Emyzer Nexus business units, subsidiaries (including Emyzer Technology), acquired entities (including Veridian AI systems), employees, contractors, and third parties involved in the development, procurement, deployment, or operation of AI systems |
| **Covers** | All AI and ML systems owned, operated, or procured by Emyzer Nexus, including systems inherited through the Veridian AI acquisition, third-party AI APIs, and AI features embedded in commercial software |
| **AI Risk Tiers** | Unacceptable Risk, High-Risk, Limited Risk, Minimal Risk — aligned to EU AI Act classification framework |
| **Review Cadence** | Annual policy review; AI system risk classifications reviewed upon material change; model performance reviewed on a cadence defined by risk tier |
| **Key Governance** | CISO provides executive oversight; AI Governance Committee owns program operations; AI System Owners manage lifecycle compliance; Legal Counsel ensures regulatory alignment |
| **Exceptions Process** | ServiceNow workflow with CISO approval; maximum 90-day duration; quarterly review of active exceptions |
| **Evidence Maintained** | AI system inventory, risk classifications, conformity assessments, model performance reports, human oversight logs, incident records, retirement documentation (all with defined retention periods) |

---

## A. Purpose

To establish a comprehensive governance framework for artificial intelligence and machine learning systems across Emyzer Nexus, ensuring that AI systems are designed, deployed, and operated in a manner that is lawful, ethical, transparent, and accountable. This policy operationalizes the organization's obligations under the EU AI Act, aligns AI risk management practices with the NIST AI Risk Management Framework (AI RMF 1.0), and integrates AI governance into the existing Information Security Management System (ISMS).

The policy reflects Emyzer Nexus's recognition that AI systems present distinct governance challenges not fully addressed by traditional information security frameworks — including model drift, training data bias, explainability limitations, and the opacity of third-party large language model APIs. It establishes the structures and controls required to manage these challenges responsibly and to maintain stakeholder trust as the organization's AI footprint evolves.

---

## B. Scope

This policy applies to all artificial intelligence and machine learning systems that Emyzer Nexus owns, operates, procures, or embeds in products and services, including:

- AI systems developed internally by Emyzer Technology or acquired through the Veridian AI integration
- Third-party AI systems and large language model APIs integrated into organizational workflows or customer-facing products
- AI features embedded within commercial software operated by the organization
- AI systems used in human resources, finance, legal, security, or customer-facing functions

**Systems specifically in scope at time of publication:**

| System | Origin | EU AI Act Risk Tier |
|--------|--------|---------------------|
| Predictive Customer Churn Model | Veridian AI (acquired) | High-Risk |
| AI-Assisted Contract Review Tool | Veridian AI (acquired) | High-Risk |

**Third-party applicability:** Third parties developing, supplying, or operating AI systems on behalf of Emyzer Nexus shall comply with the governance requirements defined in this policy through contractual obligations, including conformity documentation, bias audit availability, and incident notification requirements. AI-specific due diligence requirements are detailed in the AI Vendor Risk Due Diligence Addendum.

**Exclusions:** Rule-based automation systems that do not use machine learning or statistical inference are excluded from this policy. Applicability of exclusions shall be assessed by the AI Governance Committee on a case-by-case basis.

---

## C. Definitions

| Term | Definition |
|------|------------|
| **Artificial Intelligence (AI) System** | A machine-based system that, for a given set of objectives, makes predictions, recommendations, decisions, or generates content influencing real or virtual environments. As defined in EU AI Act Article 3(1). |
| **Machine Learning (ML)** | A subset of AI in which systems learn from data to improve performance on tasks without being explicitly programmed for each scenario. |
| **EU AI Act** | Regulation (EU) 2024/1689 of the European Parliament and of the Council, establishing harmonised rules on artificial intelligence. The first comprehensive AI regulatory framework in the European Union. |
| **NIST AI RMF** | The NIST Artificial Intelligence Risk Management Framework (AI RMF 1.0), a voluntary framework providing guidance for managing risks throughout the AI lifecycle, structured around four core functions: Govern, Map, Measure, and Manage. |
| **High-Risk AI System** | An AI system classified under Annex III of the EU AI Act as posing significant risks to health, safety, or fundamental rights, subject to mandatory conformity obligations before deployment. |
| **AI Risk Classification** | The process of categorising an AI system according to EU AI Act risk tiers (Unacceptable Risk, High-Risk, Limited Risk, Minimal Risk) to determine applicable governance obligations. |
| **AI System Inventory** | The formal register of all AI systems owned, operated, or procured by Emyzer Nexus, including risk classifications, ownership, and lifecycle status. |
| **Model Drift** | Degradation in AI model performance over time due to changes in the underlying data distribution, resulting in predictions or outputs that no longer reflect current conditions. |
| **Training Data Bias** | Systematic errors in AI model outputs caused by imbalances, exclusions, or historical prejudices present in the data used to train the model. |
| **Human Oversight** | Mechanisms ensuring that humans can understand, monitor, intervene in, and where necessary override AI system outputs and decisions. As required under EU AI Act Article 14. |
| **Explainability** | The degree to which the logic, inputs, and outputs of an AI system can be understood and explained to affected parties in meaningful terms. |
| **Conformity Assessment** | A mandatory evaluation process under the EU AI Act establishing that a high-risk AI system meets the requirements of the regulation before being placed on the market or put into service. |
| **AI System Owner** | The individual accountable for a specific AI system's lifecycle governance, including classification, compliance, monitoring, and retirement. |
| **Foundation Model / Large Language Model (LLM)** | A large-scale AI model trained on broad datasets capable of performing a wide range of tasks, often accessed via API. Subject to specific transparency and governance obligations under the EU AI Act. |
| **Post-Market Monitoring** | Ongoing collection and analysis of data on the performance, behaviour, and impacts of an AI system after deployment, as required under EU AI Act Article 72. |

---

## D. Policy Statement

Emyzer Nexus is committed to governing artificial intelligence systems in a manner that is responsible, transparent, and aligned with applicable law and ethical principles. The organization shall:

1. Maintain a complete and current **AI System Inventory**, classifying all AI systems according to EU AI Act risk tiers within **30 days** of identification, acquisition, or material change.

2. Apply governance controls **proportionate to risk classification**, with the most stringent requirements applied to High-Risk systems, including mandatory conformity assessments, human oversight mechanisms, and post-market monitoring programs.

3. Prohibit the development or deployment of AI systems that fall within the **Unacceptable Risk** tier as defined in EU AI Act Title II, including systems that manipulate individuals through subliminal techniques, exploit vulnerabilities of specific groups, or are used for prohibited real-time biometric surveillance in public spaces.

4. Ensure all High-Risk AI systems are subject to a documented **conformity assessment** before deployment or continued operation following material change, including validation of training data quality, technical documentation, human oversight controls, and accuracy and robustness testing.

5. Embed **human oversight** into all High-Risk AI systems, ensuring that human operators can understand the system's outputs, identify failures or unexpected behaviour, and intervene or override decisions where required.

6. Require **explainability** appropriate to the use case and affected population, with High-Risk systems providing meaningful explanations of decisions to affected individuals where technically feasible.

7. Maintain **post-market monitoring** for all deployed AI systems, with monitoring frequency and depth calibrated to risk tier, and with a documented process for detecting and responding to model drift, bias emergence, or unexpected outputs.

8. Integrate AI system risk into the **enterprise risk register**, treating AI-specific risks (model drift, training data bias, third-party model dependency, explainability gaps) as distinct risk categories subject to the organization's risk management framework.

9. Ensure AI system **retirement** is governed through a formal process that includes data disposition, documentation archival, and stakeholder notification where decisions or outputs of the retired system may have ongoing implications.

10. Review and update this policy **annually** or upon material changes to the EU AI Act implementing acts, organisational AI strategy, or following a significant AI-related incident.

---

## E. Roles and Responsibilities

### E.1 Chief Executive Officer (CEO)
Provides board-level accountability for responsible AI governance across Emyzer Nexus. Shall approve the AI Governance Policy and material changes to organizational AI strategy. Shall receive **quarterly** briefings on AI risk posture and compliance status from the CISO.

### E.2 Chief Information Security Officer (CISO)
Provides executive oversight of the AI governance program. Shall chair the AI Governance Committee. Shall approve AI risk acceptance decisions for High-Risk systems, escalate unresolvable compliance gaps to the CEO, and ensure alignment between AI governance and the ISMS. Shall report AI risk posture to executive leadership **monthly**.

### E.3 AI Governance Committee
A cross-functional committee chaired by the CISO, comprising the Chief Risk Officer, Legal Counsel, Chief Technology Officer, and representatives from affected business units. Shall meet **quarterly** to review the AI System Inventory, approve risk classifications, review conformity assessment outcomes, and assess emerging regulatory developments. Shall convene on an emergency basis within **5 business days** of a significant AI-related incident or regulatory development.

### E.4 Legal Counsel
Shall advise the AI Governance Committee on EU AI Act obligations, implementing acts, and regulatory developments. Shall review conformity assessments for High-Risk systems. Shall assess applicability of AI regulations to new systems at the point of procurement or development initiation. Shall ensure contractual AI governance obligations are embedded in vendor agreements.

### E.5 Chief Technology Officer (CTO)
Shall ensure technical AI governance requirements are integrated into system design, development, and procurement processes. Shall oversee the technical implementation of human oversight mechanisms, explainability tools, and post-market monitoring infrastructure. Shall approve technical documentation for High-Risk systems before submission to the AI Governance Committee.

### E.6 AI System Owners
Each AI system in the inventory shall have a designated AI System Owner accountable for that system's lifecycle governance. AI System Owners shall:
- Maintain accurate system documentation, including technical specifications, training data provenance, intended use, and known limitations
- Coordinate conformity assessments and submit findings to the AI Governance Committee
- Monitor system performance against defined metrics and escalate anomalies **within 48 hours** of detection
- Manage the human oversight program for their system, including operator training and override capability testing
- Initiate retirement procedures when a system is decommissioned

### E.7 GRC Team
Shall maintain the AI System Inventory in the GRC platform, coordinate AI risk assessments, produce compliance reporting, and track remediation of AI-related findings. Shall conduct **quarterly** reviews of inventory completeness and classification currency.

### E.8 All Employees
Shall complete AI awareness training **within 30 days** of hire and **annually** thereafter. Shall report unexpected AI system behaviour, outputs that appear biased or discriminatory, or suspected incidents **within 24 hours** of discovery through established reporting channels. Shall not deploy, integrate, or procure AI systems without prior AI Governance Committee review.

---

## F. Minimum AI Governance Requirements

The following requirements establish baseline controls across the AI system lifecycle. Detailed implementation procedures are maintained in the **AI Governance Procedures Manual** and related operational documentation.

### F.1 AI System Identification and Inventory

- Shall maintain a complete AI System Inventory in the GRC platform, updated **within 30 days** of identifying, acquiring, or materially changing any AI system.
- The inventory shall record, at minimum: system name, vendor or development origin, intended use case, affected populations, data inputs and outputs, deployment environment, EU AI Act risk tier classification, AI System Owner, deployment date, and review date.
- Shall conduct an **annual** inventory audit to identify shadow AI — AI features embedded in commercial software or adopted by business units without formal registration.
- All AI systems identified through inventory audit shall be classified and registered **within 60 days** of identification.

### F.2 AI Risk Classification

- Shall classify all AI systems according to EU AI Act risk tiers prior to deployment:
  - **Unacceptable Risk:** Prohibited. Shall not be developed or deployed.
  - **High-Risk:** Subject to full conformity requirements under this policy.
  - **Limited Risk:** Subject to transparency obligations; users must be informed they are interacting with an AI system.
  - **Minimal Risk:** Documented in inventory; standard information security controls apply.
- AI System Owners shall submit classification proposals to the AI Governance Committee for approval. The AI Governance Committee shall issue a classification decision **within 30 days** of submission.
- Classifications shall be reviewed upon any material change to the system's intended use, technical architecture, training data, or deployment context.

### F.3 Conformity Assessment (High-Risk Systems)

High-Risk AI systems shall undergo a documented conformity assessment before initial deployment and following any material change. The conformity assessment shall evaluate:

1. **Risk Management System:** Documentation that a risk management system aligned to EU AI Act Article 9 has been established and maintained throughout the system lifecycle.
2. **Data Governance:** Evidence that training, validation, and test datasets meet quality requirements, including examination of data provenance, completeness, representativeness, and known biases.
3. **Technical Documentation:** Complete technical documentation as required under EU AI Act Article 11, including system architecture, training methodology, performance metrics, and known limitations.
4. **Transparency and Instructions for Use:** Evidence that documentation for human operators is accurate, complete, and enables effective oversight.
5. **Human Oversight:** Demonstration that human oversight mechanisms are implemented, tested, and operational, including the ability to intervene or override system outputs.
6. **Accuracy, Robustness, and Cybersecurity:** Evidence that the system meets defined performance thresholds across relevant test conditions, including adversarial inputs.

Conformity assessment outcomes shall be reviewed by Legal Counsel and approved by the AI Governance Committee before deployment authorisation is issued.

### F.4 Human Oversight

- All High-Risk AI systems shall implement human oversight mechanisms enabling operators to:
  - Fully understand the system's capabilities and limitations before operation
  - Monitor the system's performance during operation
  - Identify and respond to anomalies, failures, or unexpected outputs
  - Disregard, override, or suspend system outputs where required
  - Halt the system in cases of serious risk
- Human oversight procedures shall be documented and validated **at deployment** and **annually** thereafter.
- Operators of High-Risk AI systems shall complete role-specific training **before** being granted operational access. Training completion records shall be maintained for 3 years.
- Override events shall be logged, reviewed **within 5 business days**, and reported to the AI Governance Committee **quarterly**.

### F.5 Explainability

- AI System Owners shall define an explainability standard appropriate to the system's use case and the characteristics of affected populations, documented at the time of conformity assessment.
- For High-Risk systems making decisions that significantly affect individuals, the organisation shall implement mechanisms to provide meaningful explanations of outputs to affected parties upon request, to the extent technically feasible.
- Where full algorithmic explainability is not technically feasible (as may be the case for third-party LLM APIs), the AI System Owner shall document this limitation, implement compensating measures (such as human review of outputs), and report the limitation to the AI Governance Committee.

### F.6 Post-Market Monitoring

- All deployed AI systems shall be subject to post-market monitoring at frequencies determined by risk tier:

| Risk Tier | Performance Review | Bias Audit | Drift Assessment |
|-----------|-------------------|------------|------------------|
| High-Risk | Monthly | Quarterly | Quarterly |
| Limited Risk | Quarterly | Annually | Semi-annually |
| Minimal Risk | Annually | Annually | Annually |

- Post-market monitoring shall include, at minimum: performance metric tracking against defined baselines, statistical analysis for data distribution drift, review of override logs and operator-reported anomalies, and bias testing across relevant subgroups.
- AI System Owners shall report monitoring outcomes to the AI Governance Committee **quarterly**.
- Where monitoring detects performance degradation, significant bias emergence, or unexpected outputs, the AI System Owner shall escalate to the CISO **within 48 hours** and initiate a formal investigation.

### F.7 Incident Management for AI Systems

- AI-specific incidents shall be managed through the Incident Management Policy with AI-specific extensions:
  - Model failure resulting in materially incorrect outputs affecting business decisions or individuals
  - Detection of significant bias in model outputs
  - Unauthorised access to or manipulation of training data or model artefacts
  - Third-party AI vendor security incident affecting model integrity or data confidentiality
  - Regulatory notification obligation triggered under EU AI Act Article 73
- AI incidents classified as High severity or above shall trigger a post-incident review **within 5 business days** of resolution, including root cause analysis specific to AI failure modes.
- Serious incidents involving High-Risk AI systems shall be reported to the relevant national market surveillance authority as required under EU AI Act Article 73, within the timeframes specified in applicable implementing acts.

### F.8 Third-Party AI Governance

- Third-party AI systems and APIs shall be subject to AI-specific due diligence as defined in the AI Vendor Risk Due Diligence Addendum, in addition to the standard Third-Party Risk Management Policy requirements.
- Before procuring or integrating any third-party AI system, the AI Governance Committee shall conduct an AI risk assessment covering: intended use alignment, EU AI Act risk classification, vendor transparency documentation, bias audit availability, data retention and processing practices, and contractual liability provisions for model errors.
- Contracts with third-party AI vendors shall include: EU AI Act compliance obligations, incident notification requirements, the right to audit model documentation, data processing terms aligned to the Data Classification Policy, and clear liability provisions for model failures.
- Third-party AI systems shall be registered in the AI System Inventory and subject to post-market monitoring obligations proportionate to their risk tier.

### F.9 AI System Retirement

- AI systems shall be formally retired through a documented process initiated by the AI System Owner and approved by the AI Governance Committee.
- The retirement process shall include:
  - Stakeholder notification, including affected business units and, where applicable, individuals affected by the system's decisions
  - Disposition of training data, model artefacts, and operational data in accordance with the Data Classification Policy and applicable retention schedules
  - Archival of technical documentation, conformity assessment records, and monitoring history in accordance with evidence retention requirements
  - Assessment of whether ongoing obligations exist in relation to past decisions made by the system
- Retired systems shall be removed from the AI System Inventory active register and transferred to a retired systems record retained for **7 years**.

### F.10 Prohibited AI Practices

The following AI practices are prohibited across Emyzer Nexus in accordance with EU AI Act Title II:

- AI systems that deploy subliminal techniques to manipulate individuals' behaviour in ways that harm them or others
- AI systems that exploit vulnerabilities of specific groups (age, disability, socioeconomic status) to distort their behaviour in ways that cause harm
- AI systems used for social scoring of individuals by public authorities or in contexts that lead to detrimental treatment
- Real-time remote biometric identification systems in publicly accessible spaces for law enforcement purposes (subject to narrow exceptions not applicable to Emyzer Nexus's business activities)
- AI systems that infer emotions of individuals in workplace or educational settings except for safety purposes
- Biometric categorisation systems that infer sensitive characteristics (race, political opinions, trade union membership, religious beliefs, sexual orientation)

Any request to develop, procure, or deploy a system that may fall within these categories shall be immediately referred to Legal Counsel and the CISO regardless of the requestor's seniority.

---

## G. Compliance and Monitoring

### G.1 Monitoring Activities

Compliance with this policy shall be monitored through:

- **Continuous:** AI incident monitoring via SIEM and AI System Owner reporting
- **Monthly:** CISO review of AI risk posture and open findings
- **Quarterly:** AI Governance Committee review of inventory, classification currency, conformity status, and monitoring outcomes
- **Annual:** Comprehensive AI governance program audit as part of ISMS internal audit; EU AI Act compliance gap assessment against current implementing acts

### G.2 Key Performance Indicators

| KPI | Target | Measurement Frequency |
|-----|--------|----------------------|
| AI System Inventory completeness | 100% | Quarterly |
| AI systems with current risk classification | 100% | Quarterly |
| High-Risk systems with approved conformity assessment | 100% | Quarterly |
| High-Risk systems with active post-market monitoring | 100% | Monthly |
| Operator training completion for High-Risk systems | 100% | Monthly |
| Override events reviewed within 5 business days | 100% | Monthly |
| AI incidents with post-incident review completed | 100% for High/Critical | Per incident |
| Third-party AI systems with current due diligence | ≥95% | Quarterly |

### G.3 Non-Compliance

Non-compliance with this policy shall be addressed through documented corrective action plans **within 30 days** of identification. Deployment of an AI system without completed classification and, where required, conformity assessment constitutes a critical compliance failure and shall trigger immediate escalation to the CISO and AI Governance Committee. Persistent or wilful non-compliance may result in system suspension and disciplinary action up to and including termination.

---

## H. Policy Exceptions

### H.1 Exception Request Process
Business units requiring temporary deviation from this policy shall:
1. Submit exception requests via **ServiceNow GRC workflow** with detailed business justification, AI-specific risk assessment, and proposed compensating controls.
2. Obtain approval from the CISO. Exceptions involving High-Risk AI systems require AI Governance Committee review before CISO approval.
3. Accept exceptions valid for a maximum of **90 days** unless formally renewed. Exceptions shall not permit deployment of an AI system in the High-Risk tier without a completed conformity assessment.
4. Implement and document compensating controls during the exception period.

### H.2 Exception Governance
- All active exceptions shall be reviewed **quarterly** by the AI Governance Committee.
- Exception renewals shall require updated business justification and risk assessment.
- Each exception shall include a remediation plan with a target closure date not exceeding **180 days** from initial approval.
- Exception tracking shall be maintained in the GRC platform with status updates provided to executive leadership **monthly**.

---

## I. Related Policies

1. [**Information Security Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/information-security-policy.md) — Parent policy establishing the ISMS framework and governance structure.

2. [**Risk Management Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/risk-management-policy.md) — Defines the enterprise risk assessment methodology applied to AI-specific risk categories, including model drift, training data bias, and third-party model dependency.

3. [**Third-Party Risk Management Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/third-party-risk-management-policy.md) — Establishes vendor risk requirements extended by the AI Vendor Risk Due Diligence Addendum for AI-specific third-party obligations.

4. [**Data Classification Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/data-classification-policy.md) — Governs the classification and handling of training data, model outputs, and AI system documentation.

5. [**Incident Management Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/incident-management-policy.md) — Defines incident response procedures extended to cover AI-specific failure modes and EU AI Act regulatory notification obligations.

6. **Model Risk Policy** — Operational policy governing the detailed model lifecycle, bias testing cadence, and explainability standards. (Phase 2 artifact — in development.)

---

## J. Related Documents

1. AI System Inventory and Classification Register
2. AI Governance Procedures Manual
3. Conformity Assessment Template (High-Risk Systems)
4. AI Vendor Risk Due Diligence Addendum
5. EU AI Act Control Mapping
6. Post-Market Monitoring Procedures
7. AI Incident Response Runbook
8. AI System Retirement Checklist
9. Human Oversight Validation Protocol
10. Operator Training Program — High-Risk AI Systems

---

## K. Review and Revision

This policy shall be reviewed **annually** or when any of the following occur: publication of EU AI Act implementing acts or delegated regulations affecting the organisation's AI systems; a significant AI-related incident revealing governance gaps; material changes to the organisation's AI system portfolio; or changes to the ISMS that affect AI governance obligations. All revisions require CEO approval and notification to executive leadership. Changes affecting High-Risk system obligations shall be communicated to AI System Owners **within 14 days** of policy revision.

---

## L. Framework Alignment

| Framework | Alignment |
|-----------|-----------|
| **EU AI Act (Regulation 2024/1689)** | Title II (Prohibited AI Practices), Title III (High-Risk AI Systems), Article 9 (Risk Management System), Article 10 (Data Governance), Article 11 (Technical Documentation), Article 13 (Transparency), Article 14 (Human Oversight), Article 15 (Accuracy, Robustness, Cybersecurity), Article 72 (Post-Market Monitoring), Article 73 (Serious Incident Reporting) |
| **NIST AI RMF 1.0** | GOVERN (organisational AI risk governance structures and culture), MAP (AI risk identification and context establishment), MEASURE (AI risk analysis and tracking), MANAGE (AI risk treatment, response, and recovery) |
| **ISO/IEC 42001:2023** | Clause 4 (Context of the organisation for AI management systems), Clause 6 (Planning — AI risk and opportunity management), Clause 8 (Operation — AI system lifecycle controls), Clause 9 (Performance evaluation of AI management systems), Annex A (AI management controls) |
| **ISO/IEC 27001:2022** | Clause 6.1 (Risk management integration), A.5.19 through A.5.22 (Supplier and third-party AI governance), A.8.25 through A.8.28 (Secure development and system lifecycle) |
| **ISO/IEC 23894:2023** | Guidance on AI risk management — risk identification and treatment for AI-specific threat scenarios |
| **NIST SP 800-53 Rev. 5** | SR-3 (Supply chain controls for AI components), RA-10 (Threat modelling including AI threat vectors), SA-11 (Developer testing and evaluation of AI systems) |

**Note:** This policy aligns with these standards and regulations. Compliance scope and applicability determinations are documented in the EU AI Act Control Mapping and the ISMS Statement of Applicability.

---

## M. Organisational Benefit

| Benefit Area | Description |
|--------------|-------------|
| **Regulatory Compliance** | Establishes the governance structures required to meet EU AI Act obligations, reducing the risk of regulatory penalties (up to €35 million or 7% of global annual turnover for the most serious violations) |
| **Acquisition Risk Management** | Provides a structured framework for assessing and governing AI systems inherited through the Veridian AI acquisition, preventing unmanaged compliance gaps from materialising into enforcement actions |
| **Stakeholder Trust** | Demonstrates to customers, partners, and investors that AI systems are deployed responsibly, with human oversight and accountability mechanisms in place |
| **Risk Reduction** | AI-specific risk controls — bias testing, drift monitoring, human oversight, explainability — reduce the likelihood and impact of model failures that could cause harm to individuals or organisational operations |
| **Competitive Positioning** | Proactive EU AI Act compliance positions Emyzer Nexus favourably with enterprise clients and partners in regulated industries who require evidence of responsible AI governance in their supply chain |
| **Incident Preparedness** | Defined AI incident response procedures and regulatory notification processes reduce response time and demonstrate due diligence if an AI-related incident occurs |
| **Governance Maturity** | Integrating AI governance into the existing ISMS and GRC program demonstrates organisational maturity to auditors, regulators, and prospective clients evaluating Emyzer Nexus as a technology partner |
| **Employee Confidence** | Clear policies on prohibited AI practices and human oversight obligations help employees understand boundaries and responsibilities when working with AI systems |

---

## N. Evidence of Compliance

The organisation shall maintain the following compliance evidence with defined retention periods:

### Evidence Index

| Evidence Type | System of Record | Owner | Retention Period |
|---------------|------------------|-------|------------------|
| AI System Inventory | GRC Platform | GRC Team | Indefinite (current version with full history) |
| AI Risk Classification Decisions | GRC Platform | AI Governance Committee | Life of system + 7 years |
| Conformity Assessment Records | Document Repository | AI System Owner | Life of system + 7 years |
| AI Governance Committee Minutes | Document Repository | CISO | 7 years |
| Technical Documentation (High-Risk) | Document Repository | AI System Owner | Life of system + 7 years |
| Human Oversight Validation Reports | Document Repository | AI System Owner | 5 years |
| Operator Training Records | Learning Management System | Human Resources | 3 years |
| Override Logs | GRC Platform / SIEM | AI System Owner | 3 years |
| Post-Market Monitoring Reports | GRC Platform | AI System Owner | 5 years |
| Bias Audit Reports | Document Repository | AI System Owner | 5 years |
| AI Incident Reports | ServiceNow ITSM | Information Security Team | 10 years |
| Regulatory Notifications | Legal Repository | Legal Counsel | 10 years |
| Vendor AI Due Diligence Records | GRC Platform | Procurement / Information Security | Contract + 5 years |
| AI System Retirement Records | Document Repository | AI System Owner | 7 years |
| AI Risk Register Entries | GRC Platform | Chief Risk Officer | Indefinite |
| Policy Acknowledgements | GRC Platform / HR System | Human Resources | Employment + 3 years |
| AI Awareness Training Records | Learning Management System | Human Resources | 3 years |
| Exception Records | GRC Platform | Information Security | Exception duration + 3 years |
| Annual Governance Audit Reports | GRC Platform | Internal Audit | 7 years |

---

### N.1 AI System Inventory Evidence
- **AI System Inventory Register:** Complete register maintained in the GRC platform documenting all AI systems, including system name, origin (internal/vendor/acquired), intended use, affected populations, EU AI Act risk tier, AI System Owner, deployment date, and review date. Updated **within 30 days** of changes. Retained indefinitely.
- **Classification Decisions:** AI Governance Committee decisions on risk tier classifications, including supporting analysis, Legal Counsel input, and approval record. Retained for life of system plus 7 years.
- **Annual Inventory Audit Reports:** Evidence of annual shadow AI audit, including scope, methodology, systems identified, and classification actions taken. Retained for 5 years.

### N.2 Conformity Assessment Evidence
- **Conformity Assessment Reports:** Completed assessment documentation for each High-Risk AI system covering risk management system, data governance, technical documentation, transparency, human oversight, and accuracy/robustness testing. Conducted before deployment and following material change. Retained for life of system plus 7 years.
- **Technical Documentation Packages:** Full EU AI Act Article 11 technical documentation maintained for each High-Risk system, including system architecture, training methodology, performance metrics, intended use, and known limitations. Retained for life of system plus 7 years.
- **Legal Counsel Review Records:** Documentation of Legal Counsel review of conformity assessments, including review date, findings, and approval. Retained for life of system plus 7 years.

### N.3 Human Oversight Evidence
- **Human Oversight Validation Reports:** Documentation of human oversight mechanism testing, including test scenarios, results, and confirmed capability to intervene or override. Conducted at deployment and **annually** thereafter. Retained for 5 years.
- **Operator Training Records:** LMS records showing operator name, system, training course, completion date, and assessment outcome for all High-Risk AI system operators. Retained for 3 years.
- **Override Logs:** Timestamped records of all human override events, including operator identity, system, output overridden, justification provided, and resolution. Retained for 3 years.
- **Override Review Documentation:** Records of the 5-business-day review of override events, including findings and any corrective actions. Retained for 3 years.

### N.4 Post-Market Monitoring Evidence
- **Monthly Performance Reports (High-Risk):** AI System Owner reports documenting performance metrics against defined baselines, statistical drift analysis, and operator-reported anomalies. Retained for 5 years.
- **Quarterly Bias Audit Reports (High-Risk):** Results of bias testing across relevant demographic and contextual subgroups, including methodology, findings, and remediation actions. Retained for 5 years.
- **Drift Assessment Records:** Documentation of data distribution analysis, including methodology, findings, and model update or retraining decisions. Retained for 5 years.
- **AI Governance Committee Monitoring Reviews:** Quarterly committee review minutes covering monitoring outcomes, findings, and decisions. Retained for 7 years.

### N.5 AI Incident Evidence
- **AI Incident Reports:** ServiceNow incident records for AI-specific incidents, including incident type, system affected, detection timestamp, classification, containment actions, and resolution. Retained for 10 years.
- **Post-Incident Reviews:** Structured analysis reports for High and Critical AI incidents, including AI-specific root cause analysis and corrective actions. Completed **within 5 business days** of resolution. Retained for 10 years.
- **Regulatory Notifications:** Records of serious incident notifications to national market surveillance authorities under EU AI Act Article 73, including notification content, submission timestamp, and regulatory response. Retained for 10 years.

### N.6 Third-Party AI Evidence
- **AI Vendor Due Diligence Records:** Completed AI-specific due diligence assessments covering EU AI Act classification, transparency documentation, bias audit availability, and data processing practices. Retained for contract duration plus 5 years.
- **AI Vendor Contracts:** Executed agreements incorporating AI governance obligations, incident notification requirements, audit rights, and liability provisions for model errors. Retained for contract duration plus 7 years.
- **Vendor AI Compliance Attestations:** Annual vendor attestations confirming continued EU AI Act compliance and governance posture. Retained for 5 years.

### N.7 Governance and Training Evidence
- **AI Governance Committee Minutes:** Quarterly meeting records covering inventory review, classification decisions, conformity status, monitoring outcomes, and regulatory developments. Retained for 7 years.
- **AI Awareness Training Records:** LMS records confirming completion of AI awareness training by all employees. Retained for 3 years.
- **Policy Acknowledgements:** Digital records confirming employees have acknowledged and agree to comply with this policy. Retained for employment duration plus 3 years.
- **Annual Governance Audit Reports:** Internal audit findings on AI governance program effectiveness, including findings, severity ratings, remediation plans, and closure evidence. Retained for 7 years.

### N.8 AI System Retirement Evidence
- **Retirement Approval Records:** AI Governance Committee approval of system retirement, including business justification, stakeholder notification plan, and data disposition approach. Retained for 7 years.
- **Data Disposition Records:** Documentation of training data, model artefact, and operational data disposition in accordance with the Data Classification Policy, including deletion certificates or archival confirmation. Retained for 7 years.
- **Retired System Archive:** Technical documentation, conformity assessment records, and monitoring history archived for retired systems. Retained for 7 years from retirement date.

---

## Approval History

| Date | Approver | Status | Comments |
|------|----------|--------|----------|
| 2025-06-01 | Chief Executive Officer | Approved | "This policy reflects the governance obligations we assumed through the Veridian AI acquisition and positions us correctly for EU AI Act compliance. The committee structure and conformity assessment requirements are proportionate and operationally sound. Approved." |

---

## Document Control

- **Document ID:** KB-PORTFOLIO-0011
- **Version:** 1.0
- **Classification:** Internal
- **Last Updated:** 2025-06-01
- **Next Review Date:** 2026-06-01

---

*This policy document was developed as part of the Emyzer Nexus Phase 2 GRC program and formatted for portfolio presentation.*


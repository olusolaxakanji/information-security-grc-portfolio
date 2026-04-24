# Privacy and Data Protection Policy

**Emyzer Nexus – Governance, Risk, and Compliance**

---

## Policy Metadata

| Attribute | Value |
|-----------|-------|
| **Policy Name** | Privacy and Data Protection Policy |
| **Type** | Policy |
| **Version** | 1.0 |
| **Parent Policy** | Information Security Policy (KB-PORTFOLIO-0001) |
| **Owner** | Data Protection Officer |
| **Owning Group** | App Engine Admins |
| **State** | Published |
| **Valid From** | 2025-10-01 |
| **Valid To** | 2026-10-01 |
| **Approvers** | Chief Executive Officer |
| **Reviewers** | Chief Information Security Officer; Chief Risk Officer; GRC Analyst; Legal Counsel; Human Resources Director |
| **Knowledge Base** | Governance, Risk, and Compliance |
| **Published Policy** | KB-PORTFOLIO-0013 |

---

## Description

This policy establishes the governance framework for the protection of personal data across Emyzer Nexus and its subsidiaries, operationalising the organisation's obligations under the EU General Data Protection Regulation (GDPR), the UK General Data Protection Regulation (UK GDPR), and aligned international data protection standards. It governs the lawful collection, processing, storage, transfer, and disposal of personal data in all organisational activities — including AI systems, acquired data assets, and third-party processing relationships.

**Impact:** Non-compliance with GDPR and UK GDPR carries financial penalties of up to €20 million or 4% of global annual turnover (whichever is higher) under GDPR, and equivalent penalties under UK GDPR. Beyond financial exposure, privacy failures erode customer and partner trust in ways that are operationally recoverable only slowly. For Emyzer Nexus, the Veridian AI acquisition introduced personal data processing activities — including the Predictive Customer Churn Model and AI-Assisted Contract Review Tool — that require formal Data Protection Impact Assessment (DPIA) under GDPR Article 35 given their High-Risk AI classification and the nature of their data inputs. This policy provides the framework for assessing and managing those obligations.

**Relevant Standards:** EU General Data Protection Regulation (GDPR, Regulation 2016/679); UK General Data Protection Regulation (UK GDPR); ISO/IEC 27701:2019 (Privacy Information Management System); ISO/IEC 27001:2022; EU AI Act (Regulation 2024/1689) — intersection with DPIA obligations; NIST Privacy Framework 1.0

---

## Policy Snapshot

| Dimension | Summary |
|-----------|---------|
| **Applies to** | All Emyzer Nexus employees, contractors, board members, and third parties processing personal data on behalf of the organisation — including activities arising from the Veridian AI acquisition and Emyzer Technology development operations |
| **Covers** | All personal data processing activities in Emyzer Nexus's capacity as a data controller and as a data processor on behalf of clients; all jurisdictions in which personal data from EU and UK data subjects is processed |
| **Legal Bases** | Consent, contract, legal obligation, vital interests, public task, legitimate interests — documented per processing activity in the Record of Processing Activities |
| **Key Governance** | DPO owns the programme; Legal Counsel advises on regulatory obligations; CISO ensures security controls; GRC Team maintains ROPA and DPIA register; AI Governance Committee reviews AI-specific DPIA obligations |
| **DPIA Obligation** | Mandatory for High-Risk AI systems processing personal data, large-scale profiling, systematic monitoring, and processing of special category data — as defined in GDPR Article 35 and EDPB Guidelines |
| **Breach Response** | Supervisory authority notification within 72 hours of becoming aware; affected individual notification without undue delay where required; coordinated with Incident Management Policy |
| **Exceptions Process** | ServiceNow workflow with DPO approval; maximum 90-day duration; quarterly review |
| **Evidence Maintained** | ROPA, DPIA register, consent records, data subject request logs, breach notification records, transfer mechanism documentation, vendor DPA register (all with defined retention periods) |

---

## A. Purpose

To establish the governance framework, minimum standards, and accountability structures for the protection of personal data across Emyzer Nexus, ensuring that all personal data processing activities are lawful, fair, transparent, and proportionate — and that the organisation can demonstrate compliance to regulators, clients, and data subjects when required.

This policy operationalises Emyzer Nexus's obligations as both a data controller and a data processor. As a data controller, the organisation determines the purposes and means of processing personal data in its internal operations, customer relationships, and employment activities. As a data processor, the organisation processes personal data on behalf of clients who remain the data controller — an arrangement that creates distinct contractual and regulatory obligations, particularly in relation to the security of processing and notification of personal data breaches.

The policy gives particular attention to the intersection of privacy obligations with the organisation's AI governance programme. The EU AI Act and GDPR create overlapping and occasionally complementary obligations for High-Risk AI systems that process personal data. DPIAs required under GDPR Article 35 for such systems must address not only standard data protection risks but also the AI-specific risks of automated decision-making, algorithmic bias, and data subject rights limitations arising from AI system design. This policy establishes the governance structures to navigate that intersection systematically rather than addressing privacy and AI governance as separate compliance workstreams.

---

## B. Scope

### B.1 Processing Activities in Scope

This policy applies to all processing of personal data by Emyzer Nexus, including:

- Personal data of employees, contractors, and job applicants processed in HR and payroll systems
- Personal data of clients, prospects, and contacts processed in CRM, marketing, and sales systems
- Personal data of end users of Emyzer Technology products and services
- Personal data processed through AI systems, including the Predictive Customer Churn Model and AI-Assisted Contract Review Tool inherited through the Veridian AI acquisition
- Personal data processed on behalf of clients in Emyzer Nexus's capacity as a data processor
- Personal data of third-party contacts processed in vendor management and procurement systems
- Any personal data transferred to or received from third parties, including processors, sub-processors, and international partners

### B.2 Jurisdictional Scope

Emyzer Nexus processes personal data of data subjects in the European Union and the United Kingdom. Both GDPR and UK GDPR apply concurrently to the organisation's processing activities, with specific obligations under each jurisdiction governing:

| Obligation | GDPR (EU) | UK GDPR |
|-----------|-----------|---------|
| Supervisory Authority | Relevant EU Member State authority (lead SA determined by main establishment) | Information Commissioner's Office (ICO) |
| Data Transfer Mechanism (to third countries) | Adequacy decision, SCCs, BCRs, derogations | UK adequacy regulations, IDTA, UK Addendum to EU SCCs, derogations |
| Representatives | EU Representative required if no EU establishment | UK Representative required if no UK establishment |
| Penalty Maximum | €20M or 4% global annual turnover | £17.5M or 4% global annual turnover |

Where GDPR and UK GDPR create different obligations for the same processing activity, the more stringent requirement shall apply unless Legal Counsel advises otherwise in writing with documented regulatory justification.

### B.3 Personal Data Inherited Through the Veridian AI Acquisition

The Veridian AI acquisition transferred to Emyzer Nexus control over personal data processing activities for which the organisation must now establish lawful basis, verify processing records, and conduct DPIAs where required. At time of policy publication, the following acquired processing activities are undergoing formal privacy assessment:

| Processing Activity | System | DPIA Status | Risk Basis for DPIA |
|--------------------|--------|-------------|---------------------|
| Customer churn prediction using behavioural data | Predictive Customer Churn Model | In progress | Large-scale profiling; EU AI Act High-Risk classification; potential for decisions affecting service access |
| Contract data analysis using NLP | AI-Assisted Contract Review Tool | In progress | Special category data risk (contracts may contain health, financial, or other sensitive data); EU AI Act High-Risk classification; automated analysis at scale |

Both systems are operating under interim data protection arrangements pending DPIA completion and DPO sign-off. The DPO shall report DPIA progress to the AI Governance Committee **monthly** until both assessments are complete.

### B.4 Emyzer Nexus as Data Processor

Where Emyzer Nexus processes personal data on behalf of clients, it acts as a data processor and shall:
- Process personal data only on documented instructions from the controller
- Ensure all processing meets the security requirements of GDPR Article 32
- Not engage sub-processors without the controller's prior specific or general written authorisation
- Notify the controller of personal data breaches without undue delay and in accordance with the contractual data processing agreement
- Assist the controller in fulfilling data subject rights requests and DPIA obligations where the processing involves Emyzer Nexus systems or operations
- Delete or return personal data at the end of the service relationship as instructed by the controller

### B.5 Exclusions

Anonymised data — data that has been irreversibly processed so that individuals cannot be identified directly or indirectly — is excluded from this policy. The DPO shall approve all anonymisation determinations in writing before data is treated as excluded. Pseudonymised data remains personal data and is in scope.

---

## C. Definitions

| Term | Definition |
|------|------------|
| **Personal Data** | Any information relating to an identified or identifiable natural person (a "data subject"). As defined in GDPR Article 4(1). Includes names, identification numbers, location data, online identifiers, and factors specific to physical, physiological, genetic, mental, economic, cultural, or social identity. |
| **Special Category Data** | Personal data revealing racial or ethnic origin, political opinions, religious or philosophical beliefs, trade union membership, genetic data, biometric data for identification, health data, or data concerning sex life or sexual orientation. Subject to enhanced protection under GDPR Article 9. |
| **Processing** | Any operation performed on personal data, whether automated or not — including collection, recording, storage, adaptation, retrieval, consultation, use, disclosure, combination, restriction, erasure, or destruction. As defined in GDPR Article 4(2). |
| **Data Controller** | The natural or legal person that determines the purposes and means of the processing of personal data. Emyzer Nexus acts as controller for its internal processing activities. |
| **Data Processor** | A natural or legal person that processes personal data on behalf of the controller. Emyzer Nexus acts as processor when processing client data under a data processing agreement. |
| **Data Protection Officer (DPO)** | The individual designated under GDPR Article 37 to provide expert advice on data protection obligations, monitor compliance, act as a contact point for supervisory authorities, and cooperate with those authorities. |
| **Data Processing Agreement (DPA)** | A contract between a controller and processor (or between processors and sub-processors) establishing the terms under which personal data is processed, as required by GDPR Article 28. |
| **Record of Processing Activities (ROPA)** | The internal register of all personal data processing activities conducted by or on behalf of Emyzer Nexus, as required by GDPR Article 30. The primary instrument for demonstrating processing accountability. |
| **Data Protection Impact Assessment (DPIA)** | A structured risk assessment of processing activities likely to result in a high risk to the rights and freedoms of data subjects, as required by GDPR Article 35. Mandatory for specified processing types including large-scale profiling and processing using new technologies. |
| **Lawful Basis** | One of the six legal grounds under GDPR Article 6 that must be identified and documented before personal data is processed: consent, contract, legal obligation, vital interests, public task, or legitimate interests. |
| **Data Subject** | The identified or identifiable natural person to whom personal data relates. |
| **Data Subject Rights** | The rights of data subjects under GDPR Chapter III: right of access (Article 15), right to rectification (Article 16), right to erasure (Article 17), right to restriction of processing (Article 18), right to data portability (Article 20), right to object (Article 21), and rights related to automated decision-making (Article 22). |
| **Personal Data Breach** | A breach of security leading to accidental or unlawful destruction, loss, alteration, unauthorised disclosure of, or access to, personal data. As defined in GDPR Article 4(12). |
| **Privacy by Design** | The principle, codified in GDPR Article 25, that data protection is considered and integrated into the design of systems and processes from the outset — not added as an afterthought. |
| **Standard Contractual Clauses (SCCs)** | Contractual terms adopted by the European Commission providing appropriate safeguards for personal data transfers to third countries without an adequacy decision, as permitted under GDPR Article 46. |
| **International Data Transfer Addendum (IDTA)** | The UK equivalent of SCCs, issued by the ICO, providing a transfer mechanism for personal data transfers from the UK to third countries under UK GDPR. |
| **Adequacy Decision** | A European Commission decision (for GDPR) or UK Secretary of State regulation (for UK GDPR) recognising that a third country provides a level of data protection essentially equivalent to that of the EU or UK respectively. |
| **Consent** | A freely given, specific, informed, and unambiguous indication of the data subject's agreement to the processing of their personal data. As defined in GDPR Article 4(11). For special category data, explicit consent is required under Article 9. |
| **Legitimate Interests** | A lawful basis under GDPR Article 6(1)(f) permitting processing necessary for the purposes of legitimate interests pursued by the controller or a third party, where those interests are not overridden by the interests or fundamental rights of the data subject. Requires a documented Legitimate Interests Assessment (LIA). |
| **Privacy Information Management System (PIMS)** | The management system framework established under ISO/IEC 27701:2019, extending ISO 27001 to include privacy-specific controls. Applied by Emyzer Nexus as the operational structure for managing privacy obligations within the ISMS. |
| **Automated Individual Decision-Making** | Processing that involves making a decision about an individual solely by automated means without meaningful human involvement, subject to specific restrictions and rights under GDPR Article 22. |
| **Sub-processor** | A third party engaged by a data processor to carry out specific processing activities on behalf of the controller. Subject to the same data protection obligations as the processor under GDPR Article 28(4). |

---

## D. Policy Statement

Emyzer Nexus is committed to processing personal data in a manner that respects the privacy rights of data subjects, fulfils the organisation's legal obligations under GDPR and UK GDPR, and maintains the trust of the clients, employees, and individuals whose data the organisation handles. The organisation shall:

1. Process personal data only where a **documented lawful basis** under GDPR Article 6 exists for each processing purpose, identified and recorded in the ROPA before processing commences. Special category data shall only be processed where an additional condition under GDPR Article 9 is also met and documented.

2. Maintain a complete and current **Record of Processing Activities (ROPA)** capturing all personal data processing activities across the organisation, updated within **14 days** of any new, modified, or discontinued processing activity.

3. Apply the **data protection principles** of GDPR Article 5 to all processing activities: lawfulness, fairness and transparency; purpose limitation; data minimisation; accuracy; storage limitation; integrity and confidentiality; and accountability. The accountability principle is operationalised through this policy, the ROPA, DPIAs, and the evidence regime defined in Section R.

4. Conduct a **Data Protection Impact Assessment (DPIA)** before commencing any processing activity likely to result in a high risk to the rights and freedoms of data subjects, including all High-Risk AI systems processing personal data, large-scale profiling activities, systematic monitoring, and processing of special category data at scale.

5. Embed **privacy by design and by default** in all system development, process design, and product development activities — ensuring that only personal data necessary for the specified purpose is collected, that privacy-protective options are the default, and that data protection controls are built in rather than retrofitted.

6. Fulfil **data subject rights requests** within the statutory timeframes — one calendar month from receipt (extendable by a further two months for complex or numerous requests), with no fee except in exceptional circumstances — maintaining complete records of all requests and responses.

7. Notify the relevant **supervisory authority** of personal data breaches meeting the threshold for notification within **72 hours** of becoming aware of the breach, and notify affected data subjects without undue delay where the breach is likely to result in a high risk to their rights and freedoms.

8. Ensure all **third-party processors** are engaged under a compliant Data Processing Agreement meeting the requirements of GDPR Article 28, and that sub-processor arrangements are governed with equivalent contractual protections.

9. Apply **appropriate transfer mechanisms** to all transfers of personal data to third countries without an EU adequacy decision (for GDPR) or UK adequacy regulation (for UK GDPR), including Standard Contractual Clauses, the UK International Data Transfer Addendum, or other mechanisms approved by the relevant supervisory authority.

10. Maintain a **designated Data Protection Officer** with the independence, resources, and access to fulfil the obligations of GDPR Article 39, including monitoring compliance, providing expert advice, and acting as the primary contact for supervisory authorities.

11. Address the **intersection of GDPR and EU AI Act obligations** for High-Risk AI systems processing personal data — treating the DPIA obligation under GDPR Article 35 and the EU AI Act conformity assessment under AI Governance Policy Section F.3 as complementary processes with shared evidence, coordinated under joint DPO and AI Governance Committee oversight.

12. Review and update this policy **annually** or upon material changes to GDPR or UK GDPR implementing guidance, significant new processing activities, a personal data breach revealing governance gaps, or relevant European Data Protection Board (EDPB) or ICO guidance affecting the organisation's processing activities.

---

## E. Data Protection Principles in Practice

The six data protection principles of GDPR Article 5 are not aspirational statements — they are legal obligations with specific operational implications for Emyzer Nexus.

### E.1 Lawfulness, Fairness, and Transparency
Every processing activity must have a documented lawful basis. Data subjects must receive clear, accessible, and complete privacy notices explaining what data is collected, why, how long it is kept, and their rights. Privacy notices shall be reviewed **annually** by the DPO and updated within **14 days** of any change to the processing they describe.

### E.2 Purpose Limitation
Personal data collected for a specified purpose shall not be subsequently processed in a manner incompatible with that purpose. Compatibility assessments — evaluating whether a new use of existing data is compatible with its original purpose — shall be conducted and documented by the DPO before any secondary use commences. AI model training on operational data is a secondary use requiring compatibility assessment.

### E.3 Data Minimisation
Only personal data that is adequate, relevant, and limited to what is necessary for the processing purpose shall be collected. Data minimisation obligations apply at the point of system design (privacy by design), at the point of collection, and on an ongoing basis through periodic reviews of what data is actually used versus what is held. AI training datasets are subject to specific minimisation review — the DPO and AI System Owner shall jointly assess whether training data volume and granularity is the minimum necessary for the model's intended function.

### E.4 Accuracy
Personal data shall be accurate and kept up to date. Processing systems shall include mechanisms for data subjects to correct inaccurate data, and for the organisation to verify accuracy at appropriate intervals. Inaccurate personal data used in AI model training may propagate bias — the DPO shall flag training data accuracy concerns to the AI Governance Committee as a joint data protection and model risk issue.

### E.5 Storage Limitation
Personal data shall not be retained for longer than necessary for the purpose for which it was collected. Retention periods shall be documented in the ROPA for each processing activity and enforced through automated deletion schedules or manual review processes on defined review dates. The DPO shall conduct an annual retention compliance review, with findings reported to the CISO and CRO.

### E.6 Integrity and Confidentiality
Personal data shall be processed with appropriate security measures protecting against unauthorised or unlawful processing, accidental loss, destruction, or damage. Security controls for personal data processing are governed jointly by this policy and the Information Security Policy. The DPO shall advise the CISO on data protection-specific security requirements for systems processing personal data, particularly where AI processing creates novel security risks (model inversion attacks, training data extraction).

### E.7 Accountability
Emyzer Nexus shall be able to demonstrate compliance with all six principles above. Demonstration is operationalised through: the ROPA (processing inventory), DPIAs (risk assessment), Data Processing Agreements (third-party accountability), privacy notices (transparency), data subject request logs (rights fulfilment), breach notification records (incident accountability), and this policy (governance structure). All accountability evidence is maintained with defined retention periods in Section R.

---

## F. Roles and Responsibilities

### F.1 Chief Executive Officer (CEO)
Provides board-level accountability for data protection compliance. Shall receive **quarterly** privacy compliance briefings from the DPO. Shall approve the Privacy and Data Protection Policy and material amendments. Shall ensure the DPO has sufficient resources and organisational independence to fulfil their obligations.

### F.2 Data Protection Officer (DPO)
The DPO is an independent function reporting directly to the CEO, with access to all processing activities, systems, and personnel necessary to fulfil their statutory obligations under GDPR Article 39. The DPO shall not receive instructions on how to carry out their tasks. The DPO shall:
- Monitor organisational compliance with GDPR, UK GDPR, and this policy
- Maintain and review the ROPA **quarterly** and following any new or materially changed processing activity
- Review and approve all DPIAs, with authority to recommend suspension of processing where risks cannot be adequately mitigated
- Act as the primary contact point for supervisory authorities (relevant EU lead supervisory authority and the ICO)
- Advise on data protection obligations in response to requests from any business unit **within 5 business days**
- Coordinate data subject rights request responses, maintaining oversight of the end-to-end process
- Lead personal data breach assessment and coordinate supervisory authority notification decisions
- Advise the AI Governance Committee on the intersection of GDPR and EU AI Act obligations for AI systems processing personal data
- Review and approve privacy notices and consent mechanisms before publication
- Report privacy compliance posture to the CEO **monthly** and to the Security Steering Committee **quarterly**

### F.3 Legal Counsel
Advises on the legal interpretation of GDPR and UK GDPR obligations, regulatory guidance, and enforcement trends. Reviews Data Processing Agreements, cross-border transfer mechanisms, and regulatory correspondence. Advises on the applicability of exemptions and derogations. Coordinates with external legal advisers on regulatory investigations or significant compliance questions. Reviews DPIAs for High-Risk AI systems in conjunction with the DPO.

### F.4 Chief Information Security Officer (CISO)
Ensures information security controls are adequate for the protection of personal data in accordance with GDPR Article 32. Coordinates with the DPO on security measures for personal data processing, personal data breach identification and response, and the security implications of new processing activities. Advises on technical and organisational security measures for DPIAs.

### F.5 AI Governance Committee
Reviews AI-related DPIA requirements in conjunction with the DPO for all High-Risk AI systems processing personal data. Ensures conformity assessments under the AI Governance Policy and DPIAs under this policy are conducted as coordinated, complementary processes sharing documentation where appropriate. Approves AI system deployment only after DPO confirmation that applicable DPIA obligations have been met.

### F.6 GRC Team
Maintains the ROPA in the GRC platform, manages the DPIA register, tracks data subject request completion against statutory deadlines, produces privacy compliance reporting, and manages the exceptions log. Conducts **quarterly** ROPA completeness and accuracy reviews. Coordinates the annual retention compliance review.

### F.7 Human Resources Director
Manages personal data of employees and job applicants in accordance with this policy. Ensures HR processing activities are reflected in the ROPA. Oversees employee privacy notice currency and distribution. Manages subject access requests from current and former employees in coordination with the DPO.

### F.8 All Employees and Contractors
Shall process personal data only in accordance with this policy, the Data Classification Policy, and any role-specific processing instructions. Shall report suspected personal data breaches to the Information Security Team and DPO **within 4 hours** of becoming aware. Shall refer data subject requests to the DPO **within 24 hours** of receipt, without attempting to respond independently. Shall not share personal data with third parties — including service providers, partners, or other Emyzer Nexus entities — without confirming that an appropriate legal basis and transfer mechanism is in place.

### F.9 System and Application Owners
Shall engage the DPO at the earliest practicable stage of any new system design, application development, or processing activity involving personal data. Shall implement privacy by design and by default in system architecture and configuration. Shall support DPIA processes by providing system documentation, data flow information, and technical control evidence when requested by the DPO. Shall notify the DPO within **5 business days** of any proposed material change to a processing activity.

---

## G. Lawful Basis and Record of Processing Activities

### G.1 Lawful Basis Determination

Before commencing any personal data processing activity, the responsible business unit shall work with the DPO to identify and document the applicable lawful basis. The six lawful bases under GDPR Article 6 and their primary use contexts at Emyzer Nexus are:

| Lawful Basis | GDPR Article | Primary Use Context at Emyzer Nexus |
|-------------|-------------|-------------------------------------|
| **Consent** | 6(1)(a) | Marketing communications; non-essential cookies; processing where no other basis applies and data subject choice is appropriate |
| **Contract** | 6(1)(b) | Processing necessary for the performance of a contract with the data subject (e.g., employment contracts, customer service delivery) |
| **Legal Obligation** | 6(1)(c) | Processing required by EU or Member State law (e.g., tax records, employment law obligations, regulatory reporting) |
| **Vital Interests** | 6(1)(d) | Processing necessary to protect the life of the data subject or another person — rare and exceptional use only |
| **Public Task** | 6(1)(e) | Not applicable to Emyzer Nexus's activities as a private sector organisation |
| **Legitimate Interests** | 6(1)(f) | Processing for the organisation's legitimate business interests where these are not overridden by data subject rights — requires documented Legitimate Interests Assessment (LIA) |

**Legitimate Interests Assessment:** Where legitimate interests is proposed as the lawful basis, the DPO shall conduct and document a three-stage LIA: identifying the legitimate interest, assessing the necessity of the processing, and balancing the interest against the data subject's rights and reasonable expectations. LIAs shall be reviewed if circumstances of the processing change materially.

**AI Systems and Lawful Basis:** AI model training on personal data requires a lawful basis. Where operational personal data is used to train or retrain an AI model, the DPO and AI System Owner shall confirm that the original collection basis is compatible with the training use (purpose limitation assessment) or identify an alternative basis. AI-generated outputs that constitute decisions about individuals require separate lawful basis assessment, particularly where GDPR Article 22 (automated decision-making) may apply.

### G.2 Special Category Data

Processing of special category data requires both a lawful basis under Article 6 and a condition under Article 9. The DPO must approve any special category data processing in writing before it commences. Conditions available to Emyzer Nexus include:

- Explicit consent (Article 9(2)(a))
- Employment, social security, and social protection obligations (Article 9(2)(b))
- Vital interests where the data subject cannot consent (Article 9(2)(c))
- Substantial public interest with appropriate safeguards (Article 9(2)(g))
- For health data in the context of healthcare services (Article 9(2)(h))

The AI-Assisted Contract Review Tool may process contracts containing health, financial, or other sensitive information that constitutes special category data in context. The DPO shall determine the applicable Article 9 condition as part of the DPIA for that system before full operational deployment is authorised.

### G.3 Record of Processing Activities (ROPA)

The ROPA is the foundational accountability instrument under GDPR Article 30. Emyzer Nexus shall maintain a ROPA in its capacity as both controller and processor. The ROPA shall capture, for each processing activity:

**As Controller:**
- Name and contact details of the controller and, where applicable, joint controllers and the DPO
- Purposes of processing
- Categories of data subjects
- Categories of personal data (including whether special category data is involved)
- Categories of recipients (including third countries)
- Third-country transfer details and applicable transfer mechanism
- Retention periods or criteria for determining retention
- General description of technical and organisational security measures (GDPR Article 32)
- Lawful basis for processing
- DPIA reference (where conducted)

**As Processor:**
- Name and contact details of the processor(s) and, where applicable, each controller and the DPO
- Categories of processing carried out on behalf of each controller
- Third-country transfer details and applicable transfer mechanism
- General description of technical and organisational security measures

The ROPA shall be maintained in the GRC platform, reviewed **quarterly** by the GRC Team for completeness, and updated within **14 days** of any new, modified, or discontinued processing activity. The ROPA shall be made available to supervisory authorities on request.

---

## H. Data Protection Impact Assessment (DPIA)

### H.1 When a DPIA is Mandatory

A DPIA is mandatory under GDPR Article 35 before commencing processing that is likely to result in a high risk to data subjects' rights and freedoms. Emyzer Nexus shall conduct a DPIA for any processing activity that meets one or more of the following criteria, drawn from EDPB Guidelines 09/2022:

| Criterion | Application at Emyzer Nexus |
|-----------|----------------------------|
| Automated processing for evaluation, scoring, or profiling with legal or similarly significant effects | Customer churn prediction model; any AI system producing outputs that inform decisions affecting service access, pricing, or contractual terms |
| Automated decision-making with legal or similarly significant effects | Any AI system output used without meaningful human review in decisions affecting individuals |
| Large-scale processing of special category data | Contract review tool processing contracts containing health, financial, or legally sensitive personal data |
| Systematic monitoring of publicly accessible areas or online behaviour at scale | Any monitoring analytics or behavioural tracking at scale |
| Processing of data concerning vulnerable persons | Any processing where the data subject population includes children, patients, or financially vulnerable individuals |
| Innovative or novel technology | First deployment of any AI or ML system; first use of a new AI API |
| Processing preventing data subjects from exercising rights or using services | Any automated system producing outputs that affect access to Emyzer Nexus or client services |

Processing activities meeting two or more criteria from the EDPB list of nine factors shall be treated as requiring a DPIA regardless of whether they meet the mandatory threshold above.

### H.2 DPIA Process

DPIAs shall be conducted using the following structured process:

**Step 1 — Screening (DPO)**
The DPO shall assess whether a DPIA is required within **10 business days** of being notified of a new or materially changed processing activity. The screening decision and rationale shall be documented in the DPIA register.

**Step 2 — Scoping (DPO and System/Process Owner)**
Where a DPIA is required, the DPO and the responsible System or Process Owner shall define the processing activity scope, identify all relevant stakeholders, and agree the assessment timeline. DPIA completion shall be required **before** the processing activity commences or the system is deployed.

**Step 3 — Description of Processing (System/Process Owner)**
The System or Process Owner shall document:
- The nature, scope, context, and purpose of the processing
- The categories of personal data and data subjects involved
- The data lifecycle: collection, storage, access, transfer, and deletion
- The systems and sub-processors involved
- The lawful basis and, where applicable, special category condition

**Step 4 — Necessity and Proportionality Assessment (DPO)**
The DPO shall assess whether the processing is necessary and proportionate to the stated purpose, including whether the purpose could be achieved with less personal data, for a shorter retention period, or with less invasive technology.

**Step 5 — Risk Assessment (DPO and CISO)**
The DPO and CISO shall jointly identify and assess risks to data subjects' rights and freedoms arising from the processing, including:
- Risks of unauthorised access, disclosure, or loss
- Risks of inaccuracy or data quality failure
- Risks of discriminatory or harmful outcomes from automated processing
- For AI systems: risks of algorithmic bias, model drift affecting data subject outcomes, limited explainability, and restrictions on data subject rights arising from AI design
- Risks to data subjects from cross-border transfers

**Step 6 — Measures to Address Risks (DPO, CISO, and System Owner)**
For each identified risk, the assessment shall document the technical and organisational measures implemented or proposed to reduce the risk to an acceptable level, including: encryption, access controls, pseudonymisation, data minimisation, human oversight mechanisms, explainability tools, data subject rights enablement, and contractual safeguards.

**Step 7 — DPO Review and Approval**
The DPO shall review the completed DPIA and issue one of the following outcomes:
- **Approved:** Processing may proceed. DPO records approval in the DPIA register.
- **Approved with Conditions:** Processing may proceed subject to specified conditions being implemented and verified before commencement. Conditions documented and tracked by GRC Team.
- **Deferred:** Additional information or mitigation required before the DPO can assess. Responsible party has **20 business days** to respond.
- **Rejected:** Residual risks remain high and cannot be adequately mitigated. Processing shall not commence. DPO escalates to the CEO and, where required, consults the supervisory authority under GDPR Article 36 (prior consultation).

**Step 8 — Supervisory Authority Prior Consultation (Where Required)**
Where a DPIA concludes that residual risks remain high after mitigation, Emyzer Nexus shall consult the relevant supervisory authority before commencing processing, as required by GDPR Article 36. Legal Counsel shall manage the consultation process. Processing shall not commence until the supervisory authority responds or the consultation period expires.

### H.3 DPIA and AI Governance Policy Coordination

For High-Risk AI systems processing personal data, the DPIA required under this policy and the conformity assessment required under the AI Governance Policy (Section F.3) are complementary processes addressing overlapping subject matter. To eliminate duplication and ensure consistency:

- The DPIA and conformity assessment for each High-Risk AI system shall be conducted as a **coordinated process** with shared documentation for: data governance assessment, accuracy and bias testing evidence, human oversight mechanisms, and explainability measures.
- The DPO and CISO shall jointly designate a lead assessor for each system, with the other providing review and sign-off.
- DPO approval of the DPIA and AI Governance Committee approval of the conformity assessment are **both required** before deployment authorisation is issued. Neither approval substitutes for the other.
- The DPIA register and AI System Inventory shall cross-reference each other for systems subject to both processes.

### H.4 DPIA Review and Maintenance

Approved DPIAs shall be reviewed and updated when:
- The nature, purpose, or scope of the processing changes materially
- A personal data breach occurs involving the processing activity
- Post-market monitoring of an AI system reveals unexpected data processing outcomes or bias
- Relevant EDPB or ICO guidance is published affecting the assessment methodology or findings
- The DPO determines that the original risk assessment is no longer current

DPIAs shall be reviewed at minimum **every 3 years** for ongoing processing activities, regardless of whether a material change has occurred.

---

## I. Data Subject Rights

### I.1 Rights Overview and Response Deadlines

| Right | GDPR Article | Standard Deadline | Extension Permitted |
|-------|-------------|-------------------|---------------------|
| Right of access (Subject Access Request) | 15 | 1 calendar month | +2 months for complex/numerous requests |
| Right to rectification | 16 | 1 calendar month | +2 months |
| Right to erasure ("right to be forgotten") | 17 | 1 calendar month | +2 months |
| Right to restriction of processing | 18 | Without undue delay | Not applicable |
| Notification obligation (rectification/erasure/restriction) | 19 | Without undue delay | Not applicable |
| Right to data portability | 20 | 1 calendar month | +2 months |
| Right to object | 21 | Without undue delay; immediately for direct marketing | Not applicable |
| Rights related to automated decision-making | 22 | 1 calendar month | +2 months |

All deadlines run from the day the request is received, regardless of the channel through which it is received.

### I.2 Data Subject Request Handling Process

**Receipt and Logging:** Any employee who receives a data subject request shall forward it to the DPO **within 24 hours** without attempting an independent response. The GRC Team shall log the request in the data subject request tracker **within 24 hours** of DPO receipt, recording: request type, date received, data subject identity, and statutory deadline.

**Identity Verification:** The DPO shall verify the identity of the requestor before providing any personal data. Identity verification shall be proportionate to the sensitivity of the data involved and shall not create unnecessary barriers to rights exercise. Where identity cannot be verified, the DPO shall request further information and document the exchange. The response clock continues to run from the date of original receipt regardless of verification steps.

**Assessment and Response:** The DPO shall assess whether the request is valid, whether exemptions apply, and what information or action is required. The response shall be provided in plain language, free of charge (except in exceptional circumstances of manifestly unfounded or excessive requests, with DPO approval and CEO notification), and in a format accessible to the data subject.

**Extensions:** Where the one-month deadline is extended by up to two months due to complexity, the data subject shall be notified within the original one-month period with reasons for the extension.

**Exemptions:** The DPO and Legal Counsel shall jointly assess claims of exemption (e.g., legal professional privilege, prevention of crime, national security). Exemption decisions shall be documented and retained.

**AI-Specific Considerations for Data Subject Rights:**
Rights relating to automated decision-making (Article 22) apply where AI system outputs are used to make decisions about individuals based solely on automated processing with legal or similarly significant effects. For such systems, data subjects have the right to:
- Not be subject to solely automated decisions (unless one of the Article 22(2) conditions applies)
- Obtain human intervention and the ability to express their point of view
- Obtain an explanation of the decision
- Contest the decision

The DPO shall work with AI System Owners to document which systems are subject to Article 22 obligations and how those rights are operationalised, as part of the DPIA process.

### I.3 Request Metrics and Reporting

The GRC Team shall report to the DPO **monthly** on:
- Volume of requests by type
- Completion rate within statutory deadline
- Extensions applied and reasons
- Requests refused and grounds
- Requests involving AI system data

The DPO shall include data subject request metrics in the quarterly privacy compliance report to the Security Steering Committee.

---

## J. Personal Data Breach Management

### J.1 Breach Identification and Internal Reporting

A personal data breach is a security incident with privacy implications. Breach management is coordinated between the Incident Management Policy (security response) and this policy (regulatory and notification obligations).

Any employee who suspects a personal data breach shall report it to the Information Security Team and DPO **within 4 hours** of becoming aware, using the established incident reporting channel. The Information Security Team shall treat the event as a security incident under the Incident Management Policy and simultaneously notify the DPO for privacy impact assessment.

### J.2 Breach Assessment

The DPO shall assess whether the event constitutes a personal data breach and, if so, whether it meets the threshold for supervisory authority notification within **72 hours** of the organisation becoming aware. The assessment shall consider:

- The nature of the data and the number of data subjects affected
- The likely consequences for data subjects: risk of identity theft, financial loss, discrimination, reputational damage, or physical harm
- Whether the data was encrypted, pseudonymised, or otherwise protected
- The cause and whether it has been contained
- Whether the breach involved special category data or children's data

**Breach Severity Classification:**

| Severity | Description | Notification Obligation |
|----------|-------------|------------------------|
| **Low** | Breach unlikely to result in risk to data subjects (e.g., encrypted device lost with no decryption key compromise) | No supervisory authority notification required; internal documentation only |
| **Medium** | Breach likely to result in risk to data subjects | Supervisory authority notification required within **72 hours**; individual notification assessed case by case |
| **High** | Breach likely to result in **high** risk to data subjects | Supervisory authority notification within **72 hours**; individual notification required **without undue delay** |

### J.3 Supervisory Authority Notification

Where notification is required, the DPO shall notify the relevant supervisory authority within **72 hours** of the organisation becoming aware of the breach. If not all information is available within 72 hours, initial notification shall be made with available information and supplemented as soon as possible. Notification shall include, where available:

- Description of the nature of the breach, including categories and approximate number of data subjects and records affected
- Name and contact details of the DPO
- Description of the likely consequences of the breach
- Description of the measures taken or proposed to address the breach and to mitigate possible adverse effects

Where notification is made after 72 hours, the DPO shall include reasons for the delay. Legal Counsel shall review all notifications before submission.

### J.4 Individual Notification

Where the breach is likely to result in a **high risk** to data subjects, the organisation shall notify affected individuals **without undue delay** in clear and plain language, including: the nature of the breach, the contact details of the DPO, the likely consequences, and the measures taken to address the breach. Communication shall be direct (not solely via a public notice) where reasonably practicable.

### J.5 Breach Register and Lessons Learned

All personal data breaches — regardless of whether they meet the notification threshold — shall be recorded in the breach register maintained by the GRC Team, including: incident reference, date of breach and date of discovery, description, affected data and data subjects, assessment outcome, notification decision and rationale, and remediation actions. The breach register shall be made available to supervisory authorities on request.

Breaches meeting the Medium or High threshold shall be subject to a post-incident review under the Incident Management Policy that specifically assesses privacy control gaps and identifies improvements to data protection measures.

---

## K. Privacy by Design and by Default

### K.1 Privacy by Design

Privacy by design requires that data protection is considered and built into systems and processes from the earliest stages of design, not added as a compliance afterthought. At Emyzer Nexus, privacy by design obligations apply to:

- All new system and application development by Emyzer Technology
- All new processing activities or material changes to existing activities
- All new AI system development or procurement
- All new product features that involve personal data processing

The DPO shall be engaged at the project initiation stage for any initiative involving personal data. The DPIA screening process (Section H.2, Step 1) is the formal mechanism for this engagement.

### K.2 Privacy by Default

Privacy by default requires that, by default, only the personal data necessary for each specific purpose is processed. This means:
- Data collection forms and API inputs shall collect only fields that are necessary for the stated purpose, with additional fields optional and clearly labelled
- System configurations shall apply the most privacy-protective settings as the default, with less protective options requiring deliberate user action to enable
- Data sharing defaults shall be restricted — data shall not be shared with third parties by default unless the data subject has actively opted in or another lawful basis applies
- Retention defaults shall apply the minimum retention period appropriate for the purpose

The DPO shall review privacy by default implementations for new systems and materially changed systems before go-live.

### K.3 AI System Design

For AI systems, privacy by design means:
- Minimising the personal data included in training datasets to what is technically necessary for the model's intended function
- Applying pseudonymisation or anonymisation to training data where technically feasible without materially compromising model performance
- Designing human oversight mechanisms that enable meaningful data subject rights fulfilment, including the ability to identify and correct training data errors
- Documenting design decisions that affect privacy (data inputs, retention of training data, output data containing inferences about individuals) in the technical documentation required under the AI Governance Policy
- Ensuring that AI system outputs that constitute inferences about individuals are handled as personal data where the individual is identified or identifiable

---

## L. Cross-Border Data Transfers

### L.1 Transfer Mechanism Requirements

Personal data shall not be transferred to a third country (outside the EU/EEA for GDPR purposes, or outside the UK for UK GDPR purposes) unless one of the following mechanisms is in place, documented in the ROPA, and verified by the DPO before the transfer commences:

**For GDPR (EU personal data):**
- European Commission adequacy decision covering the destination country
- Appropriate safeguards under GDPR Article 46: Standard Contractual Clauses (SCCs, 2021 version), Binding Corporate Rules, approved codes of conduct with binding commitments, approved certification mechanism
- Derogations under GDPR Article 49 for specific situations (explicit consent, contract performance necessity, vital interests) — applied narrowly and only where no other mechanism is available

**For UK GDPR (UK personal data):**
- UK adequacy regulations covering the destination country
- UK appropriate safeguards: International Data Transfer Agreement (IDTA), UK Addendum to EU SCCs, Binding Corporate Rules approved by the ICO
- Derogations under UK GDPR — applied on the same basis as GDPR derogations

### L.2 Transfer Impact Assessment

Where SCCs, the IDTA, or equivalent contractual mechanisms are used, the DPO shall conduct a Transfer Impact Assessment (TIA) evaluating whether the destination country's laws and practices allow the transfer mechanism to be effective. TIAs shall be documented and reviewed when circumstances change (e.g., new surveillance legislation in the destination country, relevant CJEU or UK court decisions).

### L.3 AI-Specific Transfer Considerations

LLM API calls that transmit personal data to a third-country provider constitute a cross-border transfer. The DPO shall assess the transfer mechanism status for each LLM API provider before personal data is included in API requests. Where no adequate transfer mechanism exists, personal data shall be pseudonymised or redacted before transmission, or the API shall not be used for purposes involving personal data until a transfer mechanism is established.

### L.4 Transfer Register

The DPO shall maintain a cross-border transfer register documenting each transfer, the applicable mechanism, the TIA reference where conducted, and the review date. The transfer register shall be reviewed **annually** and updated within **14 days** of any new transfer or change to transfer mechanism.

---

## M. Third-Party Data Processing Governance

### M.1 Data Processing Agreement Requirements

All third parties processing personal data on behalf of Emyzer Nexus shall be engaged under a written Data Processing Agreement meeting the requirements of GDPR Article 28. The DPA shall include:

- Subject matter, duration, nature, and purpose of the processing
- The type of personal data and categories of data subjects
- Obligations and rights of the controller
- The processor's obligation to process only on documented controller instructions
- Confidentiality obligations for authorised personnel
- Implementation of appropriate security measures under GDPR Article 32
- Sub-processor authorisation requirements and obligations
- Assistance obligations for data subject rights and DPIA obligations
- Deletion or return of data at the end of the service relationship
- Audit and inspection rights for the controller
- Notification obligations for personal data breaches without undue delay

Legal Counsel shall review and approve all DPAs before execution. No personal data shall be shared with a third-party processor without a signed DPA.

### M.2 Sub-Processor Management

Emyzer Nexus shall maintain a sub-processor register for each processor relationship. Where a processor proposes engaging a new sub-processor, Emyzer Nexus shall be notified in advance with sufficient information to assess the sub-processor's data protection practices. Emyzer Nexus shall have the right to object to new sub-processors within **30 days** of notification.

Where Emyzer Nexus acts as a processor for clients, the sub-processor register for those relationships shall be made available to the client on request, and new sub-processor notifications shall be made in accordance with the contractual terms.

### M.3 Processor Due Diligence

Before engaging a new processor, the DPO shall conduct privacy-specific due diligence as part of the Third-Party Risk Management Policy assessment process, covering:
- The processor's data protection practices and certifications (e.g., ISO 27701, ISO 27001)
- Security measures applied to the personal data to be processed
- Sub-processor practices and geographic processing locations
- Breach notification procedures and track record
- Data subject rights support capabilities

### M.4 Veridian AI Sub-Processing Legacy

The Veridian AI acquisition may have introduced existing sub-processing arrangements that predate the Emyzer Nexus DPA framework. The DPO shall review all processing agreements inherited through the acquisition within **60 days** of integration and remediate any gaps — replacing legacy arrangements with compliant DPAs or terminating relationships where compliance cannot be achieved.

---

## N. Consent Management

### N.1 Valid Consent Standards

Where consent is the lawful basis for processing, it must be:
- **Freely given:** Data subjects must have a genuine choice. Consent shall not be a condition of service unless the processing is necessary for that service.
- **Specific:** Consent shall be obtained for each distinct processing purpose. Bundled consent for multiple purposes is not valid.
- **Informed:** Data subjects shall receive clear information about who is processing their data, for what purpose, and their right to withdraw consent before giving it.
- **Unambiguous:** Consent shall be indicated by a clear affirmative act — a pre-ticked box, silence, or inactivity does not constitute valid consent.
- **Withdrawable:** Data subjects shall be able to withdraw consent as easily as they gave it. Withdrawal shall not affect the lawfulness of processing based on consent before withdrawal.

### N.2 Consent Records

The organisation shall maintain records demonstrating that consent was validly obtained, including: who consented, when, to what processing, and the consent mechanism used. Consent records shall be maintained for the duration of the processing plus 3 years, and shall be made available to supervisory authorities on request.

### N.3 Consent for AI Processing

Where AI systems process personal data on the basis of consent, the consent mechanism must clearly explain that AI processing is involved, what the AI system does, and whether automated decision-making with significant effects will take place. Generic consent to "data processing" does not cover AI-specific processing activities where a reasonable person would not have anticipated that use.

---

## O. Compliance and Monitoring

### O.1 Monitoring Activities

| Activity | Frequency | Owner |
|----------|-----------|-------|
| ROPA completeness and accuracy review | Quarterly | GRC Team / DPO |
| Data subject request tracker review | Monthly | DPO |
| Privacy notice currency review | Annual | DPO |
| DPIA register review | Quarterly | DPO |
| Cross-border transfer register review | Annual | DPO |
| Retention compliance review | Annual | GRC Team / DPO |
| DPA register completeness review | Quarterly | GRC Team / DPO |
| Consent record audit | Annual | DPO |
| AI system DPIA status review | Monthly (until complete for Veridian AI systems) | DPO / AI Governance Committee |
| Privacy compliance report to Security Steering Committee | Quarterly | DPO |
| Policy compliance audit (part of ISMS audit) | Annual | Internal Audit |

### O.2 Key Performance Indicators

| KPI | Target | Measurement Frequency |
|-----|--------|----------------------|
| ROPA completeness (all processing activities registered) | 100% | Quarterly |
| Processing activities with documented lawful basis | 100% | Quarterly |
| DPIAs completed before processing commencement | 100% (for mandatory cases) | Per project |
| Data subject requests completed within statutory deadline | ≥98% | Monthly |
| Personal data breach supervisory authority notifications within 72 hours | 100% (where applicable) | Per incident |
| DPAs in place for all active processors | 100% | Quarterly |
| Cross-border transfers with documented transfer mechanism | 100% | Quarterly |
| High-Risk AI system DPIAs approved before deployment | 100% | Per deployment |
| Privacy notices reviewed within the past 12 months | 100% | Annual |
| Open DPIA findings with remediation plans | 100% | Quarterly |

### O.3 Non-Compliance

Processing personal data without a documented lawful basis, failing to conduct a required DPIA before processing commencement, or sharing personal data with a processor without a DPA constitutes a critical compliance failure, triggering immediate escalation to the DPO, Legal Counsel, and CEO. Processing shall be suspended pending DPO review. Other non-compliance shall be addressed through documented corrective action plans within **30 days** of identification.

---

## P. Policy Exceptions

### P.1 Exception Process

Business units requiring temporary deviation from this policy shall:
1. Submit exception requests via **ServiceNow GRC workflow** with documented justification, risk assessment, and proposed compensating measures.
2. Obtain DPO approval. Exceptions affecting DPIA obligations or cross-border transfer mechanisms shall also require Legal Counsel review.
3. Exceptions are valid for a maximum of **90 days** and require DPO review before renewal. No exception shall permit processing of personal data without any lawful basis or DPIA where one is mandatory.

### P.2 Exception Governance

- Active exceptions reviewed **quarterly** by the DPO and GRC Team.
- Exception register maintained in the GRC platform.
- Exception metrics included in the quarterly privacy compliance report.

---

## Q. Related Policies

1. [**Information Security Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/information-security-policy.md) *(KB-PORTFOLIO-0001)* — Parent policy. Establishes the ISMS within which the Privacy Information Management System (PIMS) operates. Information security controls under GDPR Article 32 are governed jointly by this policy and the Information Security Policy.

2. [**Risk Management Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/risk-management-policy.md) *(KB-PORTFOLIO-0002)* — Privacy risks are registered in the enterprise risk register as a distinct risk category under CRO and DPO joint ownership.

3. [**Data Classification Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/data-classification-policy.md) *(KB-PORTFOLIO-0003)* — The data classification framework governs the handling of personal data by tier. Special category data is classified at minimum as Restricted.

4. [**AI Governance Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/ai-governance-policy.md) *(KB-PORTFOLIO-0011)* — Governs High-Risk AI systems processing personal data. DPIAs under this policy and conformity assessments under the AI Governance Policy are conducted as coordinated processes for AI systems in scope of both.

5. [**Model Risk Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/model-risk-policy.md) *(KB-PORTFOLIO-0012)* — Model development data governance requirements under Section G.2.2 are coordinated with DPIA training data obligations under this policy.

6. [**Third-Party Risk Management Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/third-party-risk-management-policy.md) *(KB-PORTFOLIO-0008)* — Privacy due diligence requirements are embedded in the third-party risk assessment process. DPA execution is a prerequisite for vendor onboarding where personal data processing is involved.

7. [**Incident Management Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/incident-management-policy.md) *(KB-PORTFOLIO-0006)* — Personal data breaches are managed through the security incident response process with this policy governing the regulatory notification dimension.

8. [**Security Awareness and Training Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/security-awareness-training-policy.md) *(KB-PORTFOLIO-0014)* — Data protection training for all personnel and specialist training for the DPO and Privacy team are governed under the Security Awareness and Training Policy.

---

## R. Related Documents

1. Record of Processing Activities (ROPA) — Controller
2. Record of Processing Activities (ROPA) — Processor
3. DPIA Register and Tracking Log
4. DPIA Template and Guidance
5. Legitimate Interests Assessment (LIA) Template
6. Data Subject Request Procedure
7. Data Subject Request Tracker
8. Personal Data Breach Response Procedure
9. Breach Register
10. Data Processing Agreement Template
11. Sub-Processor Register
12. Cross-Border Transfer Register
13. Transfer Impact Assessment Template
14. Privacy Notice Templates (Employee; Customer; Prospect; Website)
15. Consent Management Procedure
16. Retention Schedule
17. Privacy by Design Checklist
18. AI System DPIA Template (coordinated with AI Governance conformity assessment)

---

## S. Review and Revision

This policy shall be reviewed **annually** or upon: material changes to GDPR or UK GDPR implementing guidance or EDPB/ICO opinions; a personal data breach revealing governance gaps; significant new processing activities (including new AI systems processing personal data); relevant CJEU or UK court decisions affecting transfer mechanisms or processing lawfulness; or changes to the AI Governance Policy affecting the DPIA coordination process. All revisions require CEO approval. Material changes affecting data subject rights procedures or breach notification obligations shall be communicated to all employees **within 10 business days** of approval.

---

## T. Framework Alignment

| Framework | Alignment |
|-----------|-----------|
| **EU GDPR (Regulation 2016/679)** | Article 5 (Data protection principles), Article 6 (Lawful basis), Article 7 (Consent), Article 9 (Special categories), Articles 12–23 (Data subject rights), Article 25 (Privacy by design and default), Article 28 (Processors and DPAs), Article 30 (ROPA), Article 32 (Security of processing), Article 33 (Breach notification to supervisory authority), Article 34 (Communication to data subjects), Article 35 (DPIA), Article 36 (Prior consultation), Article 37–39 (DPO), Articles 44–49 (Cross-border transfers) |
| **UK GDPR** | Equivalent to EU GDPR provisions as retained and adapted in UK law; ICO guidance applied for UK-specific obligations including IDTA for international transfers |
| **ISO/IEC 27701:2019** | Clause 5 (PIMS requirements for controllers and processors — extending ISO 27001 Clause 4–10), Clause 6 (PIMS guidance for controllers), Clause 7 (PIMS guidance for processors), Annex A (Controller-specific control requirements), Annex B (Processor-specific control requirements), Annex D (Mapping to GDPR) |
| **ISO/IEC 27001:2022** | Clause 6.1 (Risk management — privacy risks in ISMS risk assessment), A.5.34 (Privacy and protection of PII), A.8.11–A.8.12 (Data masking and DLP controls for personal data) |
| **NIST Privacy Framework 1.0** | IDENTIFY-P (data processing inventory and ROPA), GOVERN-P (privacy governance structure and DPO function), CONTROL-P (data subject rights and consent management), COMMUNICATE-P (privacy notices and transparency), PROTECT-P (privacy by design and security controls) |
| **EU AI Act (Regulation 2024/1689)** | Recital 47 (AI systems processing personal data — interaction with GDPR), Article 10 (Data governance obligations for training data — coordinated with DPIA data minimisation assessment), Article 13 (Transparency — coordinated with privacy notice obligations), Article 22 (Interaction with GDPR Article 22 automated decision-making rights) |
| **EDPB Guidelines** | Guidelines 09/2022 (DPIA criteria — mandatory processing types), Guidelines 05/2022 (Consent), Guidelines 07/2020 (Automated decision-making), Guidelines 05/2021 (Cross-border transfers — SCCs), Guidelines 01/2021 (Interplay of GDPR and ePrivacy Directive) |
| **ICO Guidance** | ICO Data Sharing Code of Practice, ICO DPIA Guidance, ICO Legitimate Interests Guidance, ICO International Transfers Guidance (IDTA) |

---

## U. Organisational Benefit

| Benefit Area | Description |
|--------------|-------------|
| **Regulatory Risk Reduction** | Documented lawful bases, complete ROPA, DPIAs before high-risk processing, 72-hour breach notification, and DPA coverage for all processors directly reduce the risk of GDPR/UK GDPR enforcement action and associated financial penalties |
| **Acquisition Risk Management** | The Veridian AI DPIA process provides a structured mechanism for assessing and governing the privacy implications of inherited processing activities — converting an unquantified acquisition risk into a managed compliance programme with a tracked remediation timeline |
| **Client Trust and Commercial Advantage** | Enterprise and regulated-industry clients require suppliers to demonstrate GDPR compliance before contract award. DPA readiness, ROPA availability, and DPIA capability are evaluated in client due diligence processes. Privacy governance maturity is a commercial differentiator |
| **AI Governance Integration** | Coordinating DPIA and conformity assessment processes eliminates duplication, ensures consistency, and demonstrates to regulators that AI privacy risks are managed holistically rather than as separate compliance workstreams |
| **Data Subject Confidence** | Rights fulfilment within statutory deadlines, clear privacy notices, and accessible consent management build the data subject trust that underpins customer relationships in markets where individuals are increasingly aware of their privacy rights |
| **Breach Preparedness** | Defined breach assessment criteria, 72-hour notification governance, and coordinated response between the Incident Management Policy and this policy reduce regulatory and reputational exposure when incidents occur |
| **ISO 27701 Alignment** | Extending the ISMS to a PIMS under ISO 27701 positions Emyzer Nexus for certification that signals privacy governance maturity to enterprise clients, regulated-sector partners, and supervisory authorities |
| **Employee Confidence** | Clear policies on how employee personal data is handled, subject access request processes that work, and data protection training that explains obligations in context build internal trust in the organisation's privacy culture |

---

## V. Evidence of Compliance

| Evidence Type | System of Record | Owner | Retention Period |
|---------------|------------------|-------|------------------|
| Record of Processing Activities — Controller | GRC Platform | DPO / GRC Team | Indefinite (current version with full revision history) |
| Record of Processing Activities — Processor | GRC Platform | DPO / GRC Team | Indefinite (current version with full revision history) |
| Lawful Basis Documentation | GRC Platform | DPO | Life of processing activity + 5 years |
| Legitimate Interests Assessments | Document Repository | DPO | Life of processing activity + 5 years |
| DPIA Register | GRC Platform | GRC Team | Indefinite |
| Completed DPIA Reports | Document Repository | DPO | Life of processing activity + 7 years |
| DPIA Supervisory Authority Prior Consultation Records | Legal Repository | Legal Counsel | 10 years |
| DPO Advisory Records | Document Repository | DPO | 5 years |
| Privacy Notice Version History | Document Repository | DPO | 5 years from version retirement |
| Consent Records | CRM / Marketing Platform | DPO / GRC Team | Duration of consent + 3 years |
| Data Subject Request Tracker | GRC Platform | GRC Team | 5 years |
| Data Subject Request Correspondence | Document Repository | DPO | 5 years |
| Personal Data Breach Register | GRC Platform | GRC Team | 10 years |
| Supervisory Authority Breach Notifications | Legal Repository | Legal Counsel / DPO | 10 years |
| Supervisory Authority Correspondence (all) | Legal Repository | Legal Counsel | 10 years |
| Data Processing Agreements Register | GRC Platform | GRC Team | Contract duration + 7 years |
| Executed DPAs | Legal Repository | Legal Counsel | Contract duration + 7 years |
| Sub-Processor Registers | GRC Platform | GRC Team | Contract duration + 5 years |
| Cross-Border Transfer Register | GRC Platform | DPO / GRC Team | Duration of transfer + 5 years |
| Transfer Impact Assessments | Document Repository | DPO | Duration of transfer + 5 years |
| Retention Schedule | Document Repository | DPO | 5 years from version retirement |
| Annual Retention Compliance Review | GRC Platform | DPO / GRC Team | 5 years |
| Privacy Due Diligence Records (vendor) | GRC Platform | GRC Team | Contract duration + 5 years |
| Veridian AI Privacy Assessment Records | Document Repository | DPO | 7 years |
| Policy Acknowledgement Records | GRC Platform / HR System | Human Resources | Employment duration + 3 years |
| Annual Privacy Compliance Audit Reports | GRC Platform | Internal Audit | 7 years |

---

## Approval History

| Date | Approver | Status | Comments |
|------|----------|--------|----------|
| 2025-10-01 | Chief Executive Officer | Approved | "The intersection of GDPR and EU AI Act obligations for the Veridian AI systems is the most immediate compliance priority, and this policy provides the governance structure to address it systematically. The DPIA coordination process between the DPO and AI Governance Committee is well-designed. The DPO function's independence and reporting line to the CEO is appropriately structured. Approved." |

---

## Document Control

- **Document ID:** KB-PORTFOLIO-0013
- **Version:** 1.0
- **Classification:** Internal
- **Last Updated:** 2025-10-01
- **Next Review Date:** 2026-10-01

---

*This policy document was developed as part of the Emyzer Nexus Phase 2 GRC programme and formatted for portfolio presentation. It operates within the ISMS established by the Information Security Policy (KB-PORTFOLIO-0001) and extends it to a Privacy Information Management System (PIMS) aligned to ISO/IEC 27701:2019.*

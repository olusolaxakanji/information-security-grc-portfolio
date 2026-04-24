# Security Awareness and Training Policy

**Emyzer Nexus – Governance, Risk, and Compliance**

---

## Policy Metadata

| Attribute | Value |
|-----------|-------|
| **Policy Name** | Security Awareness and Training Policy |
| **Type** | Policy |
| **Version** | 1.0 |
| **Parent Policy** | Information Security Policy (KB-PORTFOLIO-0001) |
| **Owner** | Chief Information Security Officer |
| **Owning Group** | App Engine Admins |
| **State** | Published |
| **Valid From** | 2025-11-01 |
| **Valid To** | 2026-11-01 |
| **Approvers** | Chief Executive Officer |
| **Reviewers** | Chief Risk Officer; GRC Analyst; Human Resources Director; Legal Counsel |
| **Knowledge Base** | Governance, Risk, and Compliance |
| **Published Policy** | KB-PORTFOLIO-0014 |

---

## Description

This policy establishes the governance framework for security awareness and training across Emyzer Nexus and its subsidiaries, consolidating training obligations currently distributed across the Information Security Policy, AI Governance Policy, Model Risk Policy, Acceptable Use Policy, Incident Management Policy, and Third-Party Risk Management Policy into a single, authoritative governance document.

**Impact:** Human behaviour remains one of the most significant contributors to information security incidents. Untrained or undertrained personnel are the primary vector for phishing attacks, data handling errors, AI misuse, and access control violations. A structured, role-differentiated training program — with measurable completion requirements and defined consequences for non-compliance — reduces this risk systematically rather than reactively. For Emyzer Nexus, the Veridian AI acquisition introduced personnel with varied security cultures and awareness baselines, making a consistent enterprise-wide training program operationally essential.

**Relevant Standards:** NIST SP 800-50 Rev. 1 (Building a Cybersecurity and Privacy Learning Program), NIST SP 800-16 Rev. 1 (Cybersecurity Workforce Framework), ISO/IEC 27001:2022 (Annex A Controls A.6.3, A.7.2), ISO/IEC 27002:2022 (Controls 6.3, 7.2), NIST CSF 2.0 (GV.RR, PR.AT)

---

## Policy Snapshot

| Dimension | Summary |
|-----------|---------|
| **Applies to** | All Emyzer Nexus employees, contractors, temporary workers, board members, and third parties with access to Emyzer Nexus information systems or data — including personnel acquired through the Veridian AI integration |
| **Covers** | All security awareness, role-based security training, AI and model risk training, phishing simulation, specialist training, and training completion governance across the organisation |
| **Training Tracks** | General Awareness (all personnel); Role-Based (IT, GRC, Legal, Finance, HR, executives, developers, AI/ML operators, model users); Specialist (incident responders, privileged access holders, data protection officers) |
| **Completion Deadlines** | General awareness: within 30 days of start date; annually thereafter. Role-based training: within 60 days of role assignment; on material curriculum change. Specialist training: within 30 days of role assignment |
| **Key Governance** | CISO owns the program; Human Resources manages scheduling, records, and escalation; GRC Team produces compliance reporting; managers enforce completion within their teams |
| **Exceptions Process** | ServiceNow workflow with CISO approval; maximum 90-day duration; quarterly review of active exceptions |
| **Evidence Maintained** | Training completion records, curriculum version history, phishing simulation results, non-completion escalation records, curriculum review documentation, training effectiveness assessments (all with defined retention periods) |

---

## A. Purpose

To establish the governance framework, minimum standards, and accountability structures for security awareness and training across Emyzer Nexus, ensuring that all personnel — regardless of role, seniority, or employment type — have the knowledge and skills necessary to fulfil their security obligations, respond appropriately to security incidents, and use AI and technology systems responsibly.

This policy consolidates training obligations currently distributed across six subordinate policies into a single governance document with unified completion tracking, escalation procedures, and curriculum review requirements. Consolidation eliminates the risk of training gaps arising from obligations existing in policies that personnel may not read, ensures that role-specific training requirements are visible to Human Resources and line managers without requiring policy-by-policy review, and provides a single point of compliance reporting for the organisation's security training posture.

The policy recognises that effective security awareness is not a compliance checkbox. It is a continuous risk reduction program that requires curriculum grounded in real threat scenarios, delivery formats matched to how people actually learn, measurable effectiveness assessment, and governance structures that create genuine accountability — not just completion records. A training program that generates 100% completion against irrelevant curriculum has accomplished less than one achieving 85% completion against content that changes behaviour.

---

## B. Scope

### B.1 Personnel in Scope

This policy applies to all individuals who access Emyzer Nexus information systems, data, or facilities, including:

- All permanent employees of Emyzer Nexus and its subsidiaries, including Emyzer Technology
- All personnel acquired through the Veridian AI integration, effective from their first day operating under Emyzer Nexus systems access
- Contractors, consultants, and temporary workers engaged for 30 days or longer, or with access to Confidential or Restricted data regardless of engagement duration
- Board members and non-executive directors in relation to executive awareness obligations
- Third-party personnel with persistent access to Emyzer Nexus systems or data, as specified in third-party agreements

Short-term contractors engaged for fewer than 30 days with access limited to Public or Internal data shall complete a condensed security briefing in lieu of the full general awareness curriculum, documented in the training record system.

### B.2 Training Obligations Consolidated by This Policy

The following training requirements, previously distributed across subordinate policies, are governed by this policy:

| Originating Policy | Training Obligation | Now Governed Under |
|-------------------|--------------------|--------------------|
| AI Governance Policy (KB-PORTFOLIO-0011) | AI awareness training within 30 days of hire; annually thereafter | Section F.2 — General Awareness Curriculum; Section F.3 — AI and Responsible Technology Track |
| AI Governance Policy (KB-PORTFOLIO-0011) | Operator training for High-Risk AI systems before operational access | Section F.4 — Role-Based Training: AI System Operators |
| Model Risk Policy (KB-PORTFOLIO-0012) | Model-specific user training before operational access to Tier 1 or Tier 2 models | Section F.4 — Role-Based Training: Model Users |
| Acceptable Use Policy (KB-PORTFOLIO-0004) | Acceptable use awareness at onboarding | Section F.2 — General Awareness Curriculum |
| Incident Management Policy (KB-PORTFOLIO-0006) | Incident response training for responders and on-call personnel | Section F.5 — Specialist Training: Incident Response |
| Third-Party Risk Management Policy (KB-PORTFOLIO-0008) | Vendor risk awareness for personnel with third-party oversight responsibilities | Section F.4 — Role-Based Training: Procurement and Vendor Management |
| Access Control Policy (KB-PORTFOLIO-0005) | Privileged access training before elevated access provisioning | Section F.5 — Specialist Training: Privileged Access Holders |

### B.3 Exclusions

Operational technology systems in air-gapped or isolated environments are excluded from LMS-delivered training completion tracking where system architecture prevents network access, provided that equivalent in-person training delivery with manual completion records is implemented and reported to the GRC Team quarterly. No personnel exclusion from security awareness obligations is permitted.

---

## C. Definitions

| Term | Definition |
|------|------------|
| **Security Awareness** | The baseline understanding of information security threats, responsibilities, and expected behaviours required of all personnel, regardless of technical role. Distinct from security training in that awareness seeks to change attitudes and recognise risks; training seeks to build specific skills. |
| **Security Training** | Structured instruction designed to develop specific security-related skills in personnel whose roles require them — such as incident response, secure development, AI system operation, or model risk management. |
| **Learning Management System (LMS)** | The platform used to deliver, track, and report on training completion across Emyzer Nexus. The system of record for all training completion evidence. |
| **Training Track** | A defined set of training modules required for a specific population — general awareness, role-based, or specialist — delivered on defined cadences and completion timelines. |
| **Curriculum** | The complete set of training content comprising a training track, including modules, assessments, simulations, and any supplementary materials. |
| **Completion Record** | A timestamped LMS entry confirming that a named individual has completed a specified training module, including assessment outcome where applicable. The primary compliance evidence for this policy. |
| **Phishing Simulation** | A controlled, internally managed simulation of phishing attacks used to test personnel susceptibility, measure awareness program effectiveness, and trigger targeted remedial training for individuals who fail the simulation. |
| **Remedial Training** | Mandatory additional training assigned to personnel who fail a phishing simulation, fail a knowledge assessment below the defined passing threshold, or are identified as having contributed to a security incident through an awareness or training gap. |
| **AI and Responsible Technology Track** | The training track covering responsible AI use, acceptable use of generative AI tools, AI risk identification, and obligations under the AI Governance Policy. Required for all personnel as part of general awareness, with deeper modules for AI system operators and model users. |
| **Role-Based Training** | Training modules assigned based on an individual's function, system access, or data handling responsibilities, beyond the general awareness curriculum required of all personnel. |
| **Specialist Training** | Advanced training required for personnel in functions with elevated security responsibilities — incident responders, privileged access holders, data protection officers, and AI system operators of High-Risk systems. |
| **Training Effectiveness Assessment** | A structured evaluation of whether training has achieved its intended behaviour change outcomes, conducted annually using metrics including phishing simulation click rates, knowledge assessment scores, and incident root cause analysis. |
| **Onboarding Training** | The subset of required training that must be completed within defined deadlines at the start of an employment or contractor engagement. |
| **Material Curriculum Change** | An update to training content that substantially alters the knowledge or behaviour requirements communicated to personnel, triggering re-completion obligations. Distinguished from editorial updates, which do not require re-completion. |
| **Non-Completion Escalation** | The formal process by which training non-compliance is escalated from the LMS through line management to HR and ultimately to system access suspension, as defined in Section G. |

---

## D. Policy Statement

Emyzer Nexus recognises that its people are both the organisation's most significant security vulnerability and its most effective security control. The organisation's approach to security awareness and training reflects this duality: the program exists not to protect the organisation from its people, but to equip its people to protect the organisation and its customers. The organisation shall:

1. Deliver **general security awareness training** to all in-scope personnel within **30 days** of their start date and **annually** thereafter, covering the core security obligations, threat landscape, and behavioural expectations applicable to every person in the organisation.

2. Deliver **role-based training** to personnel in functions with specific security obligations within **60 days** of role assignment, ensuring that the people responsible for information security, AI governance, model risk, incident response, and vendor management have the knowledge to fulfil those responsibilities.

3. Deliver **specialist training** to personnel with elevated security responsibilities — including incident responders, privileged access holders, High-Risk AI system operators, and Tier 1 and Tier 2 model users — **before** those individuals are granted the access or operational authority their role requires. Specialist training is a **prerequisite for access**, not a parallel obligation.

4. Conduct **phishing simulations** at least **quarterly** across all in-scope personnel, using results to measure program effectiveness, identify population-level awareness gaps, and assign targeted remedial training to individuals who fail simulations.

5. Maintain **complete and accurate training records** in the LMS for all in-scope personnel, providing the CISO, GRC Team, and Human Resources with the information necessary to assess compliance and escalate non-completion.

6. Enforce **non-completion consequences** through a structured escalation process that, for persistent non-completion, results in suspension of system access pending completion — making training completion a genuine operational requirement rather than an aspirational one.

7. Review and refresh **curriculum content annually** to reflect the current threat landscape, regulatory developments, and lessons learned from security incidents — ensuring that training remains relevant to the risks people actually face, not the risks the organisation faced when the curriculum was first built.

8. Assess **training effectiveness** annually, using metrics beyond completion rates — including phishing simulation outcomes, knowledge assessment scores, and security incident root cause analysis — to determine whether the program is achieving measurable behaviour change.

9. Ensure that **Veridian AI personnel** complete all applicable onboarding training obligations within **60 days** of integration into Emyzer Nexus systems, with integration-specific modules covering the differences between Veridian AI's previous practices and Emyzer Nexus standards.

10. Review and update this policy **annually** or following a significant security incident in which an awareness or training gap contributed to the incident's occurrence or impact.

---

## E. Roles and Responsibilities

### E.1 Chief Executive Officer (CEO)
Approves the Security Awareness and Training Policy. Shall complete executive awareness training **within 30 days** of policy publication and **annually** thereafter, demonstrating visible leadership commitment to security culture. Receives **annual** training effectiveness reports from the CISO.

### E.2 Chief Information Security Officer (CISO)
Owns the security awareness and training program. Shall approve the annual training curriculum, phishing simulation schedule, and training effectiveness assessment methodology. Shall review non-completion escalation reports **monthly** and report training compliance posture to executive leadership **quarterly**. Shall present the annual training effectiveness assessment to the Security Steering Committee and recommend curriculum changes based on findings.

### E.3 Human Resources Director
Jointly responsible with the CISO for training program governance. Shall ensure training completion requirements are integrated into onboarding workflows, role change processes, and contractor engagement procedures. Shall manage the non-completion escalation process from line manager notification through to HR action (Section G). Shall provide the GRC Team with accurate and current personnel and role data to support training track assignment. Shall retain training completion records in accordance with Section N.

### E.4 GRC Team
Shall maintain the training compliance dashboard in the GRC platform, produce **monthly** non-completion reports for the CISO and Human Resources, coordinate the annual training effectiveness assessment, and manage the exceptions log. Shall conduct **quarterly** audits of LMS completion data against the personnel register to identify unclosed gaps and ensure training track assignments reflect current roles.

### E.5 Line Managers
Shall ensure that all direct reports complete assigned training within the required deadlines. Shall monitor LMS completion alerts for their teams and escalate persistent non-completion to Human Resources within **5 business days** of the non-completion escalation threshold being reached. Shall support training delivery by facilitating time for team members to complete training during working hours and treating training completion as a performance expectation.

### E.6 Information Security Team
Shall design and maintain the security awareness and training curriculum in collaboration with the GRC Team and Human Resources. Shall manage phishing simulation execution, results analysis, and remedial training assignment. Shall incorporate lessons learned from security incidents into curriculum updates. Shall advise the CISO on emerging threats requiring curriculum additions between annual review cycles.

### E.7 AI Governance Committee (Joint Responsibility)
Shall approve the AI and Responsible Technology training track curriculum and review AI-related training effectiveness metrics **annually**, in conjunction with the CISO. Shall determine when changes to AI governance obligations require material curriculum updates triggering re-completion obligations.

### E.8 All Personnel
Shall complete all assigned training within the required deadlines. Shall complete knowledge assessments embedded in training modules with a passing score of **80% or above** (one re-attempt permitted before remedial training is assigned). Shall report security concerns, suspicious activity, and potential incidents through the channels covered in general awareness training. Shall apply the knowledge and behaviours covered in training to their daily work — not treat training as a compliance exercise disconnected from operational practice.

---

## F. Training Program Requirements

### F.1 Training Track Structure

The security awareness and training program comprises three tracks. Every in-scope individual completes at least the General Awareness Track. Role-Based and Specialist training is assigned based on function and access level.

```
General Awareness Track (ALL PERSONNEL)
│
├── Role-Based Track (ASSIGNED BY FUNCTION)
│   ├── IT and Security Personnel
│   ├── GRC and Risk Personnel
│   ├── Legal and Compliance Personnel
│   ├── Finance and Accounts
│   ├── Human Resources
│   ├── Executive and Senior Leadership
│   ├── Software Developers and Engineers
│   ├── Procurement and Vendor Management
│   ├── AI System Operators (High-Risk AI Systems)
│   └── Model Users (Tier 1 and Tier 2 Models)
│
└── Specialist Track (PREREQUISITE FOR ACCESS/ROLE)
    ├── Incident Response Personnel
    ├── Privileged Access Holders
    └── Data Protection Officer and Privacy Team
```

### F.2 General Awareness Track

**Required of:** All in-scope personnel.
**Completion deadline:** Within **30 days** of start date; **annually** thereafter.
**Passing threshold:** 80% on embedded knowledge assessments.

The General Awareness Track shall cover, at minimum:

**F.2.1 Security Foundations**
- The organisation's information security obligations and why they matter
- The most significant threats facing Emyzer Nexus and its industry: phishing and social engineering, credential compromise, ransomware, data handling errors, and insider risk
- How to identify and report suspicious activity, phishing attempts, and potential security incidents
- The organisation's incident reporting channels and what to expect after a report is made

**F.2.2 Data Handling and Classification**
- The four-tier data classification framework (Public, Internal, Confidential, Restricted) with worked examples relevant to the individual's role context
- Acceptable storage, transmission, and sharing practices for each classification tier
- Personal data handling obligations under GDPR, including what constitutes personal data, what lawful basis means in practice, and how to handle data subject requests
- What to do — and who to contact — when a data handling error occurs

**F.2.3 Acceptable Use**
- Acceptable and unacceptable use of Emyzer Nexus information systems, including personal device use, remote working, and cloud storage
- The organisation's position on generative AI tool use with organisational data, including the prohibition on inputting Confidential or Restricted data into external LLM APIs without approved controls
- Password and authentication requirements, including multi-factor authentication obligations and what to do if credentials are compromised
- The consequences of acceptable use policy violations

**F.2.4 AI and Responsible Technology (Baseline)**
- What artificial intelligence is and how Emyzer Nexus uses AI systems
- The organisation's AI governance obligations and why they exist
- How to identify whether an AI system is in use in a workflow and what the governance implications are
- How to report unexpected AI system outputs, apparent bias, or AI-related concerns
- The prohibition on deploying, integrating, or procuring AI systems without AI Governance Committee review
- The specific obligations of the Acceptable Use Policy regarding generative AI tools

**F.2.5 Physical and Environmental Security**
- Workstation and screen locking requirements
- Clean desk and clear screen practices for personnel handling Confidential or Restricted data
- Visitor management and tailgating awareness
- Secure disposal of physical documents and media

### F.3 AI and Responsible Technology Track

**Required of:** All personnel identified as frequent users of AI-assisted tools, AI output consumers in business workflows, or personnel working in AI-adjacent functions (product management, commercial, legal, finance roles interfacing with AI outputs).
**Completion deadline:** Within **60 days** of role identification or tool deployment; **annually** thereafter.
**Note:** This track extends the baseline AI module in the General Awareness Track. Personnel assigned this track shall complete the General Awareness Track first.

The AI and Responsible Technology Track shall cover:

- How the organisation's AI systems work at a conceptual level — what they do, what data they process, and what their outputs are used for
- The EU AI Act risk classification framework and what High-Risk classification means for how systems must be used
- Bias in AI systems: what it is, how it arises, how to recognise potential bias in outputs, and how to report it
- Human oversight obligations: what it means to maintain meaningful human review of AI outputs, when overriding an AI output is appropriate, and how overrides are documented
- Responsible use of generative AI tools in the workplace: capability and limitation awareness, hallucination risk, appropriate and inappropriate use cases, and data input restrictions
- The organisation's AI incident reporting obligations and channels

### F.4 Role-Based Training

Role-based training is assigned by Human Resources in consultation with the GRC Team based on the individual's function and system access profile. Completion is required within **60 days** of role assignment and annually thereafter, or within **30 days** of a material curriculum change.

**F.4.1 IT and Security Personnel**
- Secure network architecture and segmentation principles
- Security monitoring tools and alert triage
- Endpoint detection and response (EDR) platform operation
- Log management and SIEM query fundamentals
- Identity and access management administration

**F.4.2 GRC and Risk Personnel**
- Risk assessment methodology and risk register management
- Policy governance lifecycle and exception management
- Compliance monitoring and evidence collection
- Third-party risk assessment and due diligence
- Regulatory mapping — ISO 27001:2022, NIST CSF 2.0, EU AI Act, GDPR

**F.4.3 Legal and Compliance Personnel**
- GDPR and UK GDPR obligations in practice
- EU AI Act legal obligations — prohibited practices, High-Risk system requirements, regulatory notification obligations
- Data subject rights request handling
- Regulatory investigation and audit response procedures
- Contract review for security and data protection obligations

**F.4.4 Finance and Accounts**
- Business email compromise and invoice fraud recognition
- Financial data classification and handling requirements
- Vendor payment process security controls
- Fraud reporting procedures

**F.4.5 Human Resources**
- Personal data handling in HR systems
- Background screening and reference check security
- Insider threat indicators and reporting channels
- Employee offboarding security obligations (account deprovisioning, asset return, data access removal)
- Training compliance monitoring and escalation procedures

**F.4.6 Executive and Senior Leadership**
- The executive threat landscape: spear phishing, whaling, vishing, and deepfake social engineering
- Executive travel security and public Wi-Fi risks
- How the organisation's AI governance and security risk posture is reported to leadership — and what good looks like
- Board-level security incident escalation and communication obligations
- Regulatory and reputational risk context for security and AI governance decisions

**F.4.7 Software Developers and Engineers**
- Secure software development lifecycle (SSDLC) practices
- OWASP Top 10 with application to Emyzer Technology's development environment
- Secure code review practices and common vulnerability patterns
- Dependency management and supply chain security
- AI system and ML pipeline security: training data integrity, model artefact protection, prompt injection risks in LLM-integrated applications, and adversarial input testing

**F.4.8 Procurement and Vendor Management**
- Third-party risk management lifecycle overview
- Vendor security due diligence requirements and red flags
- AI vendor due diligence addendum obligations
- Contract security requirements: minimum clauses, right to audit, incident notification SLAs
- Vendor offboarding and access termination security obligations

**F.4.9 AI System Operators — High-Risk AI Systems**

This track is a **prerequisite for access** to any High-Risk AI system. Operators shall complete this training before being granted operational access. Training is system-specific and shall be developed and maintained by the relevant AI System Owner in coordination with the Information Security Team.

Content shall cover, at minimum:
- The specific High-Risk AI system's purpose, capabilities, known limitations, and documented failure modes
- The system's EU AI Act classification, what High-Risk classification means in practice, and the operator's specific obligations under that classification
- How to interpret system outputs correctly, including the confidence levels, output formats, and conditions under which outputs are less reliable
- Human oversight obligations: when human review is required before acting on outputs, when outputs may be used without additional review, and how to document override decisions
- How to recognise unexpected, anomalous, or potentially biased outputs and the reporting requirements that follow
- The system's post-market monitoring program: what metrics are being tracked, what amber and red thresholds mean, and the operator's role in monitoring
- The system's override log procedure: how to record an override, what information is required, and the review process that follows
- Emergency procedures: how to halt the system in cases of serious risk and who to contact

Operator training shall be reviewed and updated by the AI System Owner following any material change to the system, with re-completion required if the update is classified as material curriculum change.

**F.4.10 Model Users — Tier 1 and Tier 2 Models**

This track is a **prerequisite for access** to Tier 1 and Tier 2 model outputs in decision-making workflows. Model Users shall complete this training before being granted access. Training is model-specific and shall be developed and maintained by the relevant Model Owner in coordination with the Information Security Team.

Content shall cover, at minimum:
- The model's purpose, intended use, and validated scope of applicability
- The model's documented limitations and the conditions under which outputs may be less reliable or invalid — including the signed limitation disclosure required under the Model Risk Policy
- How to interpret model outputs correctly and what the outputs do and do not mean for decision-making
- The boundaries of validated use: what decisions the model is approved to inform, what falls outside validated scope, and the approval process required for out-of-scope use
- Override and adjustment procedures: when a model output may be adjusted, how to document it, and the approval required
- Reporting obligations: how to report unexpected model outputs, anomalies, or concerns to the Model Owner within 24 hours
- The human review requirements for the specific model: when outputs require human review before action and what that review must include

Model User training shall be reviewed and updated by the Model Owner following any material change to the model, with re-completion required if the update is classified as material curriculum change.

### F.5 Specialist Training

Specialist training is a **prerequisite for role assignment or access provisioning**, not a parallel obligation. No individual shall be granted the access or authority their specialist role requires until specialist training is confirmed complete in the LMS.

**F.5.1 Incident Response Personnel**

Required of all personnel on the incident response team, including on-call personnel, before being added to the incident response rota.

- Incident response lifecycle: identification, classification, containment, eradication, recovery, post-incident review
- Incident classification framework and severity determination with worked scenarios
- Evidence preservation and chain of custody for digital forensics
- Regulatory notification obligations: GDPR breach notification (72-hour window), EU AI Act Article 73 serious incident reporting, national authority notification procedures
- Stakeholder communication during incidents: internal escalation, executive notification, customer communication, media protocol
- AI and model-specific incident failure modes: how to recognise and classify a model failure, data poisoning attack, adversarial input exploitation, and LLM-specific incidents (hallucination at scale, prompt injection in production)
- Post-incident review facilitation: root cause analysis methodology, finding classification, corrective action development

Annual refresher training is required. Tabletop exercise participation is required **semi-annually**, with attendance records maintained by the Information Security Team.

**F.5.2 Privileged Access Holders**

Required of all personnel with administrator-level, root, or equivalent privileged access before provisioning of elevated credentials.

- Privileged access risks and the threat model for credential compromise and insider misuse
- Just-in-time and just-enough-access principles and how they apply to Emyzer Nexus privileged access management
- Privileged session recording and monitoring: what is logged, how to operate transparently within monitored sessions, and what triggers an alert
- Secrets management: how to handle API keys, certificates, and service account credentials
- Privileged access in cloud environments: IAM role assumption, service account governance, and cross-account access controls
- Reporting and escalation: what to do if privileged credentials are suspected of compromise

Annual refresher training required.

**F.5.3 Data Protection Officer and Privacy Team**

Required of the DPO and all personnel in the Privacy function.

- GDPR and UK GDPR obligations in depth: lawful basis, data subject rights, data protection by design and by default, records of processing activities
- Data Protection Impact Assessment (DPIA) methodology, including when a DPIA is mandatory, how to conduct one, and how to document findings and decisions
- AI-specific privacy obligations: the intersection of EU AI Act High-Risk system requirements and GDPR DPIA obligations for AI systems processing personal data
- Cross-border data transfer mechanisms: standard contractual clauses, adequacy decisions, and transfer impact assessments
- Regulatory engagement: how to interact with data protection authorities, manage investigations, and handle enforcement correspondence
- Breach notification: internal escalation, GDPR 72-hour notification obligation, affected individual notification requirements

Annual refresher training required, with update training triggered by material regulatory developments.

---

## G. Completion Requirements and Non-Completion Escalation

### G.1 Training Deadlines Summary

| Training Track | Population | Initial Deadline | Recurrence |
|----------------|-----------|-----------------|------------|
| General Awareness | All personnel | 30 days from start date | Annual |
| AI and Responsible Technology | Assigned personnel | 60 days from assignment | Annual |
| Role-Based (all tracks except F.4.9 and F.4.10) | Assigned by function | 60 days from role assignment | Annual; on material change |
| Role-Based — AI System Operators (F.4.9) | High-Risk AI system operators | Before access provisioning | On material change |
| Role-Based — Model Users (F.4.10) | Tier 1 and Tier 2 model users | Before access provisioning | On material change |
| Specialist — Incident Response | IR team and on-call personnel | Before rota addition | Annual; semi-annual tabletop |
| Specialist — Privileged Access | Privileged access holders | Before access provisioning | Annual |
| Specialist — Data Protection | DPO and Privacy team | Before role commencement | Annual; on regulatory change |

### G.2 Knowledge Assessment Standards

All training modules that include knowledge assessments shall apply a **passing threshold of 80%**. Personnel who fail on first attempt shall be permitted one re-attempt within **5 business days**. Personnel who fail the re-attempt shall be automatically assigned remedial training by the LMS and their line manager notified. Remedial training shall be completed within **10 business days** of assignment. Failure to complete remedial training within 10 business days triggers the non-completion escalation process.

### G.3 Non-Completion Escalation Process

Training is an operational requirement. Non-completion has defined consequences, escalating on a structured timeline.

| Day | Action | Responsible Party |
|-----|--------|-------------------|
| Deadline date | Automated LMS alert to individual and line manager | LMS (automated) |
| Deadline + 5 | Line manager confirms follow-up with individual | Line Manager |
| Deadline + 10 | GRC Team non-completion report issued to HR and CISO | GRC Team |
| Deadline + 15 | HR formal non-completion notification to individual and line manager | Human Resources |
| Deadline + 20 | CISO review of persistent non-completions; determination of access action | CISO |
| Deadline + 21 | System access suspended for General Awareness and Annual Role-Based non-completions pending completion. Access provisioning blocked for prerequisite training non-completions. | Information Security Team |
| Deadline + 30 | HR initiates formal performance management process | Human Resources |

Access suspension shall be lifted within **24 hours** of training completion confirmed in the LMS. The CISO may grant a 5-business-day extension to the access suspension threshold where the individual has a documented operational dependency and is actively completing the training. Extensions shall be recorded in the GRC platform exceptions log.

### G.4 Phishing Simulation Program

The Information Security Team shall conduct phishing simulations across all in-scope personnel **at least quarterly**. Simulations shall:

- Vary in sophistication across the calendar year — ranging from general phishing indicators to spear-phishing scenarios personalised to role and organisational context
- Include at least one AI-enhanced phishing scenario annually, reflecting the current use of LLM tools in sophisticated phishing campaigns
- Be randomised in timing within each quarter to prevent habituation
- Measure click rate, credential submission rate, and report rate as primary metrics

**Individual outcomes:**
- Personnel who click a simulated phishing link shall receive immediate in-browser awareness reinforcement and be assigned targeted remedial phishing training within **24 hours** of the simulation event.
- Personnel who submit credentials in a simulation shall be treated as a high-priority remediation case, with line manager notification and mandatory 1:1 security coaching scheduled within **5 business days**.
- Personnel who correctly report a simulation to the Information Security Team shall be acknowledged positively — the programme measures reporting culture, not just susceptibility.

**Programme-level outcomes:**
- Quarterly phishing simulation results shall be reported to the CISO and included in the training effectiveness assessment.
- Department-level results shall be shared with relevant line managers to enable targeted team-level awareness interventions.
- Simulation methodology and scenarios shall be reviewed **annually** to ensure they reflect current phishing techniques, including AI-generated content and deepfake-based social engineering.

---

## H. Veridian AI Integration — Transition Requirements

Personnel acquired through the Veridian AI integration shall complete all applicable onboarding training obligations within **60 days** of being granted access to Emyzer Nexus information systems. The following applies specifically to integration personnel:

- **General Awareness Track:** Within 60 days of system access grant (standard deadline is 30 days for new hires; the extended deadline reflects the integration context and volume of personnel to be onboarded).
- **AI and Responsible Technology Track:** Within 60 days of system access grant. Given that Veridian AI personnel worked directly with AI systems, this track is priority-assigned.
- **Integration Supplement Module:** A dedicated module covering the differences between Veridian AI's previous practices and Emyzer Nexus governance standards, including: data classification requirements, AI governance obligations, acceptable use standards, and incident reporting procedures. Required within **30 days** of system access grant. Developed by the Information Security Team in consultation with the GRC Team before integration go-live.
- **Role-Based and Specialist Training:** Assigned based on post-integration roles and completed within the standard deadlines for each track.

The GRC Team shall maintain a dedicated Veridian AI integration training register and report completion status to the CISO **monthly** for the first six months post-integration.

---

## I. Curriculum Governance

### I.1 Annual Curriculum Review

The Information Security Team shall conduct a full curriculum review **annually**, covering:

- Relevance of current content to the threat landscape — including emerging phishing techniques, AI-specific threats, and regulatory developments
- Lessons learned from security incidents in the past 12 months, identifying content gaps that contributed to incident occurrence or impact
- Changes to applicable regulations, standards, or internal policies that require curriculum updates
- Training effectiveness assessment findings identifying knowledge gaps or behavioural outcomes not achieved
- Benchmark comparison with industry training standards and peer programmes where available

Curriculum review findings shall be submitted to the CISO for approval. Material curriculum changes require CISO approval and trigger re-completion obligations. Editorial updates (corrections, formatting, minor clarifications) do not require re-completion.

### I.2 Out-of-Cycle Curriculum Updates

The CISO may authorise out-of-cycle curriculum updates in response to:

- A significant security incident in which a training gap contributed to occurrence or impact
- A material regulatory change requiring immediate workforce communication
- An emerging threat that poses significant risk and is not addressed in current content
- A significant change to organisational AI systems or governance obligations

Out-of-cycle updates classified as material curriculum changes by the CISO shall trigger re-completion obligations communicated with a defined deadline, typically **30 days** from update publication.

### I.3 Curriculum Version Control

All training modules shall be version-controlled with a document history recording the author of changes, change description, classification (material or editorial), approval date, and re-completion requirement. Version history shall be retained in the document repository for 5 years.

---

## J. Training Effectiveness Assessment

Completion rates are necessary but insufficient evidence of program effectiveness. The GRC Team shall conduct an annual training effectiveness assessment covering:

**J.1 Quantitative Metrics**
- General Awareness completion rate by business unit and employment type
- Role-Based completion rate by track
- Knowledge assessment pass rates by module (first attempt and overall)
- Phishing simulation click rate trend (quarterly over the past 12 months)
- Phishing simulation report rate trend
- Remedial training completion rate
- Proportion of security incidents in which root cause analysis identified an awareness or training gap

**J.2 Qualitative Assessment**
- Review of security incident root cause analyses from the past 12 months to identify patterns attributable to awareness or training gaps
- Line manager survey on perceived training relevance and team security behaviour
- Sample review of knowledge assessment responses to assess quality of understanding, not just pass/fail outcomes
- Assessment of whether training content reflects current threat scenarios or requires modernisation

**J.3 Reporting and Action**
The training effectiveness assessment shall be submitted to the CISO and presented to the Security Steering Committee **annually**, accompanied by:
- A summary of findings against each metric
- An assessment of whether the programme achieved its behaviour change objectives in the past year
- Recommended curriculum changes for the coming year
- Proposed metrics targets for the coming year

---

## K. Compliance and Monitoring

### K.1 Monitoring Activities

| Activity | Frequency | Owner |
|----------|-----------|-------|
| LMS completion dashboard review | Weekly | GRC Team |
| Non-completion report to CISO and HR | Monthly | GRC Team |
| Phishing simulation execution | Quarterly | Information Security Team |
| Phishing simulation results report | Quarterly | Information Security Team |
| Training compliance posture to executive leadership | Quarterly | CISO |
| Veridian AI integration training register review | Monthly (first 6 months post-integration) | GRC Team |
| Curriculum review | Annual | Information Security Team |
| Training effectiveness assessment | Annual | GRC Team |
| Policy compliance audit (part of ISMS audit) | Annual | Internal Audit |

### K.2 Key Performance Indicators

| KPI | Target | Measurement Frequency |
|-----|--------|----------------------|
| General Awareness completion within deadline | ≥95% | Monthly |
| General Awareness annual completion rate (all personnel) | 100% | Quarterly |
| Role-Based training completion within deadline | ≥90% | Monthly |
| Specialist training completion before access provisioning | 100% | Per provisioning event |
| Knowledge assessment first-attempt pass rate | ≥85% | Quarterly |
| Remedial training completion within 10 business days | 100% | Monthly |
| Phishing simulation click rate (annual trend) | Year-on-year reduction | Quarterly |
| Phishing simulation report rate | ≥30% and increasing | Quarterly |
| Phishing simulation credential submission rate | <5% | Quarterly |
| Security incidents with training gap as contributing factor | Year-on-year reduction | Annual |
| Veridian AI integration training completion within 60 days | 100% | Monthly (first 6 months) |
| Open training-related exceptions | ≤5 at any time | Quarterly |

### K.3 Non-Compliance

Personnel who do not complete mandatory training within the escalation timeline defined in Section G shall have system access suspended. Persistent non-compliance shall be addressed through the HR performance management process. Line managers who do not escalate persistent non-completion within their teams within the required timeframe shall be subject to the same performance management process as the non-completing individual. The CISO shall report systemic non-compliance (business unit completion rates below 80% for 30 or more days beyond deadline) to the CEO.

---

## L. Policy Exceptions

### L.1 Exception Process

Personnel requiring a temporary extension to training completion deadlines shall:

1. Submit an exception request via **ServiceNow GRC workflow** with documented business justification (e.g., medical leave, extended travel, operational emergency).
2. Obtain line manager endorsement and CISO approval. Exceptions affecting prerequisite training (AI System Operator, Model User, Incident Response, Privileged Access) require CISO approval and shall not delay access suspension where access has already been provisioned.
3. Accept a maximum extension of **90 days** from the original deadline. No exception shall exempt an individual from completion — only extend the deadline.
4. Exceptions shall not be granted for personnel who have previously exceeded the escalation timeline without a documented exceptional circumstance.

### L.2 Exception Governance

- All active exceptions reviewed **quarterly** by the GRC Team and CISO.
- Exception register maintained in the GRC platform with monthly status updates.
- No exception shall remain open beyond 90 days without a renewed application and re-approved business justification.

---

## M. Related Policies

1. [**Information Security Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/information-security-policy.md) *(KB-PORTFOLIO-0001)* — Parent policy. Establishes the ISMS framework and baseline security obligations from which training requirements derive.

2. [**AI Governance Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/ai-governance-policy.md) *(KB-PORTFOLIO-0011)* — Establishes AI awareness training obligations (within 30 days of hire; annually) and High-Risk AI system operator training requirements (before access provisioning) now consolidated under this policy.

3. [**Model Risk Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/model-risk-policy.md) *(KB-PORTFOLIO-0012)* — Establishes Tier 1 and Tier 2 model user training requirements (before access provisioning) and model-specific limitation disclosure obligations now consolidated under this policy.

4. [**Acceptable Use Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/acceptable-use-policy.md) *(KB-PORTFOLIO-0004)* — Governs system and AI tool use obligations covered in the General Awareness Track.

5. [**Access Control Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/access-control-policy.md) *(KB-PORTFOLIO-0005)* — Governs privileged access provisioning requirements; Specialist Track F.5.2 is a prerequisite for elevated access under this policy.

6. [**Incident Management Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/incident-management-policy.md) *(KB-PORTFOLIO-0006)* — Governs incident response; Specialist Track F.5.1 is a prerequisite for incident response rota membership under this policy.

7. [**Third-Party Risk Management Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/third-party-risk-management-policy.md) *(KB-PORTFOLIO-0008)* — Governs vendor risk obligations covered in Role-Based Track F.4.8.

8. [**Privacy and Data Protection Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/privacy-data-protection-policy.md) *(KB-PORTFOLIO-0013)* — Governs GDPR and privacy obligations covered in the General Awareness Track and Specialist Track F.5.3. *(In Development)*

---

## N. Related Documents

1. Training Curriculum — General Awareness Track (Version-Controlled)
2. Training Curriculum — AI and Responsible Technology Track (Version-Controlled)
3. Role-Based Training Curricula by Function (Version-Controlled)
4. Specialist Training Curricula — Incident Response, Privileged Access, Data Protection (Version-Controlled)
5. AI System Operator Training Curricula (System-Specific, maintained by AI System Owners)
6. Model User Training Curricula (Model-Specific, maintained by Model Owners)
7. Phishing Simulation Program — Annual Schedule and Methodology
8. Training Effectiveness Assessment Template
9. Training Non-Completion Escalation Procedure
10. Veridian AI Integration Training Register
11. Curriculum Review Checklist
12. Training Exception Request Form (ServiceNow)

---

## O. Review and Revision

This policy shall be reviewed **annually** or upon: a significant security incident in which an awareness or training gap contributed to occurrence or impact; material changes to applicable regulations or standards (including EU AI Act implementing acts and GDPR guidance); significant changes to the organisation's AI system portfolio that alter operator or user training obligations; or changes to subordinate policies that affect consolidated training requirements. All revisions require CEO approval. Changes that alter completion deadlines, escalation thresholds, or prerequisite training requirements shall be communicated to Human Resources, all line managers, and the GRC Team **within 10 business days** of approval.

---

## P. Framework Alignment

| Framework | Alignment |
|-----------|-----------|
| **NIST SP 800-50 Rev. 1** | Section 2 (Building a Learning Programme — needs assessment, curriculum design, delivery), Section 3 (Programme Management — metrics, effectiveness measurement, continuous improvement), Section 4 (Role-Based Training — functional role identification and curriculum differentiation) |
| **NIST SP 800-16 Rev. 1** | Role-based cybersecurity training framework — functional speciality identification, knowledge, skill, and ability mapping for IT/Security, GRC, Developer, and Executive tracks |
| **ISO/IEC 27001:2022** | A.6.3 (Information security awareness, education, and training — mandatory awareness for all personnel), A.7.2 (Information security terms and conditions — training obligations for personnel with specific responsibilities), Clause 7.2 (Competence requirements for personnel affecting information security performance) |
| **ISO/IEC 27002:2022** | Control 6.3 (Information security awareness, education, and training — implementation guidance for programme design, content, and effectiveness measurement), Control 7.2 (Managing human resources security — training as part of security obligations during employment) |
| **NIST CSF 2.0** | GV.RR (Roles, responsibilities, and authorities — training to support role clarity and accountability), PR.AT (Awareness and Training — Programme design, delivery, and effectiveness measurement for all personnel and privileged users) |
| **EU AI Act (Regulation 2024/1689)** | Article 14(4) (Measures for human oversight — training of operators to use High-Risk AI systems correctly), Article 26(6) (Deployer obligations — ensuring operators have necessary competence and training before High-Risk AI system use) |
| **GDPR (Regulation 2016/679)** | Article 39(1)(b) (DPO duties — monitoring compliance including awareness raising and training of personnel involved in processing operations), Article 5(1)(f) (Integrity and confidentiality principle — training as an organisational measure supporting secure processing) |

---

## Q. Organisational Benefit

| Benefit Area | Description |
|--------------|-------------|
| **Risk Reduction** | A structured, role-differentiated training programme with measurable completion requirements and phishing simulation reduces the likelihood of human-vector security incidents — the most common cause of data breaches across all industries |
| **Regulatory Compliance** | Meets ISO 27001:2022 Annex A training obligations, EU AI Act operator training requirements (Article 14/26), GDPR DPO training obligations, and NIST SP 800-50 programme standards in a single consolidated framework |
| **Acquisition Integration** | The Veridian AI integration supplement and 60-day extended onboarding deadline provide a structured mechanism for bringing acquired personnel to Emyzer Nexus security standards without disrupting integration timelines |
| **AI Governance Operationalisation** | Prerequisite training for High-Risk AI system operators and Tier 1/2 model users converts governance paper requirements into operational reality — no operator can access a governed system without documented training completion |
| **Policy Consolidation** | Consolidating training obligations from six policies into one governance document eliminates the risk of gaps arising from obligations existing in documents personnel do not routinely read, and gives Human Resources a single source of truth for compliance tracking |
| **Behaviour Change Focus** | Annual effectiveness assessments, phishing simulation metrics, and incident root cause analysis create accountability for behaviour change outcomes — not just completion rates — aligning the programme with its actual purpose |
| **Audit Readiness** | Comprehensive completion records with defined retention periods, version-controlled curriculum documentation, and structured effectiveness reporting provide the evidence base required by ISO 27001 auditors, regulatory inspectors, and client due diligence reviewers |
| **Cultural Foundation** | Positive phishing simulation reporting acknowledgement, executive leadership training visibility, and line manager accountability create the conditions for a genuine security culture rather than a compliance-driven one |

---

## R. Evidence of Compliance

| Evidence Type | System of Record | Owner | Retention Period |
|---------------|------------------|-------|------------------|
| Training completion records (all tracks) | Learning Management System | Human Resources | Employment duration + 3 years |
| Knowledge assessment results | Learning Management System | Human Resources | Employment duration + 3 years |
| Remedial training assignment and completion records | Learning Management System | Human Resources | Employment duration + 3 years |
| Phishing simulation execution records | Information Security Team repository | Information Security Team | 3 years |
| Phishing simulation results (programme-level) | GRC Platform | GRC Team | 3 years |
| Phishing simulation results (individual-level) | Learning Management System | Human Resources | Employment duration + 3 years |
| Non-completion escalation records | GRC Platform / HR system | Human Resources | Employment duration + 3 years |
| Access suspension records (training-related) | ServiceNow ITSM | Information Security Team | 5 years |
| Training curriculum — version history | Document Repository | Information Security Team | 5 years from version retirement |
| Curriculum review records | Document Repository | Information Security Team | 5 years |
| Training effectiveness assessments | GRC Platform | GRC Team | 5 years |
| Security Steering Committee training reports | Document Repository | CISO | 7 years |
| Policy exception records | GRC Platform | GRC Team / CISO | Exception duration + 3 years |
| Veridian AI integration training register | GRC Platform | GRC Team | 5 years from integration completion |
| AI System Operator training records (system-specific) | Learning Management System | Human Resources | Employment duration + 3 years |
| Model User training records (model-specific) | Learning Management System | Human Resources | Employment duration + 3 years |
| Tabletop exercise attendance records | Information Security Team repository | Information Security Team | 3 years |
| Policy acknowledgement records | GRC Platform / HR system | Human Resources | Employment duration + 3 years |
| Annual compliance audit reports | GRC Platform | Internal Audit | 7 years |

---

## Approval History

| Date | Approver | Status | Comments |
|------|----------|--------|----------|
| 2025-11-01 | Chief Executive Officer | Approved | "Consolidating training obligations across six policies into one document with a unified escalation process and effectiveness assessment is the right governance decision. The prerequisite model for AI operator and model user access is particularly important given our current AI governance programme. The Veridian AI integration provisions are appropriately structured. Approved." |

---

## Document Control

- **Document ID:** KB-PORTFOLIO-0014
- **Version:** 1.0
- **Classification:** Internal
- **Last Updated:** 2025-11-01
- **Next Review Date:** 2026-11-01

---

*This policy document was developed as part of the Emyzer Nexus Phase 2 GRC programme and formatted for portfolio presentation. It consolidates training obligations previously distributed across KB-PORTFOLIO-0001, KB-PORTFOLIO-0004, KB-PORTFOLIO-0005, KB-PORTFOLIO-0006, KB-PORTFOLIO-0008, KB-PORTFOLIO-0011, and KB-PORTFOLIO-0012.*

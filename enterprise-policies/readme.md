# Enterprise Policies

**Emyzer Nexus – Governance, Risk, and Compliance Portfolio**

---

> **For recruiters and hiring managers:** The [60-Second Review Path](#60-second-review-path) below is designed for you. It surfaces the highest-signal artifacts first and tells you exactly what each one demonstrates.

---

## What This Is

This directory contains the enterprise policy framework developed for Emyzer Nexus, a fictional mid-market SaaS company navigating a period of rapid governance maturity: including the integration of Veridian AI, an acquired ML startup, and growing exposure to EU regulatory obligations.

The policies here are not templates. Each one is written for a specific organisational scenario, with role-specific accountability structures, calibrated controls, evidence retention schedules, ServiceNow workflow references, and cross-policy dependencies that reflect how enterprise GRC programs actually operate. The scenario grounds every policy decision in a business context that a recruiter or practitioner can evaluate.

**My background informing this work:** GRC program design, policy architecture, EU AI Act and ISO 27001 compliance, risk register management, and enterprise technical writing. I write about GRC practice at [cleanlikesoapblog.wordpress.com/category/grc](https://cleanlikesoapblog.wordpress.com/category/grc/): including the judgment calls, trade-offs, and real-world constraints that don't make it into policy documents.

---

## The Scenario

**Organisation:** Emyzer Nexus: a mid-market B2B SaaS company with operations across the EU and UK, serving clients in regulated industries including financial services, healthcare, and professional services.

**Subsidiary:** Emyzer Technology: the internal development arm.

**Acquisition:** Veridian AI: an ML startup acquired in 2024, bringing two High-Risk AI systems (under EU AI Act classification) into the Emyzer Nexus environment without existing governance documentation meeting enterprise standards:

| Inherited System | EU AI Act Classification | Governance Status at Acquisition |
|-----------------|--------------------------|----------------------------------|
| Predictive Customer Churn Model | High-Risk | Undocumented; no independent validation on record |
| AI-Assisted Contract Review Tool | High-Risk | Partial documentation; validation incomplete |

This acquisition scenario drives the most consequential policy decisions in the framework, particularly around AI governance, model risk, third-party risk, and incident management, and is the thread that connects Phase 1 and Phase 2 of the portfolio.

---

## 60-Second Review Path

If you have one minute, read in this order:

| Step | Document | What It Demonstrates |
|------|----------|----------------------|
| 1 | [AI Governance Policy](#ai-governance-policy) | EU AI Act mapping, NIST AI RMF alignment, acquisition risk, human oversight design |
| 2 | [Model Risk Policy](#model-risk-policy) | SR 11-7 fluency, independent validation frameworks, tiered governance, Veridian AI remediation |
| 3 | [Risk Management Policy](#risk-management-policy) | Enterprise risk methodology, risk appetite integration, cross-policy risk register ownership |
| 4 | Evidence Index in any Tier 1 policy | How I think about compliance proof, retention periods, and audit readiness |

If you have five minutes, add the [Third-Party Risk Management Policy](#third-party-risk-management-policy) and the cross-reference map in [Policy Architecture](#policy-architecture).

---

## Policy Index

### Phase 1: Foundation Policies

| Policy | Doc ID | Owner | Status | Frameworks |
|--------|--------|-------|--------|------------|
| [Information Security Policy](#information-security-policy) | KB-PORTFOLIO-0001 | CISO | Published | ISO 27001:2022, NIST CSF 2.0 |
| [Risk Management Policy](#risk-management-policy) | KB-PORTFOLIO-0002 | CRO | Published | ISO 31000:2018, NIST CSF 2.0 |
| [Data Classification Policy](#data-classification-policy) | KB-PORTFOLIO-0003 | CISO | Published | ISO 27001:2022, GDPR |
| [Acceptable Use Policy](#acceptable-use-policy) | KB-PORTFOLIO-0004 | CISO | Published | ISO 27001:2022 |
| [Access Control Policy](#access-control-policy) | KB-PORTFOLIO-0005 | CISO | Published | ISO 27001:2022, NIST SP 800-53 Rev. 5 |
| [Incident Management Policy](#incident-management-policy) | KB-PORTFOLIO-0006 | CISO | Published | ISO 27035:2023, NIST SP 800-61 Rev. 2 |
| [Business Continuity Policy](#business-continuity-policy) | KB-PORTFOLIO-0007 | CRO | Published | ISO 22301:2019, NIST SP 800-34 |
| [Third-Party Risk Management Policy](#third-party-risk-management-policy) | KB-PORTFOLIO-0008 | CRO | Published | ISO 27001:2022, NIST CSF 2.0 |
| [Change Management Policy](#change-management-policy) | KB-PORTFOLIO-0009 | CTO | Published | ITIL 4, ISO 27001:2022 |
| [Vulnerability Management Policy](#vulnerability-management-policy) | KB-PORTFOLIO-0010 | CISO | Published | NIST SP 800-40 Rev. 4, CIS Controls v8 |

### Phase 2: AI and Advanced Risk Policies

| Policy | Doc ID | Owner | Status | Frameworks |
|--------|--------|-------|--------|------------|
| [AI Governance Policy](#ai-governance-policy) | KB-PORTFOLIO-0011 | CISO | Published | EU AI Act, NIST AI RMF 1.0, ISO/IEC 42001:2023 |
| [Model Risk Policy](#model-risk-policy) | KB-PORTFOLIO-0012 | CRO | Published | SR 11-7, NIST AI RMF 1.0, EU AI Act |
| [Privacy and Data Protection Policy](#privacy-and-data-protection-policy) | KB-PORTFOLIO-0013 | DPO | Published | GDPR, UK GDPR, ISO 27701:2019 |
| [Security Awareness and Training Policy](#security-awareness-and-training-policy) | KB-PORTFOLIO-0014 | CISO | Published | ISO 27001:2022, NIST SP 800-50 |

---

## Policy Architecture

Every policy in this framework has a deliberate position in the hierarchy. Understanding the structure is more useful to a practitioner than reading each document in isolation.

```
Information Security Policy (KB-PORTFOLIO-0001)
│   The ISMS parent. All security and risk policies derive authority from here.
│
├── Risk Management Policy (KB-PORTFOLIO-0002)
│   │   Owns the enterprise risk register. Defines risk appetite and
│   │   treatment methodology used by all subordinate policies.
│   │
│   ├── Third-Party Risk Management Policy (KB-PORTFOLIO-0008)
│   │       Governs vendor risk lifecycle. Extended by the AI Vendor Risk
│   │       Due Diligence Addendum for AI-specific procurement obligations.
│   │
│   └── Business Continuity Policy (KB-PORTFOLIO-0007)
│           Aligns recovery objectives with risk appetite thresholds
│           defined in the Risk Management Policy.
│
├── Data Classification Policy (KB-PORTFOLIO-0003)
│       Governs data handling across all policies. Training data, model
│       artefacts, and AI outputs reference classification tiers defined here.
│
├── Access Control Policy (KB-PORTFOLIO-0005)
│       Governs identity and access controls referenced across incident,
│       change, and AI governance policies.
│
├── Incident Management Policy (KB-PORTFOLIO-0006)
│       Defines the base incident response process. AI and model incidents
│       extend this policy with domain-specific failure modes and regulatory
│       notification obligations.
│
├── AI Governance Policy (KB-PORTFOLIO-0011)
│   │   Strategic governance for all AI and ML systems. Operationalises
│   │   EU AI Act obligations. Parent to the Model Risk Policy for AI/ML
│   │   systems that also meet the model definition.
│   │
│   └── Model Risk Policy (KB-PORTFOLIO-0012)
│           Operational model lifecycle controls. Applies to all quantitative
│           and AI/ML models. Subordinate to AI Governance Policy for AI/ML
│           systems; independent authority for non-AI models. Aligns to SR 11-7.
│
├── Change Management Policy (KB-PORTFOLIO-0009)
│       Governs change controls referenced in model deployment and AI system
│       material change processes.
│
└── Vulnerability Management Policy (KB-PORTFOLIO-0010)
        Governs technical vulnerability controls referenced in AI system
        security and model artefact integrity requirements.
```

**Why this matters:** A common gap in portfolio GRC work is policies that exist as isolated documents. In practice, a Tier 1 AI model touches the AI Governance Policy (strategic), Model Risk Policy (operational lifecycle), Third-Party Risk Management Policy (if vendor-sourced), Data Classification Policy (training data), Incident Management Policy (model failure response), and Change Management Policy (material change controls) simultaneously. Every cross-policy reference in this framework is intentional and traceable.

---

## Policy Summaries

### Information Security Policy

**KB-PORTFOLIO-0001 | Owner: CISO | Parent: None**

The ISMS parent policy. Establishes the governance structure, roles, and baseline security obligations from which all subordinate policies derive authority. Defines the scope of the ISMS, the Emyzer Nexus security governance bodies (Security Steering Committee, CISO function), and the annual review and exception governance processes applied consistently across the framework.

**Key design decisions:**
- Scope explicitly includes Emyzer Technology (subsidiary) and acquired entities: a deliberate choice that forces governance obligations to travel with the acquisition from day one.
- Exception governance uses a ServiceNow GRC workflow with CISO approval authority, establishing the pattern used by all subordinate policies.
- Alignment to ISO 27001:2022 Annex A controls mapped in the Statement of Applicability, referenced throughout the framework.

---

### Risk Management Policy

**KB-PORTFOLIO-0002 | Owner: CRO | Parent: Information Security Policy**

Defines the enterprise risk assessment methodology, risk appetite statement, risk treatment options, and risk register governance. The policy establishes the CRO as enterprise risk register owner and the mechanism by which AI risk, model risk, third-party risk, and operational risk feed a unified risk picture reported to the board.

**Key design decisions:**
- Risk appetite is expressed in quantitative and qualitative terms for each risk category, providing the thresholds that Model Risk Policy monitoring escalation triggers reference.
- Treatment methodology follows ISO 31000:2018, avoid, reduce, share, accept, with formal risk acceptance requiring CRO sign-off above defined materiality thresholds.
- The policy explicitly establishes AI-specific risk categories (model drift, training data bias, third-party model dependency) as distinct entries in the enterprise risk register, not subsets of operational risk.

---

### Data Classification Policy

**KB-PORTFOLIO-0003 | Owner: CISO | Parent: Information Security Policy**

Establishes the four-tier data classification framework (Public, Internal, Confidential, Restricted) applied across all data handling, storage, and transmission. Every AI and model policy references this classification scheme for training data governance, model artefact protection, output handling, and retention compliance.

**Key design decisions:**
- Training datasets and model artefacts are classified at minimum as Confidential, with High-Risk AI system data classified as Restricted.
- Retention schedules referenced in the AI Governance Policy and Model Risk Policy evidence indexes are anchored to this policy's disposition framework.
- The policy includes a data handling matrix covering cloud storage, email, endpoint, and API transmission: directly relevant to how LLM API outputs are governed.

---

### Acceptable Use Policy

**KB-PORTFOLIO-0004 | Owner: CISO | Parent: Information Security Policy**

Governs employee and contractor use of Emyzer Nexus information systems, including AI tools, personal devices, and cloud services. Includes specific provisions governing the use of third-party generative AI tools with organisational data: a gap in most acceptable use policies that predates widespread AI adoption.

**Key design decisions:**
- Generative AI use provisions prohibit inputting Confidential or Restricted data into external LLM APIs without AI Governance Committee-approved data handling controls in place.
- Shadow AI reporting obligations align with the AI Governance Policy's annual inventory audit requirements: employees discovering undisclosed AI use are required to report through the same channels as other compliance concerns.

---

### Access Control Policy

**KB-PORTFOLIO-0005 | Owner: CISO | Parent: Information Security Policy**

Defines identity and access management requirements across Emyzer Nexus systems, including role-based access control, privileged access management, and access review cadences. Referenced by the AI Governance Policy and Model Risk Policy for model operator access provisioning and training completion prerequisites.

**Key design decisions:**
- Privileged access to model training environments and AI system configuration is classified as high-privilege access subject to quarterly review: tighter than the standard annual review cycle.
- Access deprovisioning is tied to model retirement procedures: model operator access shall be removed within 5 business days of model retirement completion.

---

### Incident Management Policy

**KB-PORTFOLIO-0006 | Owner: CISO | Parent: Information Security Policy**

Establishes the incident response lifecycle, identification, classification, containment, eradication, recovery, and post-incident review, with severity classification framework and escalation paths. Extended by the AI Governance Policy (AI-specific failure modes and EU AI Act Article 73 regulatory notification) and Model Risk Policy (model-specific failure mode classification).

**Key design decisions:**
- The AI and model incident extensions are not separate documents: they are explicit extensions to this policy, ensuring AI incidents flow through the same ITSM tooling (ServiceNow) and post-incident review process as all other incidents.
- Regulatory notification obligations under EU AI Act Article 73 are embedded in the High/Critical severity path, with Legal Counsel notification triggered automatically at that classification.
- Post-incident review templates include model-specific root cause categories (conceptual error, data quality failure, out-of-scope use, monitoring failure, operator error) alongside standard incident root cause taxonomy.

---

### Business Continuity Policy

**KB-PORTFOLIO-0007 | Owner: CRO | Parent: Information Security Policy**

Governs business continuity and disaster recovery planning across Emyzer Nexus, including Recovery Time Objectives and Recovery Point Objectives calibrated to the organisation's risk appetite. Includes AI system continuity provisions covering model availability, fallback decision processes for AI system outages, and third-party AI API dependency management.

**Key design decisions:**
- AI system availability is treated as a distinct continuity risk, not subsumed into general IT continuity, because the failure modes differ (model degradation vs. system unavailability) and the fallback processes require human decision-making guidance rather than just IT failover.
- The Predictive Customer Churn Model and AI-Assisted Contract Review Tool each have documented fallback procedures defining how affected business processes operate during model unavailability.

---

### Third-Party Risk Management Policy

**KB-PORTFOLIO-0008 | Owner: CRO | Parent: Information Security Policy**

Governs the end-to-end vendor risk lifecycle including due diligence, contract requirements, ongoing monitoring, and offboarding. Extended by the AI Vendor Risk Due Diligence Addendum, which adds AI-specific assessment criteria for vendors supplying AI systems or model APIs.

**Key design decisions:**
- The AI Vendor Risk Due Diligence Addendum is a subordinate document rather than an amendment to this policy: designed to be updated independently as EU AI Act implementing acts develop without requiring full policy revision.
- Third-party AI API vendors (LLM providers) are subject to enhanced due diligence covering training data transparency, model versioning disclosure, API output variability documentation, and incident notification SLAs: requirements not present in standard vendor assessment frameworks.
- Contractual requirements include the right to audit model documentation and the right to terminate if the vendor fails to maintain EU AI Act compliance: tested against the Veridian AI acquisition scenario to ensure they work in a post-acquisition context.

---

### Change Management Policy

**KB-PORTFOLIO-0009 | Owner: CTO | Parent: Information Security Policy**

Defines the change management lifecycle for technology, process, and configuration changes across Emyzer Nexus. Includes AI system change provisions classifying model material changes as requiring change management review before implementation: the control point that prevents undocumented model modifications from bypassing the revalidation process.

**Key design decisions:**
- Material change to an AI or ML model is defined consistently with the AI Governance Policy and Model Risk Policy definitions: the same definition governs both change management review requirements and revalidation triggers.
- Emergency change provisions include AI-specific guidance for rapid model suspension decisions, acknowledging that the risk of delay (continued model operation) may outweigh the risk of bypassing standard change controls in a confirmed incident.

---

### Vulnerability Management Policy

**KB-PORTFOLIO-0010 | Owner: CISO | Parent: Information Security Policy**

Governs the identification, assessment, prioritisation, and remediation of technical vulnerabilities across Emyzer Nexus infrastructure, applications, and AI systems. Includes model security provisions covering training data integrity, model artefact protection, and adversarial input testing.

**Key design decisions:**
- AI-specific vulnerability categories (adversarial inputs, prompt injection for LLM integrations, model inversion attacks, training data poisoning) are explicitly in scope: not treated as edge cases.
- Adversarial input testing cadence for High-Risk AI systems aligns with the EU AI Act Article 15 (Accuracy, Robustness, Cybersecurity) requirements referenced in the AI Governance Policy conformity assessment framework.

---

### AI Governance Policy

**KB-PORTFOLIO-0011 | Owner: CISO | Parent: Information Security Policy | 

The strategic governance framework for all AI and machine learning systems across Emyzer Nexus. Establishes EU AI Act risk classification obligations, conformity assessment requirements for High-Risk systems, human oversight design standards, post-market monitoring cadences, and prohibited AI practices. The most technically complex policy in the framework.

**Key design decisions:**
- The AI Governance Committee is a named governance body with defined cross-functional membership, quarterly cadence, and emergency convening obligations: not a vague "stakeholder group."
- Human oversight requirements are written to EU AI Act Article 14 standards: operators must be able to understand, monitor, intervene in, and halt AI system outputs. These are testable obligations, not principles.
- Third-party LLM API opacity is treated as a documented limitation requiring compensating controls, not ignored. Where full algorithmic explainability is not feasible, the policy requires disclosure, human review of outputs, and committee-level acknowledgement.
- The Veridian AI acquisition is woven through the scope, the systems-in-scope table, and the evidence requirements: demonstrating governance under realistic conditions, not ideal ones.

**Frameworks:** EU AI Act (Regulation 2024/1689): Articles 9, 10, 11, 13, 14, 15, 72, 73; NIST AI RMF 1.0 (Govern, Map, Measure, Manage); ISO/IEC 42001:2023; ISO/IEC 27001:2022; ISO/IEC 23894:2023; NIST SP 800-53 Rev. 5

👉 [Read the AI Governance Policy](./ai-governance-policy.md)

---

### Model Risk Policy

**KB-PORTFOLIO-0012 | Owner: CRO | Parent: AI Governance Policy | 

The operational model lifecycle policy subordinate to the AI Governance Policy. Governs the identification, development, independent validation, deployment authorisation, ongoing monitoring, overlay management, incident response, and retirement of all quantitative and AI/ML models. The only policy in the framework with direct SR 11-7 alignment: a deliberate choice signalling readiness for regulated-industry clients and financial services contexts.

**Key design decisions:**
- Independent validation is a hard requirement for Tier 1 and Tier 2 models: not a recommendation. Deployment authorisation is blocked without it. This is not how most portfolio policies handle validation, and the deliberate structural choice is worth noting.
- The tiering framework has seven assessment dimensions, each with explicit Tier 1/2/3 criteria. Tier assignment is not subjective: it is a documented, committee-reviewed decision with an audit trail.
- The Veridian AI models receive dedicated treatment in the tiering section: a named rationale block explains why both systems land at Tier 1, and the interim monitoring arrangements section acknowledges the operational reality of governing systems that predate the policy.
- Overlay and adjustment governance is often absent from model risk policies. Recurring overlays in the same direction are defined as a revalidation trigger: a control that catches model failures masked by manual correction before they become incidents.
- SR 11-7 Section III (Model Validation) is the primary reference for validation independence requirements: the standard that regulated financial institutions and their technology vendors are expected to meet.

**Frameworks:** SR 11-7 (Federal Reserve / OCC Sections I–IV); NIST AI RMF 1.0; EU AI Act Articles 9, 10, 11, 15, 72; ISO/IEC 42001:2023; ISO/IEC 23894:2023; ISO/IEC 27001:2022

👉 [Read the Model Risk Policy](./model-risk-policy.md)

---

### Privacy and Data Protection Policy

**KB-PORTFOLIO-0013 | Owner: DPO | 

Will govern the organisation's obligations under GDPR and UK GDPR, including lawful basis for processing, data subject rights management, Data Protection Impact Assessments (DPIAs), and the DPO function. The AI Governance Policy and Model Risk Policy both reference this policy for training data governance and AI system impact assessment obligations. Being developed to address the intersection of GDPR and EU AI Act obligations: including DPIA requirements for High-Risk AI systems processing personal data, an area where the two regulatory frameworks create overlapping and occasionally conflicting obligations.

👉 [Read the Privacy and Data Protection Policy](./privacy-and-data-protection-policy.md)

---

### Security Awareness and Training Policy

**KB-PORTFOLIO-0014 | Owner: CISO | 

Will govern security awareness training requirements across Emyzer Nexus, including AI-specific training obligations referenced in the AI Governance Policy (AI awareness training within 30 days of hire) and Model Risk Policy (model-specific user training before operational access). Being developed to consolidate training obligations currently distributed across four policies into a single governance document with unified LMS tracking and completion reporting.

👉 [Read the Security Awareness and Training Policy](./security-awareness-and-training-policy.md)

---

## Design Principles

These principles governed every policy in the framework. They are worth stating explicitly because they explain why the documents look the way they do: and why certain deliberate choices might initially look unusual.

**Controls are testable, not aspirational.** Every requirement is written to be verifiable. "Human operators can understand and override AI system outputs" is not a testable control. "Human oversight mechanisms shall be tested annually with results documented in a validation report retained for 5 years" is. The difference matters to auditors, regulators, and practitioners evaluating whether a policy does what it claims.

**Accountability is named, not distributed.** Each policy names specific roles: not "relevant stakeholders" or "appropriate personnel." Named accountability is harder to write, because it requires understanding the organisational structure well enough to assign obligations to real functions. It is also the only kind of accountability that works.

**The acquisition scenario is a feature, not a complication.** Most portfolio GRC work is written for clean environments. The Veridian AI acquisition creates inherited risk, documentation gaps, interim operating arrangements, and remediation timelines: the conditions under which GRC practitioners actually operate. Governing that scenario demonstrates more than governing a greenfield build.

**Policies are a system.** Individual policy documents are less important than the policy architecture they form. Cross-references are intentional. Definitions are consistent. Evidence retention periods are coordinated. The framework is designed to hold together under audit, not just to read well in isolation.

**Evidence requirements are specific.** Every Tier 1 policy includes a comprehensive evidence index with system of record, owner, and retention period for each evidence type. This is how compliance is demonstrated: not through policy documents, but through the records they require.

---

## Framework Coverage

| Standard / Regulation | Policies Aligned |
|----------------------|-----------------|
| **ISO 27001:2022** | All Phase 1 policies; AI Governance Policy; Model Risk Policy |
| **ISO 31000:2018** | Risk Management Policy; Third-Party Risk Management Policy; AI Governance Policy |
| **EU AI Act (Regulation 2024/1689)** | AI Governance Policy; Model Risk Policy |
| **NIST AI RMF 1.0** | AI Governance Policy; Model Risk Policy |
| **ISO/IEC 42001:2023** | AI Governance Policy; Model Risk Policy |
| **ISO/IEC 23894:2023** | AI Governance Policy; Model Risk Policy |
| **SR 11-7 (Federal Reserve / OCC)** | Model Risk Policy |
| **NIST CSF 2.0** | Information Security Policy; Risk Management Policy; Third-Party Risk Management Policy |
| **NIST SP 800-53 Rev. 5** | Access Control Policy; Vulnerability Management Policy; AI Governance Policy |
| **NIST SP 800-61 Rev. 2** | Incident Management Policy |
| **ISO 22301:2019** | Business Continuity Policy |
| **ISO 27035:2023** | Incident Management Policy |
| **ITIL 4** | Change Management Policy |
| **CIS Controls v8** | Vulnerability Management Policy |
| **GDPR / UK GDPR** | Data Classification Policy; Privacy and Data Protection Policy (in development) |
| **ISO 27701:2019** | Privacy and Data Protection Policy (in development) |

---

## Skills Demonstrated

This framework demonstrates the following GRC competencies:

**Policy Architecture and Hierarchy**: Designing a coherent multi-policy framework with intentional parent-child relationships, consistent definitions, and cross-policy dependencies that hold together under audit. Not writing individual policies; building a system.

**EU AI Act Implementation**: Mapping regulatory obligations from a complex regulation to operational policy controls, including prohibited practices enforcement, conformity assessment design, human oversight requirements, post-market monitoring cadences, and Article 73 regulatory notification integration.

**AI and Model Risk Governance**, Applying NIST AI RMF and SR 11-7 to design tiered governance structures, independent validation frameworks, monitoring escalation triggers, and overlay governance, the controls that manage AI and model risk at the operational level, not just the strategic level.

**Acquisition Risk Management**, Designing governance that accounts for inherited risk, documentation gaps, and interim operating arrangements, the conditions that arise when an organisation acquires technology that predates its governance framework.

**Evidence Architecture**: Building evidence indexes with defined systems of record, named owners, and retention periods calibrated to regulatory and operational requirements. Understanding that policies create compliance obligations, and compliance is demonstrated through records.

**Risk-Proportionate Control Design**: Applying tiered governance frameworks that concentrate the most rigorous controls on the highest-risk systems, rather than applying uniform requirements regardless of materiality. Demonstrating judgment about where controls add value and where they add only burden.

**Cross-Framework Alignment**, Navigating the intersection of multiple frameworks, EU AI Act, ISO 27001, NIST AI RMF, SR 11-7, GDPR, without treating them as independent checklists, and identifying where they create overlapping, complementary, or occasionally conflicting obligations.

**Technical Communication**: Writing policy documents that are precise enough to be audited, readable enough to be used by non-specialists, and structured to support the decision-making of practitioners who need to act on them quickly.

---

## Repository Structure

```
policies/
├── README.md                              ← You are here
│
├── Phase 1: Foundation
│   ├── information-security-policy.md     KB-PORTFOLIO-0001
│   ├── risk-management-policy.md          KB-PORTFOLIO-0002
│   ├── data-classification-policy.md      KB-PORTFOLIO-0003
│   ├── acceptable-use-policy.md           KB-PORTFOLIO-0004
│   ├── access-control-policy.md           KB-PORTFOLIO-0005
│   ├── incident-management-policy.md      KB-PORTFOLIO-0006
│   ├── business-continuity-policy.md      KB-PORTFOLIO-0007
│   ├── third-party-risk-management-policy.md  KB-PORTFOLIO-0008
│   ├── change-management-policy.md        KB-PORTFOLIO-0009
│   └── vulnerability-management-policy.md KB-PORTFOLIO-0010
│
└── Phase 2: AI and Advanced Risk
    ├── ai-governance-policy.md            KB-PORTFOLIO-0011  ✓ Published
    ├── model-risk-policy.md               KB-PORTFOLIO-0012  ✓ Published
    ├── privacy-data-protection-policy.md  KB-PORTFOLIO-0013  ⧖ In Development
    └── security-awareness-training-policy.md  KB-PORTFOLIO-0014  ⧖ In Development
```

---

## Further Reading

GRC practice involves judgment calls that policy documents can't fully capture: trade-offs between control rigour and operational feasibility, decisions about where frameworks conflict, and the institutional dynamics that determine whether a governance program actually works. I write about these topics at:

**[cleanlikesoapblog.wordpress.com/category/grc](https://cleanlikesoapblog.wordpress.com/category/grc/)**

Posts in that category cover EU AI Act implementation considerations, model risk governance in practice, and the intersection of GRC program design with real organisational constraints.

---

*This policy framework is a portfolio artifact developed under the Emyzer Nexus GRC scenario. All organisations, individuals, and systems referenced are fictional. Framework and regulatory references are accurate as of the document publication dates.*

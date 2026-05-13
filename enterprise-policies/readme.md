# Enterprise Policies

**Emyzer Nexus: Phase 2 | Fictional case study.**

> All entities, systems, personnel, and scenarios are invented for professional demonstration purposes. Framework references are accurate as of the document dates. `[VERIFY]` tags flag regulatory citations requiring legal confirmation before use in a real context.

---

## What This Directory Contains

Four enterprise-level policies governing Emyzer Nexus as the post-acquisition parent entity. These policies exist because the Phase 1 Emyzer Technology policies did not cover the governance domains introduced by the Veridian AI acquisition: AI system governance, model lifecycle management, the GDPR obligations created by AI training data and external LLM API use, and the EU AI Act human oversight training requirement.

Each policy closes a specific gap. None of them repeat what Phase 1 already established.

---

## 60-Second Review Path

| If you want to evaluate... | Start here |
|---|---|
| EU AI Act implementation | [AI Governance Policy](ai-governance-policy.md) then [EU AI Act Control Mapping](../ai-governance/eu-ai-act-mapping.md) |
| Model lifecycle governance and SR 11-7 alignment | [Model Risk Policy](model-risk-policy.md) |
| GDPR obligations at the AI training data and LLM API layer | [Privacy and Data Protection Policy](privacy-and-data-protection-policy.md) |
| Policy hierarchy connecting Phase 1 to Phase 2 | [Emyzer Technology Overview](../emyzer-technology/README.md) then [M&A GRC Integration Charter](../integration-management/m%26a-grc-integration-charter.md) |

---

## Policy Architecture

These four policies sit at the top of the Phase 2 policy hierarchy. Below them, Phase 1 Emyzer Technology policies remain in effect as subsidiary documentation.

```
Information Security Policy (Phase 1, KB-PORTFOLIO-0001)
│
├── AI Governance Policy (Phase 2, KB-PORTFOLIO-0011)
│   │   Strategic governance for all AI/ML systems. EU AI Act obligations.
│   │   Parent to the Model Risk Policy for AI/ML systems.
│   │
│   └── Model Risk Policy (Phase 2, KB-PORTFOLIO-0012)
│           Operational model lifecycle. Independent validation. SR 11-7 alignment.
│           Monitoring escalation. Overlay governance.
│
├── Privacy and Data Protection Policy (Phase 2, KB-PORTFOLIO-0013)
│       GDPR obligations for AI training data and LLM API data processing.
│       DPIA requirements. Data subject rights in automated decision contexts.
│
└── Security Awareness and Training Policy, Tier 2 (Phase 2, KB-PORTFOLIO-0014)
        EU AI Act Article 14 human oversight training obligations.
        Extends Phase 1 training programme with AI-specific curriculum.
```

**Why this matters:** A Tier 1 AI system at Emyzer Nexus touches all four of these policies simultaneously: the AI Governance Policy governs its lifecycle, the Model Risk Policy governs its operational controls, the Privacy Policy governs its training data and output handling, and the Training Policy governs who is authorised to interact with it. Each cross-policy reference in this framework is traceable.

---

## Policies

### [AI Governance Policy](ai-governance-policy.md)

**KB-PORTFOLIO-0011 | Owner: CISO | Parent: Information Security Policy**

The gap this closes: Phase 1 had no AI governance framework. Veridian AI's two systems were in production under EU AI Act High-Risk classification with no conformity governance in place at acquisition close.

This policy creates the governance structure. It establishes the AI Governance Committee as the named classification and conformity assessment authority, not a vague stakeholder body. It defines High-Risk system obligations under EU AI Act Articles 9-15 as testable operational requirements. It sets conditions for post-market monitoring activation and defines prohibited AI practices.

**Key design decisions:**
- Human oversight requirements are written to EU AI Act Article 14 standards: operators must be able to understand, monitor, intervene in, and halt AI system outputs. These obligations are testable, not aspirational.
- Third-party LLM API opacity is treated as a documented limitation requiring compensating controls: human review of outputs, committee-level acknowledgement of the constraint, and disclosure in conformity documentation. The limitation is not ignored.
- The Veridian AI acquisition is woven through the scope, the systems-in-scope table, and the evidence requirements: governance designed for realistic conditions, not ideal ones.

**Frameworks:** EU AI Act (Articles 9-15, 72, 73) [VERIFY], NIST AI RMF 1.0, ISO/IEC 42001:2023, ISO/IEC 23894:2023

---

### [Model Risk Policy](model-risk-policy.md)

**KB-PORTFOLIO-0012 | Owner: CRO | Parent: AI Governance Policy**

The gap this closes: Phase 1 had no model lifecycle controls. PCM-001 and CRT-001 were in production without documented validation, monitoring cadences, or escalation triggers. This policy operationalises the AI Governance Policy at the model level.

This is the only policy in the framework with direct SR 11-7 alignment: a deliberate choice signalling readiness for regulated-industry clients and financial services contexts where model risk governance is a compliance requirement, not a best practice.

**Key design decisions:**
- Independent validation is a hard requirement for Tier 1 and Tier 2 models. Deployment authorisation is blocked without it. This is not a recommendation.
- The tiering framework uses seven assessment dimensions with explicit Tier 1/2/3 criteria. Tier assignment is a documented, committee-reviewed decision with an audit trail, not a subjective judgment.
- Overlay and adjustment governance is often absent from model risk policies. Recurring overlays in the same direction are a defined revalidation trigger: the control that catches model failures masked by manual correction before they become incidents.
- The Veridian AI models receive dedicated treatment: a named rationale block explains why both systems land at Tier 1, and the interim monitoring arrangements section acknowledges the operational reality of governing systems that predate the policy.

**Frameworks:** SR 11-7 (Federal Reserve/OCC, Sections I-IV), NIST AI RMF 1.0, EU AI Act (Articles 9-11, 15, 72) [VERIFY], ISO/IEC 42001:2023

---

### [Privacy and Data Protection Policy](privacy-and-data-protection-policy.md)

**KB-PORTFOLIO-0013 | Owner: DPO | Parent: Information Security Policy**

The gap this closes: Veridian's data processing activities created two GDPR obligations not addressed in Phase 1. PCM-001 trained on customer PII, creating data governance obligations for training datasets. CRT-001 transmitted contract data to an external LLM API, creating data processor obligations under GDPR Article 28 [VERIFY] that were unresolved at acquisition close.

This policy establishes the lawful basis for each processing activity, DPIA requirements for High-Risk AI systems processing personal data, data subject rights procedures for automated decision contexts, and the conditions under which CRT-001's data processing can resume full operation.

**Key design decisions:**
- DPIA requirements for High-Risk AI systems are defined at the intersection of GDPR Article 35 [VERIFY] and EU AI Act Title III obligations: the two frameworks create overlapping and occasionally conflicting requirements, and this policy navigates that intersection explicitly.
- Data processor agreements for external LLM API vendors are required before personal data may be transmitted: the specific gap that triggered CRT-001's restricted use restriction at acquisition close.

**Frameworks:** GDPR (Regulation 2016/679) [VERIFY], UK GDPR, ISO 27701:2019

---

### [Security Awareness and Training Policy (Tier 2)](security-awareness-and-training-policy.md)

**KB-PORTFOLIO-0014 | Owner: CISO | Parent: Security Awareness and Training Policy (Phase 1)**

The gap this closes: EU AI Act Article 14 requires that staff interacting with High-Risk AI systems receive training enabling them to understand the system's capabilities and limitations, interpret outputs correctly, and exercise effective human oversight. The Phase 1 training policy did not include this obligation.

This Tier 2 policy extends the Phase 1 programme with AI-specific curriculum requirements for staff with operational access to PCM-001 and CRT-001. It does not replace the Phase 1 programme: it adds obligations to it, using the Phase 1 completion tracking infrastructure.

**Key design decisions:**
- Training is a prerequisite for access provisioning. Under the Access Control Policy, model operator access is not granted until training is complete: the control that prevents untrained staff from operating High-Risk systems.
- Role-based curriculum: operators of PCM-001 receive churn model-specific training; operators of CRT-001 receive contract review-specific training. Generic AI awareness training does not satisfy Article 14 for either system.

**Frameworks:** EU AI Act Art. 14 [VERIFY], ISO 27001:2022 A.6.3, NIST SP 800-50

---

## Design Principles Applied Across All Four Policies

**Controls are testable, not aspirational.** Every requirement is written to be verifiable. "Human oversight mechanisms shall be tested annually with results documented in a validation report retained for 5 years" is a testable control. "Human operators should be able to understand AI outputs" is not. The difference matters in an audit.

**Accountability is named.** Each policy names specific roles, not "relevant stakeholders." Named accountability is harder to write because it requires knowing the organisational structure well enough to assign obligations to real functions. It is the only kind of accountability that works.

**Policies are a system.** Cross-references between these four policies and the Phase 1 framework are intentional. Definitions are consistent. Evidence retention periods are coordinated. The framework is designed to hold together under audit.

**Evidence requirements are specific.** Every Tier 1 policy includes an evidence index with system of record, owner, and retention period for each evidence type. This is how compliance is demonstrated: not through policy documents, but through the records they require.

---

## Framework Coverage

| Standard / Regulation | Policies Aligned |
|---|---|
| EU AI Act (Regulation 2024/1689) [VERIFY] | AI Governance Policy, Model Risk Policy, Security Awareness and Training Policy (Tier 2) |
| NIST AI RMF 1.0 | AI Governance Policy, Model Risk Policy |
| ISO/IEC 42001:2023 | AI Governance Policy, Model Risk Policy |
| SR 11-7 (Federal Reserve / OCC) | Model Risk Policy |
| GDPR / UK GDPR | Privacy and Data Protection Policy |
| ISO 27701:2019 | Privacy and Data Protection Policy |
| ISO 27001:2022 | All four policies |
| NIST SP 800-50 | Security Awareness and Training Policy (Tier 2) |

---

## Related Documentation

| Document | Description |
|---|---|
| [Portfolio Overview](../README.md) | Top-level narrative and 60-second review path |
| [Emyzer Nexus Overview](../emyzer-nexus/readme.md) | Phase 2 programme context and key governance decisions |
| [AI Governance Programme](../ai-governance/readme.md) | AI programme detail: system inventory, EU AI Act mapping, risk assessments |
| [Phase 1 Policies](../policies/README.md) | The 10 Phase 1 Emyzer Technology policies these four policies extend |

---

*All content in this portfolio is a fictional case study. Framework and regulatory references are accurate as of the document publication dates.*

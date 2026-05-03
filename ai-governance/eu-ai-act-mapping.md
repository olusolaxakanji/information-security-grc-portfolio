# EU AI Act Control Mapping

**Emyzer Nexus — AI Governance Programme**

---

## Document Information

| Attribute | Value |
|---|---|
| **Document ID** | AI-MAP-001 |
| **Document Type** | Compliance Control Mapping |
| **Version** | 1.0 |
| **Effective Date** | 2025-06-01 |
| **Owner** | AI Governance Committee / Legal Counsel |
| **Classification** | Internal Use |
| **Review Cadence** | Annual; updated when EU AI Act implementing acts are published |
| **Systems in Scope** | PCM-001 (Predictive Customer Churn Model), CRT-001 (AI-Assisted Contract Review Tool) |

---

## 1. Purpose and Scope

This document maps the compliance obligations imposed by EU AI Act (Regulation 2024/1689) [VERIFY] on Emyzer Nexus's two High-Risk AI systems to the controls and evidence currently in place. It covers Articles 9, 10, 11, 13, 14, 15, 72, and 73 — the core High-Risk system obligations — and identifies compliance gaps with associated remediation priorities.

The mapping serves three purposes:

1. **Audit readiness** — provides a traceable record connecting regulatory obligations to operational controls and evidence
2. **Gap management** — identifies where controls are absent or insufficient, enabling prioritised remediation planning
3. **Governance reporting** — gives the AI Governance Committee a structured view of compliance posture across both systems

**[VERIFY] tags** appear throughout this document on specific article citations. These tags indicate that Legal Counsel should confirm the precise applicability, scope, and interpretation of the cited provision before the compliance position is relied upon in any regulatory context.

---

## 2. Mapping Methodology

### 2.1 Compliance Assessment Approach

Compliance status was assessed through:
- Review of existing system documentation inherited from Veridian AI
- Technical interviews with the VP Customer Success (PCM-001 owner) and General Counsel (CRT-001 owner)
- Review of controls implemented or planned under the AI Governance Policy
- Gap analysis against published EU AI Act text [VERIFY] and available guidance

### 2.2 Status Definitions

| Status | Definition |
|---|---|
| **Compliant** | Requirement is fully met; evidence exists and is current |
| **Partial** | Requirement is partially met; controls exist but gaps remain; remediation in progress or planned |
| **Gap** | Requirement is not met; no control currently in place; remediation required |
| **Gap — Critical** | Requirement is not met and creates significant regulatory or operational risk; immediate remediation required |
| **Not Applicable** | Requirement does not apply to this system based on its classification or use case |

---

## 3. Article-by-Article Mapping

### 3.1 Article 9 — Risk Management System [VERIFY]

**Requirement summary:** High-Risk AI systems must have a risk management system established, implemented, documented, and maintained throughout the system's lifecycle. The system must identify and analyse known and foreseeable risks; estimate and evaluate risks arising from normal use and reasonably foreseeable misuse; adopt appropriate risk management measures; test systems for their intended purpose.

| Requirement | PCM-001 Status | PCM-001 Evidence / Notes | CRT-001 Status | CRT-001 Evidence / Notes |
|---|---|---|---|---|
| Risk management system documented and maintained | Partial | AI System Risk Assessment (AI-RA-2025-001) initiated; 4 risks identified and under treatment | Partial | AI System Risk Assessment (AI-RA-2025-002) initiated; 4 risks identified; 2 rated Critical (LLM hallucination, data privacy) |
| Known and foreseeable risks identified | Partial | Model drift and training data bias documented; explainability gap documented; further threat modelling required | Partial | Hallucination, dependency risk, data privacy, and prompt injection documented; full threat model not yet complete |
| Risks from foreseeable misuse assessed | Gap | Misuse assessment not yet formally documented | Gap | Prompt injection from malicious contract content assessed at medium severity; broader misuse analysis not documented |
| Risk management measures adopted and proportionate | Partial | Human override capability implemented; drift monitoring active; operator training complete | Partial | Mandatory legal review of all outputs; use restriction for PII-containing contracts; operator training complete |
| Testing throughout lifecycle | Partial | Performance baselines established; quarterly re-evaluation against held-out validation set | Gap | Testing of third-party LLM component not possible due to API opacity; output quality sampling programme in place as proxy |

---

### 3.2 Article 10 — Data and Data Governance [VERIFY]

**Requirement summary:** Training, validation, and test data must meet quality criteria (relevance, representativeness, and as free of errors as possible); data governance and management practices must be established covering data preparation, labelling, provenance; known biases must be examined and addressed; data must not contain personal data beyond what is necessary.

| Requirement | PCM-001 Status | PCM-001 Evidence / Notes | CRT-001 Status | CRT-001 Evidence / Notes |
|---|---|---|---|---|
| Training data quality criteria documented | Partial | Training data schema documented; quality criteria (completeness, freshness) informally applied; formal quality standard not yet documented | Not Applicable (direct) | Emyzer Nexus does not control LLM API training data; [VERIFY: whether Article 10 obligations transfer to deployers when using third-party foundation models] |
| Data provenance documented | Gap | Training data provenance documentation incomplete — collected by Veridian AI pre-acquisition; original data collection consent and lawful basis not verified | Gap — Critical | LLM API vendor training data provenance entirely unknown to Emyzer Nexus; vendor has not provided this information |
| Bias examination completed | Partial | Preliminary demographic-neutral assessment performed; no protected characteristic bias testing completed; gap — quarterly bias audit scheduled | Gap — Critical | No bias information available for third-party LLM training data; hallucination rate tracking in progress |
| Data governance practices established | Gap | DPO review in progress; training data retention schedule not documented; access controls on training data not audited | Gap — Critical | GDPR Article 28 [VERIFY] DPA with LLM API vendor not executed; data processing terms unresolved |
| Personal data in training data minimised | Gap | PCM-001 training data contains client personal data (names implicitly via account IDs; usage behaviour); DPIA not yet completed | Gap | Contract documents (input data) contain personal data; transmitted to external API without DPA in place |

---

### 3.3 Article 11 — Technical Documentation [VERIFY]

**Requirement summary:** Technical documentation must be drawn up before a High-Risk AI system is placed on the market or put into service and kept up-to-date. Documentation must demonstrate compliance with the regulation and allow authorities to assess compliance. Minimum content requirements are set out in Annex IV [VERIFY].

| Requirement | PCM-001 Status | PCM-001 Evidence / Notes | CRT-001 Status | CRT-001 Evidence / Notes |
|---|---|---|---|---|
| Technical documentation drawn up before deployment | Gap | System was already deployed pre-acquisition; documentation sprint initiated post-classification; partial documentation available from Veridian AI engineering | Gap — Critical | System already deployed pre-acquisition; third-party API technical documentation unavailable from vendor |
| Documentation current and complete (Annex IV [VERIFY]) | Partial | Model architecture, training methodology, and performance metrics partially documented; gaps in intended purpose statement and known limitation disclosure | Gap — Critical | Cannot produce complete Annex IV documentation without third-party vendor cooperation; critical gap for regulatory examination |
| Documentation available to authorities on request | Partial | Partial documentation maintained in document repository; completion target 2025-09-30 for PCM-001 | Gap — Critical | Full documentation cannot be produced due to third-party API opacity; interim position: document the limitation with compensating controls |
| Documentation updated following material change | Documented (procedure) | Change management process extended to require technical documentation update for any model retraining | Documented (procedure) | API version change process defined; triggers documentation review |

---

### 3.4 Article 13 — Transparency and Provision of Information to Deployers [VERIFY]

**Requirement summary:** High-Risk AI systems must be designed and developed to ensure sufficient transparency so that deployers can understand and use the system appropriately. Systems must be accompanied by instructions for use (concise, complete, correct, and clear), covering intended purpose, accuracy level, known biases, foreseeable unintended outcomes, human oversight measures, and the characteristics, capabilities, and limitations.

| Requirement | PCM-001 Status | PCM-001 Evidence / Notes | CRT-001 Status | CRT-001 Evidence / Notes |
|---|---|---|---|---|
| Instructions for use documented | Partial | Operator guide exists (inherited from Veridian AI); limited on accuracy levels and bias disclosures; update in progress | Partial | Legal team guidance document exists; lacks structured capability/limitation disclosure |
| Accuracy level disclosed | Partial | Overall model accuracy and AUC score documented at aggregate level; per-segment accuracy not yet disclosed | Gap | Third-party LLM accuracy characteristics not disclosed by vendor; hallucination rate measured empirically by Emyzer Nexus but not systematically disclosed to operators |
| Known biases disclosed | Gap | Bias disclosure to operators not yet implemented; bias testing not completed | Gap | Cannot disclose LLM bias characteristics as this information is not available from vendor |
| Foreseeable unintended outcomes disclosed | Partial | Operator training includes awareness of model limitations (lag, coverage gaps for non-Veridian client segments) | Partial | Hallucination risk disclosed in operator training; not captured in formal instructions for use |
| Human oversight measures described | Documented | Operator guide and training describe override capability and escalation | Documented | Mandatory legal review described in operator guide; override (discard all AI output) available |
| Limitations of system disclosed | Partial | Explainability limitation disclosed in training; quarterly retraining lag disclosed | Partial | Third-party API dependency limitation disclosed; explainability limitation disclosed |

---

### 3.5 Article 14 — Human Oversight [VERIFY]

**Requirement summary:** High-Risk AI systems must be designed and developed with appropriate human oversight measures enabling individuals to monitor the system's performance, understand the system's capabilities and limitations, detect and address failures, override or disregard outputs, and halt the system if necessary.

| Requirement | PCM-001 Status | PCM-001 Evidence / Notes | CRT-001 Status | CRT-001 Evidence / Notes |
|---|---|---|---|---|
| Operators can understand outputs | Partial | Churn score and tier communicated clearly; individual score rationale not available (model opacity) | Partial | Output format (clause analysis, flags) is human-readable; rationale for LLM positions not available |
| Operators can monitor performance | Compliant | Weekly score review cadence; CS managers review flagged accounts before action; anomaly reporting channel | Compliant | Legal team reviews all outputs; anomalous outputs reported to General Counsel for follow-up |
| Operators can detect failures | Partial | Anomaly thresholds defined in monitoring programme; detection relies on aggregate metrics, not individual output quality | Partial | Individual output quality monitored via solicitor review; no automated hallucination detection capability |
| Operators can override outputs | Compliant | CS managers can suppress or override any score-triggered workflow; no automated action taken without human approval | Compliant | All CRT-001 outputs are advisory; Legal team may and frequently does disregard AI analysis; all-output-override is the default position |
| System can be halted | Compliant | Kill switch procedure documented; CISO or General Counsel can suspend system use; emergency halt procedure tested | Compliant | System can be suspended at any time; interim use restriction (no PII contracts) demonstrates partial suspension capability |
| Operator training completed before access | Compliant | 23 operators trained; LMS records confirm completion; access control system prevents login before training certification | Compliant | 8 operators trained; LMS records confirm completion; access requires training certification |

---

### 3.6 Article 15 — Accuracy, Robustness, and Cybersecurity [VERIFY]

**Requirement summary:** High-Risk AI systems must achieve an appropriate level of accuracy, robustness, and cybersecurity across their lifecycle. Systems must be resilient to errors, faults, and inconsistencies. Performance levels must be declared in technical documentation. Adversarial input resilience must be assessed.

| Requirement | PCM-001 Status | PCM-001 Evidence / Notes | CRT-001 Status | CRT-001 Evidence / Notes |
|---|---|---|---|---|
| Performance level declared in documentation | Partial | Overall accuracy, AUC score, and precision/recall metrics documented at aggregate level; per-tier accuracy not yet documented | Gap | Third-party LLM performance characteristics not declared by vendor; empirical hallucination rate tracked by Emyzer Nexus |
| Resilience to errors and faults | Partial | Model degrades gracefully to conservative scoring if input data is incomplete; error handling in ingestion pipeline | Partial | Preprocessing pipeline handles malformed documents; LLM API errors cause graceful failure (no output) rather than incorrect output |
| Resilience to inconsistencies in input | Partial | Input validation applied in ingestion pipeline; performance on out-of-distribution inputs not formally tested | Gap | Prompt injection risk from malicious contract content not fully assessed; input sanitisation in development |
| Adversarial input resilience assessed | Gap | Adversarial testing against PCM-001 not yet conducted; planned for Q3 2025 | Gap | Cannot conduct adversarial testing on opaque third-party model; prompt injection is the primary adversarial risk; sanitisation in development |
| Cybersecurity measures in place | Compliant | Model artifacts stored in secured S3 bucket (encryption at rest and in transit); IAM access controls; no external API calls | Partial | Preprocessing layer secured; external API call over TLS; API key managed in AWS Secrets Manager; vendor security posture not independently verified |

---

### 3.7 Article 72 — Post-Market Monitoring [VERIFY]

**Requirement summary:** Providers of High-Risk AI systems must establish and document a post-market monitoring system proportionate to the nature of the AI technology and risks. The system must collect, document, and analyse data from deployers and users on the AI system's performance. Providers must report serious incidents. EU database registration required for most High-Risk systems.

| Requirement | PCM-001 Status | PCM-001 Evidence / Notes | CRT-001 Status | CRT-001 Evidence / Notes |
|---|---|---|---|---|
| Post-market monitoring plan documented | Compliant | PCM-001 Monitoring Plan documented; monthly performance review; quarterly drift assessment; bias audit cadence defined | Partial | CRT-001 Monitoring Plan documented; output quality sampling; hallucination rate tracking; gap: systematic bias assessment not possible |
| Data collection from deployers | Compliant | CS team anomaly reporting process; weekly override log review; quarterly performance briefing from AI System Owner | Partial | Legal team output quality feedback channel; override log maintained; no automated collection capability |
| Anomaly reporting to AI system owner | Compliant | CS anomaly reports reviewed within 5 business days; escalation to CISO if performance degradation detected | Compliant | Legal anomaly reports reviewed by General Counsel; escalation to CISO for significant findings |
| Serious incident reporting (Art.73 [VERIFY]) | Procedure documented | Procedure in place; no incidents to date | Procedure documented | Procedure in place; no incidents to date |
| EU AI database registration [VERIFY: timing of obligation] | Planned | Registration planned once conformity assessment complete; target Q4 2025 | Planned | Registration deferred pending conformity assessment completion; complex due to third-party API dependency |

---

### 3.8 Article 73 — Reporting of Serious Incidents [VERIFY]

**Requirement summary:** Providers of High-Risk AI systems must report any serious incident — defined as an incident that directly or indirectly leads to the death or serious damage to the health of persons, a serious disruption of critical infrastructure, or a breach of fundamental rights obligations — to the market surveillance authority of the relevant Member State(s). Timeframes and specific reporting obligations are set out in implementing acts [VERIFY: implementing act publication status].

| Requirement | PCM-001 Status | PCM-001 Evidence / Notes | CRT-001 Status | CRT-001 Evidence / Notes |
|---|---|---|---|---|
| Serious incident definition understood and documented | Partial | AI incident classification procedure references Article 73 [VERIFY]; definition applied in Incident Management Policy extension | Partial | Same procedure applies; note that CRT-001 legal analysis errors could constitute a serious incident if they contribute to decisions affecting fundamental rights |
| Notification procedure to market surveillance authority | Documented | Incident response runbook includes Art.73 [VERIFY] notification procedure; Legal Counsel designated as notification authority | Documented | Same procedure; Legal Counsel to assess whether contract-related incidents trigger notification |
| Incident records maintained | Compliant | Incident records maintained in ServiceNow; retention 10 years per Evidence Index | Compliant | Same system |
| Incidents to date | None | No serious incidents involving PCM-001 detected since classification | None | No serious incidents involving CRT-001 detected since classification |

---

## 4. Gap Summary and Remediation Priorities

| Gap ID | Article | System | Gap Description | Priority | Owner | Target Date | Status |
|---|---|---|---|---|---|---|---|
| GAP-001 | Art.10 [VERIFY] | PCM-001 | Training data provenance not documented; lawful basis for personal data in training set not verified | High | DPO | 2025-09-30 | In Progress — DPO review initiated |
| GAP-002 | Art.10 [VERIFY] | CRT-001 | LLM API vendor training data provenance entirely unknown | **Critical** | General Counsel | 2025-09-30 | In Progress — vendor engagement initiated |
| GAP-003 | Art.10 [VERIFY] | CRT-001 | GDPR Article 28 [VERIFY] DPA with LLM API vendor not executed | **Critical** | Legal Counsel | 2025-09-30 | In Progress — DPA negotiation underway; use restriction in place |
| GAP-004 | Art.11 [VERIFY] | CRT-001 | Full Annex IV [VERIFY] technical documentation cannot be produced due to third-party API opacity | **Critical** | General Counsel / Legal Counsel | 2025-12-31 | Planning — vendor cooperation required; contingency: document limitation with compensating measures |
| GAP-005 | Art.11 [VERIFY] | PCM-001 | Technical documentation incomplete; Annex IV requirements not fully met | High | VP Customer Success / CTO | 2025-09-30 | In Progress — documentation sprint underway |
| GAP-006 | Art.13 [VERIFY] | PCM-001 | Bias disclosures not yet provided to operators; bias testing not complete | High | AI Governance Committee | 2025-09-30 | Planned — bias audit Q3 2025 |
| GAP-007 | Art.13 [VERIFY] | CRT-001 | LLM accuracy and bias characteristics cannot be disclosed due to vendor opacity | High | General Counsel | 2025-12-31 | Blocked — requires vendor engagement or alternative strategy |
| GAP-008 | Art.15 [VERIFY] | PCM-001 | Adversarial input testing not yet conducted | Medium | CTO | 2025-12-31 | Planned — Q3 2025 |
| GAP-009 | Art.15 [VERIFY] | CRT-001 | Prompt injection risk not fully mitigated; input sanitisation in development | High | CTO | 2025-09-30 | In Progress |
| GAP-010 | Art.9 [VERIFY] | Both | Full threat model and foreseeable misuse assessment not documented | Medium | AI Governance Committee | 2025-09-30 | In Progress |

---

## 5. Framework Alignment

| EU AI Act Article | NIST AI RMF Function | ISO/IEC 42001:2023 Clause | Current Control / Document |
|---|---|---|---|
| Article 9 — Risk Management | MAP, MEASURE, MANAGE | Cl. 6.1, 8.4 | AI System Risk Assessments; AI Governance Policy Section F |
| Article 10 — Data Governance | MAP | Cl. 8.4, Annex A A.6 | Data Classification Policy; DPO review programme |
| Article 11 — Technical Documentation | GOVERN, MAP | Cl. 7.5, 8.4 | Technical documentation sprint; Veridian AI documentation review |
| Article 13 — Transparency | GOVERN | Cl. 8.3 | Operator guides; training programme |
| Article 14 — Human Oversight | MANAGE | Cl. 8.4, Annex A A.8 | Human oversight protocols; operator training; override logging |
| Article 15 — Accuracy and Robustness | MEASURE | Cl. 8.4, Annex A A.9 | Post-market monitoring programme; adversarial testing (planned) |
| Article 72 — Post-Market Monitoring | MEASURE, MANAGE | Cl. 9.1, Annex A A.10 | PCM-001 and CRT-001 monitoring plans; quarterly AI Governance Committee review |
| Article 73 — Serious Incident Reporting | MANAGE | Cl. 10.1 | AI incident response extension; Legal Counsel notification procedure |

---

## 6. Document Control

| Version | Date | Author | Changes |
|---|---|---|---|
| 1.0 | 2025-06-01 | GRC Team | Initial publication |

- **Document ID:** AI-MAP-001
- **Classification:** Internal Use
- **Next Review:** 2026-06-01 or upon publication of EU AI Act implementing acts affecting Annex III classification or Article obligations

---

*This document was developed as part of the Emyzer Nexus Phase 2 AI Governance Programme and formatted for portfolio presentation.*

# Risk Assessment Programme

**Emyzer Technology: Phase 1 | Fictional case study.**

> All entities, systems, personnel, and risk findings are invented for professional demonstration purposes. Framework references are accurate as of the document dates.

---

## What a Risk Programme Needs to Accomplish

A risk assessment programme has one job: give decision-makers an accurate picture of the organization's risk posture so they can make defensible treatment decisions. That requires three things to work together: a methodology that produces consistent, comparable scores; a register that documents actual posture rather than comfortable posture; and an appetite statement that defines what the organization will and will not accept.

These three documents do exactly that. The methodology defines the process. The register applies it. The appetite statement sets the boundaries within which risk decisions are governed.

---

## Documents

### [Risk Assessment Methodology](risk-assessment-methodology.md)

The methodology establishes how risks are identified, scored, treated, and monitored across Emyzer Technology. It is the reference document every risk entry in the register traces back to for its scoring rationale.

**Six steps:** Risk identification, threat and vulnerability analysis, likelihood and impact scoring, risk rating determination, treatment selection, and monitoring cadence assignment.

**Scoring framework:** 5x5 matrix producing an inherent rating (before controls) and a residual rating (after controls). Hybrid qualitative/quantitative approach: qualitative for scenario-driven assessment, quantitative for financial exposure estimation where data supports it.

**Monitoring cadences by residual rating:** Critical risks reviewed monthly. High risks reviewed quarterly. Medium risks reviewed semi-annually. Low risks reviewed annually. Cadences are not uniform, because not all risks warrant the same monitoring investment.

**Multi-framework alignment:** NIST SP 800-30 Rev. 1 (primary process guidance), ISO 27005 (information security risk management), COBIT (IT governance integration), FAIR (quantitative methodology where applied).

**Extension at Phase 2:** The methodology is extended at Phase 2 with AI-specific risk categories: model drift, training data bias, explainability gaps, and third-party model dependency. The extension adds categories without replacing the framework, keeping AI risk findings comparable to the rest of the enterprise register.

### [Asset Risk Register](asset-risk-register.md)

15 risk entries across four categories: information security, privacy, operational, and third-party risk. Every entry carries an inherent rating, current controls, residual rating, treatment status, risk owner, and next review date.

**The most important entry in the register is not the highest-rated one.** One entry documents a budget-blocked Critical risk at its actual residual rating rather than adjusted downward to match what is available to mitigate it. The budget constraint is identified as the root cause. The risk is escalated to the Risk Management Committee accordingly.

Most GRC practitioners, when a critical risk cannot be mitigated due to budget, reclassify it to a lower level so the register looks clean. This register does not. That entry is the clearest signal in the document that it reflects actual risk posture, not comfortable risk posture.

**Treatment lifecycle coverage:** The register includes entries at every stage: newly identified, in active treatment, monitoring at residual level, and formally accepted. That range shows a functioning programme, not a one-time exercise.

### [Risk Appetite Statement](risk-appetite-statement.md)

Domain-specific tolerance thresholds governing how risk decisions are made and governed across Emyzer Technology.

**Four domains with defined thresholds:** Information security, privacy, operational, and third-party risk. Each domain has a quantitative and qualitative appetite expression calibrated to the organization's regulatory obligations and strategic context.

**Unacceptable risk conditions:** The statement defines risk conditions that cannot be accepted regardless of compensating controls or resource constraints. This puts a ceiling on risk acceptance decisions: the Risk Management Committee cannot formally accept a risk that meets an unacceptable condition, even if treatment is not immediately available.

**Audience:** Three audiences are served. Executives and the board need a clear mandate for risk-based decision making. Risk and security teams translate appetite into operational controls and treatment priorities. Auditors and regulators require evidence that risk governance is structured, intentional, and documented.

---

## How the Three Documents Work Together

The methodology defines how risks are scored and what treatment options apply. The register applies that methodology to 15 specific risks and records the treatment decisions made. The appetite statement defines the thresholds that govern which treatments are acceptable and which risks require formal acceptance or escalation.

A risk entry rated Critical that cannot be treated within appetite must be escalated to the Risk Management Committee before the next review cycle. That escalation path is the mechanism that connects all three documents in operation.

---

## Frameworks Applied

| Framework | Application |
|---|---|
| NIST SP 800-30 Rev. 1 | Primary risk assessment process guidance |
| ISO 27005 | Information security risk management principles |
| ISO 31000:2018 | Enterprise risk management methodology and risk appetite governance |
| NIST CSF 2.0 | ID.RA and ID.RM function alignment |
| COSO ERM | Risk appetite governance integration |
| FAIR | Quantitative risk assessment methodology where applied |

---

## Related Documentation

| Document | Description |
|---|---|
| [Emyzer Technology Overview](../emyzer-technology/README.md) | Phase 1 programme context |
| [Risk Management Policy](../policies/risk-management-policy.md) | Governance policy that authorizes this programme and defines the Risk Management Committee's role |
| [AI System Risk Assessments](../ai-governance/risk-assessments.md) | Phase 2 extension: methodology applied to PCM-001 and CRT-001 with AI-specific categories |
| [Portfolio Overview](../README.md) | Top-level narrative and 60-second review path |

---

*All content in this portfolio is a fictional case study. Framework and regulatory references are accurate as of the document publication dates.*

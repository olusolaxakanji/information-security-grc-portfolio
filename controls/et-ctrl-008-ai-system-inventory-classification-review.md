# ET-CTRL-008: AI System Inventory and Risk Classification Review

| Field | Value |
|---|---|
| Control ID | ET-CTRL-008 |
| Title | AI System Inventory and Risk Classification Review |
| Entity | Emyzer Nexus (Emyzer Technology operations in scope) |
| Regulatory citation | [EU AI Act (Regulation 2024/1689)](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32024R1689) Art. 9 (Risk management system for high-risk AI systems), Art. 10 (Data and data governance), Art. 11 (Technical documentation), Art. 49 (Registration of high-risk AI systems in the EU database) [VERIFY: confirm Art. 49 registration obligations and applicability timeline under transitional provisions]; [NIST AI RMF 1.0](https://airc.nist.gov/RMF) MAP 1.1 (Context is established), MAP 2.2 (Scientific findings and organizational risks are reasoned consistently), MEASURE 1.1 (AI risk metrics are defined); [ISO/IEC 42001:2023](https://www.iso.org/standard/81230.html) Cl. 6.1 (Actions to address risks and opportunities for AI management systems) |
| Control owner | Chief Information Security Officer |
| Control type | Preventive / Detective |
| Testing frequency | Annual; plus upon any material change to an AI system |
| Last tested | 2025-07-01 |
| Test result | Pass |
| Evidence reference | `evidence/2025/ET-CTRL-008/` |
| Status | Active |

---

## Control Description

The CISO, supported by the AI Governance Committee, maintains a current inventory of all AI systems in use across Emyzer Nexus, including Emyzer Technology operations and the inherited Veridian AI systems, and reviews risk classifications at least annually or upon any material change to an AI system.

**Inventory fields required per system (from AI Governance Policy KB-PORTFOLIO-0011):**

- System name and version
- Vendor or development origin
- Intended use case and affected user populations
- Data inputs and outputs (including training data sources for development-origin systems)
- Deployment environment
- EU AI Act risk tier classification (Unacceptable / High-Risk / Limited / Minimal)
- AI System Owner (named individual)
- Deployment date
- Last classification review date

**EU AI Act risk tiers:**

| Tier | Definition | Governance Requirement |
|---|---|---|
| Unacceptable | Prohibited practices under Art. 5 | Immediate decommission; no deployment |
| High-Risk | Systems falling under Annex III categories (e.g., employment, education, essential services, law enforcement) | Art. 9 risk management system; Art. 10 data governance; Art. 11 technical documentation; Art. 14 human oversight; Art. 15 accuracy and robustness; conformity assessment before deployment |
| Limited | Systems with specific transparency risks | Art. 13 transparency and information obligations |
| Minimal | All other AI systems | No mandatory requirements; voluntary code of practice applies |

**Veridian AI inherited systems:** Both the Predictive Customer Churn Model and the AI-Assisted Contract Review Tool are classified High-Risk. These systems are subject to the remediation timeline in the Policy Rationalization Roadmap and require independent validation under the Model Risk Policy (KB-PORTFOLIO-0012) before deployment authorisation can be granted.

**Material change trigger:** Any of the following events triggers an off-cycle classification review: change to the system's intended use case, significant update to training data, substantial model retrain or version upgrade, change to affected populations, or change to the deployment environment.

## Test Procedure

1. Pull the AI system inventory from `ai-governance/ai-system-inventory.md` and confirm it is dated within the last 12 months, or within 30 days of the most recent material change.
2. Verify that every system in the inventory has all required fields populated. Flag any field left blank as an exception requiring resolution within 10 business days.
3. For each High-Risk system: confirm the following documentation is on file and current: Article 9 risk management record, Article 10 data governance documentation, Article 11 technical documentation package, Article 14 human oversight controls design, and a completed conformity assessment report.
4. For the Veridian AI inherited systems specifically: confirm current remediation progress against the Policy Rationalization Roadmap. Document which governance milestones have been met and which remain outstanding. Confirm that any system operating under an interim monitoring arrangement has an arrangement that is still within its CISO-approved duration.
5. For any AI system where a material change occurred during the review period: confirm an off-cycle classification review was completed within 30 days of the change and the inventory was updated accordingly.
6. Confirm the AI Governance Committee reviewed and formally approved the annual inventory update in a documented committee meeting.
7. File the updated inventory, AI Governance Committee meeting minutes, conformity assessment evidence, and any interim monitoring arrangement approvals in `evidence/2025/ET-CTRL-008/`.

## Escalation

Discovery of an AI system not included in the inventory (shadow AI) is escalated to the CISO and AI Governance Committee within 24 hours. The system is suspended from operational use until it has been formally classified and, if classified High-Risk, an interim monitoring arrangement approved by the AI Governance Committee is in place. Legal Counsel assesses whether EU AI Act Article 73 regulatory notification obligations are triggered for any High-Risk system that was operating without the required governance documentation.

## Change History

| Version | Date | Changed by | Summary of change |
|---|---|---|---|
| 1.0 | 2026-01-13 | Chief Information Security Officer | Initial version |

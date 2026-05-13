# Business Continuity Programme

**Emyzer Technology: Phase 1 | Fictional case study.**

> All entities, systems, personnel, and scenarios are invented for professional demonstration purposes. ISO 22301:2019, NIST SP 800-34, and other framework references are accurate as of the document dates.

---

## What Business Continuity Documentation Needs to Do

Business continuity documentation has one purpose: give the organization the information it needs to continue critical operations during a disruption and recover them within defined timeframes. That requires recovery objectives grounded in actual operational data, not estimates. Estimated RTOs and RPOs do not hold up in a real incident or in an audit.

The Emyzer Technology BC programme starts with a 42-stakeholder Business Impact Analysis before setting a single recovery objective. The RTO and RPO targets in the BC/DR Policy are not chosen; they are derived.

---

## Documents

### [Business Impact Analysis Report](business-impact-analysis-report.md)

The BIA is the foundation the entire programme rests on. Without it, recovery objectives are guesses.

**42 stakeholder interviews** across Emyzer Technology's four business lines: hardware and device production, cloud service management, enterprise technical support, and global security implementation. Interviews identify which processes are critical, what their dependencies are, and what the financial and operational impact of disruption looks like at each time interval.

**4-tier process prioritisation:** Critical, High, Medium, and Low. Priority is determined by financial exposure, regulatory obligation, and customer contractual commitment. Processes in the same tier share RTO/RPO targets.

**Financial exposure quantification across 12 critical processes.** Each process has a documented revenue impact per hour of downtime, a regulatory penalty exposure where applicable, and a reputational impact assessment. These figures are what RTO targets are calibrated against.

**RTO range:** 4-24 hours, tiered by process criticality.
**RPO range:** 1-24 hours, tiered by data sensitivity and transaction volume.

The BIA report is the document that answers "why is this RTO 4 hours and not 8?" in an audit or an incident debrief. Without it, the answer is "because we decided that." With it, the answer is "because the financial exposure analysis showed X per hour of downtime for that process class."

### [Business Continuity and DR Policy](../policies/bcdr-policy.md)

Establishes governance, roles, and recovery procedures for the BCMS. Recovery objectives in this policy trace directly back to the BIA rather than being set independently.

**Key design decisions:**
- RTO and RPO targets are tiered by process class, not set uniformly. Applying the same recovery objective to all processes regardless of criticality wastes resource on low-impact processes and under-invests in critical ones.
- AI system availability is treated as a distinct continuity risk at Phase 2. AI system failure modes (model degradation, LLM API outage) differ from general IT outage, and fallback processes require human decision-making guidance rather than just IT failover procedures. PCM-001 and CRT-001 each have documented fallback procedures in the Phase 2 programme.
- BC/DR testing is a scheduled governance obligation, not optional. Test results are reviewed by the Risk Management Committee.

**Frameworks:** ISO 22301:2019 (Clauses 4-10), NIST SP 800-34 Rev. 1, BCI Good Practice Guidelines

---

## How the Programme Connects to the Broader Framework

The BC/DR Policy derives authority from the Information Security Policy and operates within the risk appetite thresholds defined in the Risk Management Policy. Recovery objectives that fall outside risk appetite thresholds require Risk Management Committee review.

The Incident Management Policy governs the first response to an event. The BC/DR programme governs what happens after initial containment, when the question shifts from "what happened" to "how do we keep operating and when do we recover."

At Phase 2, the AI Governance Policy adds requirements for AI system continuity: fallback procedures for High-Risk system unavailability and human oversight requirements during model-assisted process degradation.

---

## Frameworks Applied

| Framework | Application |
|---|---|
| ISO 22301:2019 | BCMS governance, BIA methodology, recovery planning, testing |
| NIST SP 800-34 Rev. 1 | Contingency planning guidance; RTO/RPO determination |
| BCI Good Practice Guidelines | BIA methodology and exercise programme design |
| ISO/IEC 27031:2011 | IT disaster recovery and resilience alignment |

---

## Related Documentation

| Document | Description |
|---|---|
| [Emyzer Technology Overview](../emyzer-technology/README.md) | Phase 1 programme context |
| [Risk Management Policy](../policies/risk-management-policy.md) | Risk appetite thresholds that BC recovery objectives are calibrated against |
| [Incident Management Policy](../policies/incident-management-policy.md) | First-response governance that precedes BC/DR activation |
| [AI Governance Policy](../enterprise-policies/ai-governance-policy.md) | Phase 2 extension: AI system continuity and fallback procedures |
| [Portfolio Overview](../README.md) | Top-level narrative and 60-second review path |

---

*All content in this portfolio is a fictional case study. Framework and regulatory references are accurate as of the document publication dates.*

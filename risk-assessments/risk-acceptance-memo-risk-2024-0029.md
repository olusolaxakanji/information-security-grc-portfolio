# Risk Acceptance Memorandum

**Risk ID:** RISK-2024-0029
**Risk Title:** Physical Security of Server Room — Single-Factor Access Control
**Asset:** On-Premises Data Center
**Memorandum Date:** 2024-03-15
**Risk Rating at Acceptance:** 6 — Medium
**Treatment Decision:** Accept (with compensating controls)

---

## Purpose

This memorandum formally documents the decision to accept the residual risk associated with single-factor badge-only access control at Emyzer Technology's on-premises server room. It records the business rationale for rejecting the proposed control, the compensating measures implemented in lieu of full remediation, the conditions under which this acceptance will be reassessed, and the authority under which the decision is made.

This memo is the completion record for the treatment action in RISK-2024-0029 in the Asset Risk Register. It satisfies the formal acceptance documentation requirements in the Risk Management Policy (Section 5.3): risks accepted rather than mitigated require a written record of rationale, compensating controls, and review conditions before the acceptance status is recorded in the register.

---

## Risk Summary

| Field | Detail |
|---|---|
| **Asset** | On-Premises Data Center — server room, Building A, Level B1 |
| **Risk scenario** | Unauthorized physical access via tailgating or compromised badge credentials, enabling equipment theft, tampering, or sabotage of production systems |
| **Threat source** | Adversarial: insider or external intruder; Accidental: tailgating by authorized personnel |
| **Vulnerability** | Single-factor badge-only access; no anti-tailgate mechanism; no biometric verification |
| **Inherent risk rating** | 8 — Medium (Likelihood 2 × Impact 4) |
| **Existing controls at assessment** | Badge access control system; visitor sign-in log; security camera coverage with 30-day footage retention |
| **Residual risk rating** | 6 — Medium (Likelihood 2 × Impact 3; impact reduced by camera deterrence and access logging) |
| **Risk owner** | Director of IT Operations |

---

## Proposed Control Evaluated and Rejected

**Control evaluated:** Biometric access control system (fingerprint scanner integrated with existing badge infrastructure)

**Estimated cost:**
- Hardware and installation: $45,000
- Annual maintenance and licensing: $6,000
- Total 3-year cost of ownership: $63,000

**Reason for rejection:**

The cost of biometric implementation does not produce a proportionate risk reduction given the planned decommission of the on-premises data center.

Emyzer Technology has approved a phased migration of production systems to AWS cloud infrastructure, targeting completion by December 2025. The on-premises server room will be decommissioned as production workloads migrate. Investing $45,000 in physical access controls for a facility with an 18-month operational runway does not represent a sound allocation of risk budget.

The residual risk is Medium, not High or Critical. No physical security incident involving the server room has been recorded in the past 24 months. The badge access system, visitor log, and camera coverage provide a reasonable deterrence posture for a facility in planned decommission. The risk does not meet the threshold requiring treatment regardless of cost (as defined in the Risk Appetite Statement, Section 3.2: unacceptable conditions requiring treatment apply to Critical and High risks with no compensating controls; Medium risks may be accepted with documented rationale and compensating measures).

**Alternative considered:** Increasing camera coverage to 24-hour monitoring with motion-triggered alerts. Evaluated and also rejected: cost ($8,000 installation plus $1,200/year monitoring) was considered disproportionate to a Medium-rated risk with no incident history and an impending decommission timeline.

---

## Compensating Controls Implemented

Two compensating measures were implemented at the time of this decision to reduce residual exposure without full biometric remediation:

| Control | Description | Owner | Effective Date |
|---|---|---|---|
| Extended camera footage retention | Server room camera retention extended from 30 days to 90 days. The extended retention window provides a longer investigative baseline in the event of a physical security incident and increases deterrence for insider threats. | Facilities Manager | 2024-03-15 |
| Quarterly physical access list review | Physical access badge list reviewed and certified by the Director of IT Operations each quarter. Access removed for any departed or role-changed personnel within 48 hours of notification. Review results documented and filed with the GRC team. | Director of IT Operations | 2024-03-15 |

These controls do not eliminate the single-factor vulnerability. They reduce the residual likelihood of undetected unauthorized access and strengthen the investigative capability available after any incident.

---

## Conditions for Reassessment

This acceptance is conditional. The risk will be returned to active treatment and this memo will be reviewed if any of the following conditions occur before the server room is decommissioned:

| Trigger | Description |
|---|---|
| Migration delay | The cloud migration timeline extends beyond December 2025, materially increasing the remaining operational life of the server room |
| Physical security incident | Any physical security incident, attempted unauthorized access, or near-miss occurs at or near the server room |
| Risk rating change | The residual risk rating is reassessed and moves from Medium to High or Critical |
| Asset sensitivity change | Any change in the classification or sensitivity of systems or data held in the server room |
| Annual review | Scheduled for March 2025 regardless of the above |

---

## Risk Register Update

Upon execution of this memo, the Asset Risk Register entry for RISK-2024-0029 will be updated as follows:

- **Treatment Strategy:** Accept
- **Treatment Status:** Accepted
- **Comments:** See Risk Acceptance Memorandum dated 2024-03-15. Biometric control rejected: $45K cost disproportionate given planned cloud migration timeline (decommission target December 2025). Compensating controls implemented: 90-day camera retention, quarterly access list review. Reassessment triggered if migration extends beyond 2025.

---

## Acceptance Decision

Having reviewed the risk description, the proposed control and its estimated cost, the business rationale for rejection, and the compensating measures in place, the accepting authority concludes that the residual risk of Medium (score 6) is within the organization's risk tolerance for physical security risks under the conditions documented above.

The risk is formally accepted. It will be monitored at the standard Medium-risk cadence (review date: 2025-03-15) and escalated immediately if any reassessment trigger defined above is met.

| Role | Name | Date |
|---|---|---|
| Risk Owner | Director of IT Operations | 2024-03-15 |
| Reviewing Authority | IT Security Manager | 2024-03-15 |
| GRC Analyst | GRC Team | 2024-03-15 |

---

## Document Control

| Version | Date | Author | Notes |
|---|---|---|---|
| 1.0 | 2024-03-15 | GRC Team | Initial acceptance memo |

**Linked documents:**
- Asset Risk Register — RISK-2024-0029
- Risk Assessment Methodology
- Risk Appetite Statement — Section 3.2 (Physical Security tolerance thresholds)
- Risk Management Policy — Section 5.3 (Risk acceptance documentation requirements)

*Retention: 7 years from acceptance date, or until the risk is formally closed following server room decommission, whichever is later.*

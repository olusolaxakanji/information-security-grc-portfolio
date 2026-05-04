# Policy Exception Record: Template

---

## Template Metadata

| Field               | Value                                                                                        |
|---------------------|----------------------------------------------------------------------------------------------|
| Template ID         | TMPL-EX-001                                                                                  |
| Version             | 1.0                                                                                          |
| Status              | Active                                                                                       |
| Purpose             | Document policy exception requests, approvals, compensating controls, and remediation plans  |
| Owner               | ISO / GRC Team                                                                               |
| Approved By         | CISO                                                                                         |
| Review Frequency    | Annual                                                                                       |
| GitHub Reference    | https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/templates/exception-record-v1.md |

---

## Instructions for Use

**What is a policy exception?**
A policy exception is a formally documented and approved temporary deviation from a specific requirement in an approved GRC policy. An exception acknowledges that the organisation is not currently meeting a stated control requirement and provides a structured, time-limited framework for managing the residual risk during the period of non-compliance.

An exception is NOT the same as:
- A **policy gap**: where the policy has not yet been written or does not address a particular scenario. Gaps are addressed through policy development, not exception requests.
- A **permanent policy change**: if a requirement is no longer appropriate, the policy should be formally amended through the policy review process, not bypassed indefinitely via exceptions.
- A **finding**: a finding is raised when a control is discovered to have failed or been deficient. An exception is prospective: it is requested before the deviation occurs, or immediately upon discovery before remediation is possible. If a control failure is discovered retrospectively and cannot be immediately remediated, raise a finding AND an exception to cover the period until remediation is complete.

**Who can request an exception**
Any department head, system owner, or risk owner may submit an exception request. The requestor is responsible for completing Sections 1–5 of this template and submitting it to the ISO for review. Requestors must not self-approve exceptions.

**Who can approve an exception**
- The ISO conducts the initial review and recommends approval or rejection.
- The CISO is the approval authority for all exceptions.
- Where the exception involves a regulatory obligation (e.g., a requirement under data protection law, a certification requirement), Legal Counsel must also review before approval.
- Where the residual risk of the exception exceeds the organisation's defined risk appetite, the CRO must co-approve.

**Maximum exception duration**
Exceptions are time-limited. The default maximum duration is **90 days**. Extensions require a new exception request or a documented renewal approved by the CISO. Exceptions may not be renewed more than twice without a formal review by the CISO and CRO and escalation to the board or risk committee. Indefinite exceptions are not permitted.

**Consequences of non-approval**
Where an exception request is rejected, the requestor must bring the relevant system, process, or activity into compliance with the policy before it proceeds. The ISO will assess whether a temporary compensating control can bridge the gap while remediation occurs. If no path to compliance is available within a reasonable timeframe, the matter must be escalated to the CISO and documented as an accepted risk with board-level visibility.

**Numbering convention**
Exception IDs follow the format EX-YYYY-NNNN (e.g., EX-2025-0004). Assigned sequentially by the GRC team.

---

## Section 1: Exception Request

| Field                              | Detail                                                                                    |
|------------------------------------|-------------------------------------------------------------------------------------------|
| Exception ID                       | [EX-YYYY-NNNN]                                                                            |
| Policy Reference                   | [Policy name, specific section and clause, version, e.g., Access Control Policy v2.1, Section 5.2, Multi-Factor Authentication Requirement] |
| Specific Requirement Being Excepted | [Quote or summarise the precise policy requirement from which the exception is sought]   |
| Exception Type                     | [Select one: Temporary Operational / Technical Limitation / Transitional / Business Justification] |
| Requestor                          | [Full name, Role, Department]                                                             |
| Request Date                       | [YYYY-MM-DD]                                                                              |
| Proposed Exception Start Date      | [YYYY-MM-DD]                                                                              |
| Proposed Exception End Date        | [YYYY-MM-DD: maximum 90 days from start date unless extended with CISO approval]        |
| Total Proposed Duration            | [N days / N weeks]                                                                        |
| Systems / Processes Affected       | [List all systems, applications, processes, or services to which the exception applies. Be specific: do not use "all systems" without justification.] |
| Affected Users / Data              | [Define the scope: which user groups, data types, data subjects, or data volumes are affected by the exception] |
| Data Classification of Affected Data | [e.g., Restricted / Confidential / Internal / Public: per Data Classification Policy] |

*Exception Types defined:*
- *Temporary Operational: a short-term operational necessity (e.g., patching window, system migration, emergency response)*
- *Technical Limitation: the policy requirement cannot be implemented due to a technical constraint of the affected system or vendor*
- *Transitional: the organisation is in the process of implementing the required control but it is not yet fully deployed*
- *Business Justification: compliance with the policy as written would create a disproportionate business impact; alternative safeguards are in place*

---

## Section 2: Business Justification

*Explain clearly and specifically why compliance with the policy requirement as written is not feasible during the proposed exception period. State the business impact of enforcing the policy requirement without the exception. Acceptable justifications include: regulatory or contractual obligation that conflicts with the policy requirement, documented technical limitation of a specific system, or time-bounded transitional necessity with a credible remediation plan. "It would be inconvenient," "it is complex," or "we have not had time to implement it" are not acceptable justifications on their own. If a technical limitation is the basis, include supporting technical documentation or reference.*

**Why compliance is not currently feasible:**
[Provide a specific, factual explanation. Include relevant dates, system names, constraints, and any external dependencies.]

**Business impact of not granting the exception:**
[What operational, contractual, or regulatory consequence would result from enforcing the policy requirement without the exception? Quantify where possible.]

**Why the proposed duration is the minimum necessary:**
[Explain why the exception cannot be shorter. What activities need to happen during this period? What is the earliest feasible date for compliance?]

---

## Section 3: Risk Assessment

| Field                                     | Detail                                                                                   |
|-------------------------------------------|------------------------------------------------------------------------------------------|
| Threat Scenario                           | [What specific threat or failure scenario could occur if the policy requirement is not met during the exception period?] |
| Likelihood (with compensating controls)   | [1–5 scale: 1 = Remote, 2 = Unlikely, 3 = Possible, 4 = Likely, 5 = Almost Certain]    |
| Impact (if threat materialises)           | [1–5 scale: 1 = Negligible, 2 = Minor, 3 = Moderate, 4 = Major, 5 = Catastrophic]      |
| Residual Risk Score                       | [Likelihood × Impact = Score: e.g., 3 × 4 = 12]                                        |
| Residual Risk Level                       | [Low (1–4) / Medium (5–9) / High (10–19) / Critical (20–25)]                            |
| Risk Description                          | [Narrative description of what could go wrong during the exception period and its potential consequence for the organisation, its data subjects, and its regulatory standing.] |
| Risk Owner                                | [Name, Role: the person accountable for managing the risk during the exception period] |
| Exceeds Organisational Risk Appetite?     | [Yes / No: if Yes, CRO co-approval is mandatory per Section 6]                         |
| Risk Appetite Reference                   | [Reference the relevant risk appetite statement from the Risk Management Framework]      |

---

## Section 4: Compensating Controls

*A compensating control is an alternative safeguard that reduces the risk created by the policy deviation to an acceptable level during the exception period. At least one compensating control is required for any exception to be approved. An exception cannot be approved without compensating controls unless the residual risk is explicitly accepted by the CISO. Where the CISO accepts risk without compensating controls, document the rationale in Section 6.*

*Each compensating control must be specific, verifiable, and directly address the risk identified in Section 3. "Increased vigilance" or "monitoring the situation" are not acceptable compensating controls without specific, measurable parameters.*

| Control                | Description                                     | Owner              | Implementation Date | Effectiveness Assessment                    |
|------------------------|-------------------------------------------------|--------------------|---------------------|---------------------------------------------|
| [Control name]         | [Specific description of what the control does and how it addresses the residual risk] | [Name, Role] | [YYYY-MM-DD] | [How will you verify the control is operating effectively? What evidence will be collected?] |
| [Control name]         | [Specific description]                          | [Name, Role]       | [YYYY-MM-DD]        | [Verification method and evidence]          |
| [Control name]         | [Specific description]                          | [Name, Role]       | [YYYY-MM-DD]        | [Verification method and evidence]          |

*If compensating controls are not feasible, state the reason here and note that CISO explicit risk acceptance is required:*
[N/A, compensating controls are in place as above / Compensating controls not feasible because: [reason], CISO risk acceptance required]

---

## Section 5: Remediation Plan

*The remediation plan describes the specific steps that will bring the affected system, process, or activity into compliance with the policy requirement. The plan must be realistic, include specific milestone dates, and identify responsible owners. The remediation plan must demonstrate that the exception period is genuinely temporary and that compliance will be achieved by the exception end date.*

*If the remediation plan cannot deliver compliance by the exception end date, the requestor must seek an extension before the exception expires: not retrospectively.*

| Milestone                          | Description                                   | Owner              | Target Date  | Status              |
|------------------------------------|-----------------------------------------------|--------------------|--------------|---------------------|
| [Milestone 1: e.g., Procurement]  | [Specific activity or deliverable]            | [Name, Role]       | [YYYY-MM-DD] | [Not Started / In Progress / Complete] |
| [Milestone 2: e.g., Implementation] | [Specific activity or deliverable]          | [Name, Role]       | [YYYY-MM-DD] | [Not Started / In Progress / Complete] |
| [Milestone 3: e.g., Testing]      | [Specific activity or deliverable]            | [Name, Role]       | [YYYY-MM-DD] | [Not Started / In Progress / Complete] |
| [Milestone 4: e.g., Go-Live / Compliance Confirmed] | [Specific activity or deliverable] | [Name, Role] | [YYYY-MM-DD] | [Not Started / In Progress / Complete] |

**Full compliance target date:** [YYYY-MM-DD: must be on or before exception end date]
**Remediation owner:** [Name, Role: accountable for delivering the remediation plan]

---

## Section 6: Approval Chain

*Complete each row in the order listed. No later approver should sign before the earlier review is complete. Where a role is not required (e.g., CRO is not required if risk does not exceed appetite), mark as "N/A: not required because [reason]." Do not leave rows blank.*

| Role                  | Name                       | Decision                        | Date         | Comments                                       |
|-----------------------|----------------------------|---------------------------------|--------------|------------------------------------------------|
| ISO (first review)    | [Name]                     | [Recommend Approval / Recommend Rejection / Recommend Approval with Additional Conditions] | [YYYY-MM-DD] | [ISO's assessment and any conditions or concerns] |
| CISO (approval authority) | [Name]                 | [Approved / Rejected / Approved with Conditions / Deferred] | [YYYY-MM-DD] | [CISO's rationale; any additional conditions imposed] |
| CRO (co-approval if risk exceeds appetite) | [Name or N/A] | [Co-Approved / Rejected / N/A: risk within appetite] | [YYYY-MM-DD] | [CRO's risk assessment comment] |
| Legal Counsel (if regulatory obligation implicated) | [Name or N/A] | [No legal objection / Legal objection raised, see notes / N/A, no regulatory obligation affected] | [YYYY-MM-DD] | [Legal Counsel's assessment of regulatory exposure] |

**Final Decision:** [APPROVED / APPROVED WITH CONDITIONS / REJECTED]
**Exception Valid From:** [YYYY-MM-DD]
**Exception Expires:** [YYYY-MM-DD]
**Conditions attached to approval (if any):**
[List each condition. The ISO is responsible for tracking conditions to closure. Unresolved conditions at the exception end date may result in the exception lapsing.]

---

## Section 7: Monitoring During Exception Period

*Describe how the GRC team and the risk owner will verify that the compensating controls defined in Section 4 remain in operation throughout the exception period. Monitoring must be active: it is not sufficient to assume controls are working without verification. Define the frequency of monitoring, what specifically will be checked, and who is responsible.*

**Monitoring activities:**
[Describe each monitoring activity: e.g., weekly review of access logs; fortnightly check-in between ISO and risk owner; automated alerting on the relevant control failure scenario]

**Monitoring frequency:** [e.g., Weekly / Fortnightly / Monthly]
**Monitoring owner:** [Name, Role]
**Escalation trigger:** [Define the condition under which the exception would be immediately escalated or revoked: e.g., compensating control fails; affected system experiences a security incident; scope of exception expands beyond what was approved]
**Monitoring evidence record location:** [Where will evidence of monitoring activity be stored?]

---

## Section 8: Exception Closure

*Complete this section when the exception is closed. The closure must be documented regardless of how the exception is resolved: whether the underlying issue has been remediated (and the exception is no longer required), the exception has been extended, or the risk has been formally accepted as a permanent deviation (which requires a separate risk acceptance record).*

| Field                      | Detail                                                                                    |
|----------------------------|-------------------------------------------------------------------------------------------|
| Closure Date               | [YYYY-MM-DD]                                                                              |
| Closure Type               | [Resolved, policy compliance achieved / Extended, new exception EX-YYYY-NNNN raised / Risk Accepted, formal risk acceptance record raised] |
| Evidence of Compliance (if Resolved) | [Reference the evidence that demonstrates the policy requirement is now being met: e.g., Control testing record CTR-2025-NNNN confirming MFA is operational on all affected accounts] |
| Closing Authority          | [Name, Role, Date: the person who certifies the exception is closed]                    |
| Lessons Learned            | [What would have prevented the need for this exception? Are any process changes or control improvements recommended to avoid similar exceptions?] |

---

## Appendix: Exception Approval Matrix

*This matrix defines the minimum required approvers based on exception type and residual risk level. The CISO may require additional approvals at their discretion. All exceptions require ISO review regardless of type or risk level.*

| Exception Type              | Residual Risk: Low | Residual Risk: Medium | Residual Risk: High | Residual Risk: Critical |
|-----------------------------|--------------------|-----------------------|---------------------|-------------------------|
| Temporary Operational       | ISO + CISO         | ISO + CISO            | ISO + CISO + CRO    | ISO + CISO + CRO + Board Notification |
| Technical Limitation        | ISO + CISO         | ISO + CISO            | ISO + CISO + CRO    | ISO + CISO + CRO + Board Notification |
| Transitional                | ISO + CISO         | ISO + CISO + CRO      | ISO + CISO + CRO    | ISO + CISO + CRO + Board Notification |
| Business Justification      | ISO + CISO         | ISO + CISO + CRO      | ISO + CISO + CRO + Legal | ISO + CISO + CRO + Legal + Board Approval |
| Any (regulatory obligation implicated) | ISO + CISO + Legal | ISO + CISO + Legal | ISO + CISO + CRO + Legal | ISO + CISO + CRO + Legal + Board Approval |

*Board Notification: The CISO must notify the board or its delegated risk committee at the next regular meeting and include the exception in the Quarterly GRC Board Report.*
*Board Approval: The board or its delegated risk committee must formally approve the exception before it becomes effective.*

---

*End of Template TMPL-EX-001 v1.0. Remove all guidance text (italicised instructions) before distributing a completed Exception Record. The completed record must be stored in the GRC platform and referenced in the exception register.*

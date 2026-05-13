# ServiceNow Evidence Exports

**Emyzer Technology: Phase 1 | Fictional case study.**

---

## What This Directory Proves

Polished markdown documents tell a reader what the policies say. Raw platform exports prove the policies exist inside a GRC system with proper governance controls applied.

These five PDFs are direct exports from ServiceNow GRC's Policy and Compliance module. They were not formatted for presentation. They are exactly what ServiceNow generates when you manage policies correctly: system-generated timestamps, approval metadata, ownership records, compliance mappings, and version history as the platform produces them.

The difference between a policy document and a ServiceNow export is the difference between writing a policy and implementing one.

---

## What the Exports Capture

Each PDF contains:

- **Policy metadata:** Name, type, version, knowledge base reference, compliance score
- **Ownership:** Named policy owner, named approver, review cycle, validity dates
- **Approval workflow:** Who approved, when, and their documented comments
- **Framework alignment:** Which controls and standards the policy maps to in the platform
- **Related lists:** Connected controls, evidence requirements, linked documents

---

## File Inventory

| Export | What it shows | Linked Policy |
|---|---|---|
| [Access Control Policy.pdf](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/servicenow-evidence/Access%20Control%20Policy.pdf) | RBAC/ABAC implementation, quarterly access review controls, privileged access governance | [Access Control Policy](../policies/access-control-policy.md) |
| [Business Continuity and DR Policy.pdf](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/servicenow-evidence/Business%20Continuity%20and%20Disaster%20Recovery%20Policy.pdf) | BCMS governance structure, ISO 22301 alignment, recovery objective framework | [BC/DR Policy](../policies/bcdr-policy.md) |
| [Incident Management Policy.pdf](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/servicenow-evidence/Incident%20Management%20Policy.pdf) | IRT activation criteria, GDPR 72-hour notification path, severity classification framework | [Incident Management Policy](../policies/incident-management-policy.md) |
| [Information Security Policy.pdf](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/servicenow-evidence/Information%20Security%20Policy.pdf) | ISMS parent policy: Security Steering Committee, exception governance, review cadence | [Information Security Policy](../policies/information-security-policy.md) |
| [Risk Management Policy.pdf](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/servicenow-evidence/Risk%20Management%20Policy.pdf) | 5x5 risk methodology, materiality thresholds, Risk Management Committee authority | [Risk Management Policy](../policies/risk-management-policy.md) |

---

## How to Read a ServiceNow Export

ServiceNow policy exports follow a consistent structure:

1. **Header block:** Report metadata including run date and administrator
2. **Policy details:** Name, type, ownership, compliance score, parent policy linkage
3. **Policy text:** The full governance language: purpose, scope, definitions, procedures
4. **Approval records:** Approver names, timestamps, and comments
5. **Related lists:** Connected controls, evidence requirements, version history

No formatting has been applied after export. What you see is what ServiceNow produces.

---

## Related Documentation

| Document | Description |
|---|---|
| [Controls Library](../controls/README.md) | The operational controls that run against these policies |
| [Emyzer Technology Overview](../emyzer-technology/README.md) | Phase 1 programme context |
| [Portfolio Overview](../README.md) | Top-level narrative and 60-second review path |

---

*All content in this portfolio is a fictional case study.*

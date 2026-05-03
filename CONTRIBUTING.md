# Contributing to the GRC Portfolio

This document defines how changes are proposed, reviewed, approved, and merged into the Emyzer Nexus GRC repository. The programme spans three entities: Emyzer Nexus (parent), Emyzer Technology (subsidiary), and Veridian AI (acquired). This process applies to documentation across all three.

> **Simulated Programme Note:** This is a fictional portfolio. Approval here means changes are reviewed for quality, accuracy, and internal consistency before merging. The governance model reflects how a real multi-entity GRC programme operates. It is applied here to maintain documentation discipline and show how decisions get made.

---

## Roles and Ownership

| Role | Responsibility |
|---|---|
| **CISO** | Owns the ISMS and AI Governance programme; final approver on all security policies, AI governance policies, and changes to the policy hierarchy |
| **CRO** | Owns the enterprise risk management and business continuity programmes; final approver on risk register entries, risk appetite changes, and BC/DR documentation |
| **DPO** | Owns the privacy and data protection programme; final approver on privacy policy changes and DPIA governance documentation |
| **CTO** | Owns the change management and vulnerability management policies; primary reviewer for technical governance documents |
| **ISO** | Operational owner of the ISMS; primary drafter and reviewer of Phase 1 security policy documents |
| **GRC Analyst** | Primary reviewer for all policy, template, and compliance mapping documents; responsible for policy register currency and cross-reference accuracy |
| **Business Continuity Manager** | Reviewer for BC/DR documentation; owns the Business Impact Analysis and tabletop exercise records |
| **AI Governance Committee** | Collective approver for AI system inventory changes, EU AI Act control mapping updates, and Veridian AI risk assessment revisions |
| **External Reviewer / Portfolio Evaluator** | Read-only access; no merge authority |

---

## Review Cadence

### Continuous (on every change)

- All edits are made on a feature branch and submitted as a pull request.
- PR title format: `[type] short description` where type is one of `policy`, `risk`, `ai-governance`, `integration`, `bcdr`, `template`, `evidence`, `compliance-mapping`, or `report`.
- At least one reviewer must approve before merging. Changes to policies or the risk register require the relevant programme owner (CISO, CRO, or DPO) as one of the approvers.
- Changes to AI system classifications, EU AI Act mappings, or Veridian AI risk assessments require AI Governance Committee review.

### Monthly

- **Risk register triage:** CRO reviews any risks rated `Critical` or `High` and confirms that residual ratings and treatment status are current.
- **Evidence freshness check:** GRC Analyst spot-checks that evidence referenced in published policies has been updated in line with each document's defined review cadence.
- **Cross-reference integrity check:** Confirm that inter-policy references (particularly between the AI Governance Policy, Model Risk Policy, Incident Management Policy, and Change Management Policy) remain consistent with the current document versions.

### Quarterly

- **Risk register refresh:** All risk owners review and attest to their entries. Ratings are updated if circumstances or treatment status have changed. Risk appetite thresholds are compared against current posture.
- **Business continuity review:** Business Continuity Manager confirms that RTO/RPO targets in the BC/DR Policy remain aligned with the current Business Impact Analysis findings.
- **AI Governance Committee meeting:** Committee reviews the AI system inventory, any material changes to High-Risk AI systems, EU AI Act regulatory developments, and Veridian AI remediation progress against the Policy Rationalization Roadmap.
- **Portfolio compliance report:** Summary of documentation currency, open planned items, and any framework updates affecting published policies. Drafted by GRC Analyst.

### Annually

- **Full policy review:** Every policy in `policies/` and `enterprise-policies/` is reviewed for continued accuracy against current frameworks and the simulated organisational scenario. Policies not materially changed are re-dated and re-attested. Policies requiring amendment go through the standard PR process.
- **EU AI Act regulatory developments review:** CISO and AI Governance Committee assess any EU AI Act implementing acts, delegated regulations, or Commission guidance published during the year and determine whether they require updates to the AI Governance Policy, EU AI Act Control Mapping, or AI System Inventory.
- **Business Impact Analysis refresh:** Business Continuity Manager assesses whether the BIA findings remain valid. Material changes to critical process RTOs, RPOs, or financial exposure estimates are updated via PR.
- **Control framework review:** GRC Analyst compares the framework coverage matrix in each programme area against the latest published versions of ISO 27001, NIST CSF, NIST AI RMF, and other referenced standards. New obligations are noted; retired guidance is archived with an explanatory note.
- **Full GRC programme retrospective:** Assesses programme completeness (published vs. planned artefacts), documentation quality, and whether the portfolio accurately represents the skills and governance competencies it is intended to demonstrate. This CONTRIBUTING.md is updated if process changes are needed.

---

## Branch and Commit Conventions

- Branch names: `type/short-slug`. Examples: `policy/nexus-privacy-gdpr-update`, `risk/emyzer-tech-q3-register`, `ai-governance/eu-ai-act-system-inventory`, `integration/veridian-rationalization-roadmap`.
- Commit messages: imperative mood, ≤72 characters on the first line. Examples: `Add EU AI Act Article 9 control mapping for churn model`, `Publish Privacy and Data Protection Policy v1.0`, `Update Veridian AI risk assessment — Tier 1 classification rationale`.
- Do not commit personally identifiable information, API keys, or credentials. This is a public portfolio repository.
- ServiceNow evidence exports (PDFs) are committed to `servicenow-evidence/` only. Raw exports from other platforms are not committed without a corresponding README entry explaining their provenance.

---

## Archiving vs. Deleting

Records must never be hard-deleted from `main`. Instead:

- Superseded policies are moved to `policies/archive/` or `enterprise-policies/archive/` with a note in the file header referencing the replacement document and the date of supersession.
- Resolved or accepted risks are moved to `risk-assessments/archive/` with their final treatment status and closure date recorded.
- Veridian AI original documentation (however incomplete) is retained permanently in its designated folder as part of the acquisition record. Governance integration does not erase evidence of the inherited state.
- Outdated templates are retained under their version number (e.g., `policy-v1.md`) when a new version is published. The templates README is updated to point to the latest version; old versions remain for reference.

Retention periods follow ISO 27001:2022 Annex A and GDPR Article 5(1)(e) storage limitation principles (generally 7 years for governance records) as the binding standards for the simulated programme.

---

## Questions

Raise questions about document structure, framework alignment, or portfolio design by opening a GitHub Issue. For suggestions on the fictional scenario or organisational context, open an Issue with the label `scenario-design`.

# Business Continuity Plan (BCP)

**Emyzer Technology – Business Continuity Management System**

---

## Document Metadata

| Attribute | Details |
|-----------|---------|
| **Document Title** | Business Continuity Plan |
| **Document ID** | BC-PLAN-001 |
| **Version** | 1.0 |
| **Effective Date** | 2024-09-01 |
| **Review Date** | 2025-09-01 |
| **Classification** | Restricted — Distribution Limited to Crisis Management Team and Named Alternates |
| **Owner** | Business Continuity Manager (Susan Orwell) |
| **Approved By** | Chief Executive Officer |
| **Framework Alignment** | [ISO 22301:2019](https://www.iso.org/standard/75106.html) [VERIFY], [NIST SP 800-34 Rev. 1](https://csrc.nist.gov/publications/detail/sp/800-34/rev-1/final) [VERIFY] |
| **Parent Policy** | Business Continuity and Disaster Recovery Policy (KB-PORTFOLIO-0006) |
| **Linked Documents** | BIA Report, Asset Risk Register, Incident Management Policy, Data Classification Policy |

> **RESTRICTED DOCUMENT.** This plan contains operational recovery procedures and crisis contact information. It is classified Restricted and must not be shared outside the Crisis Management Team and named alternates without the express written approval of the Business Continuity Manager.

---

## Table of Contents

1. [Purpose and Scope](#1-purpose-and-scope)
2. [Activation Criteria](#2-activation-criteria)
3. [Recovery Objectives](#3-recovery-objectives)
4. [Crisis Management Team](#4-crisis-management-team)
5. [Communication Plan](#5-communication-plan)
6. [Recovery Strategies by Disruption Type](#6-recovery-strategies-by-disruption-type)
7. [Recovery Procedures by Tier](#7-recovery-procedures-by-tier)
8. [IT Recovery Procedures](#8-it-recovery-procedures)
9. [Testing and Exercising](#9-testing-and-exercising)
10. [Plan Maintenance](#10-plan-maintenance)
11. [Framework Alignment](#11-framework-alignment)
12. [Related Documents](#12-related-documents)
13. [Evidence Index](#13-evidence-index)
14. [Approval History](#14-approval-history)

---

## 1. Purpose and Scope

### 1.1 Purpose

This Business Continuity Plan (BCP) operationalises Emyzer Technology's business continuity capability in response to disruptive incidents affecting its people, technology, premises, and supply chain. It translates the strategic commitments of the Business Continuity and Disaster Recovery Policy (BC/DR Policy) into actionable, tested procedures for use by the Crisis Management Team (CMT) and designated recovery owners during an incident.

This plan is aligned to ISO 22301:2019 Clause 8.3 [VERIFY] (Business continuity strategy and solutions) and Clause 8.4 [VERIFY] (Business continuity plans and procedures), and draws its recovery objective inputs from the Business Impact Analysis (BIA) Report (BC-BIA-001, effective 2024-05-22).

The plan serves three primary functions:

1. **Activation guide** — provides structured criteria and authority for declaring a business continuity incident and activating the CMT.
2. **Operational playbook** — provides numbered, step-by-step recovery procedures for each business function tier, enabling execution under pressure without reliance on institutional memory.
3. **Governance record** — documents the testing regime, maintenance cycle, and evidence requirements necessary to demonstrate ongoing ISO 22301 compliance.

### 1.2 Scope

This plan applies to all critical and essential business processes across all Emyzer Technology operational regions, spanning Asia Pacific, the Americas, Europe, the Middle East, and Africa. It covers disruptions to:

- **Technology** — including cloud infrastructure, enterprise applications, end-user computing, and network services;
- **People** — including simultaneous unavailability of key personnel, public health incidents, and industrial action;
- **Premises** — including loss of or inaccessibility to office facilities, data centres, and manufacturing sites;
- **Suppliers** — including failure of Tier 1 suppliers whose unavailability would directly impair a Tier 1 or Tier 2 business function.

This plan does not replace departmental recovery plans (referenced in Annexes A through D) but takes precedence over them during a declared incident. Disaster recovery (DR) procedures for IT infrastructure are detailed in Section 8 and the separate IT Disaster Recovery Runbooks held by the IT Recovery Lead.

**Out of scope:** Individual project-level continuity planning; personal data breach response (governed by Incident Management Policy); and Emyzer Nexus / Veridian AI entity continuity (to be addressed in Phase 2 documentation).

### 1.3 Plan Activation

This plan is activated by the Business Continuity Manager (Susan Orwell) or a designated alternate (see Section 4). Once activated, this plan supersedes normal operating procedures for the affected functions. Activation does not require CEO approval but the CEO (Incident Commander) must be notified within the timeframes specified in Section 2.

The BC Manager holds sole authority to deactivate the plan and declare recovery complete. Deactivation requires written confirmation that all affected Tier 1 functions have returned to normal operational status.

---

## 2. Activation Criteria

The following thresholds define the conditions under which this plan is activated. Activation does not require all conditions to be met; any single condition meeting or exceeding its threshold is sufficient for activation.

| # | Disruption Type | Activation Threshold | Activating Authority | CMT Notification Within |
|---|-----------------|---------------------|---------------------|-------------------------|
| 1 | IT / System Outage | Critical system (Tier 1 or Tier 2) unavailable for more than 2 consecutive hours, or outage projected to exceed 2 hours | BC Manager | 30 minutes of threshold breach |
| 2 | Premises Loss | Office, facility, or data centre inaccessible or rendered unsafe by any cause | BC Manager | 1 hour of confirmed inaccessibility |
| 3 | Cyber Incident | Confirmed security breach, ransomware deployment, or data exfiltration event affecting production systems | CISO and BC Manager (joint activation) | Immediately upon confirmation |
| 4 | Key Person Unavailability | Simultaneous unavailability of 3 or more members of the Executive Leadership Team | CEO (or next available executive) | 2 hours |
| 5 | Supplier Failure | Tier 1 supplier unable to deliver contracted services or components for more than 24 consecutive hours | BC Manager | 4 hours of confirmed failure |
| 6 | Natural Disaster / Force Majeure | Any natural disaster, civil unrest, pandemic escalation, or force majeure event affecting one or more operational regions | BC Manager | Immediately upon risk assessment |
| 7 | Regulatory Direction | Regulatory authority or law enforcement directive requiring operational suspension or restriction | Legal Counsel and BC Manager (joint notification) | Immediately upon receipt |

**Pre-activation monitoring:** The BC Manager and IT Recovery Lead maintain situational awareness through the ServiceNow Major Incident process and the NOC/SOC monitoring dashboards. Where a situation is developing but has not yet reached the activation threshold, the BC Manager may declare a **Standby Alert**, placing the CMT on 30-minute readiness without formal activation.

**Escalation during activation:** If the BC Manager is unavailable, the IT Recovery Lead or COO may activate in their place. The BC Manager must be contacted and informed as soon as practically possible.

---

## 3. Recovery Objectives

Recovery objectives are derived from the Business Impact Analysis Report (BC-BIA-001) and define the maximum operational tolerances for each critical business function. These objectives inform resource allocation decisions and technical DR configurations.

**Definition of terms:**
- **MTPD (Maximum Tolerable Period of Disruption):** The time after which organisational viability, contractual compliance, or regulatory standing is materially threatened.
- **RTO (Recovery Time Objective):** The target time within which a business function must be restored to minimum viable operation following disruption.
- **RPO (Recovery Point Objective):** The maximum acceptable data loss expressed as a point in time prior to the incident.

**Priority Tier classification** is drawn directly from the BIA four-tier prioritisation framework:

### Tier 1 — Mission Critical (RTO ≤ 4 hours)

| # | Business Function | Description | MTPD | RTO | RPO | Priority Tier |
|---|-------------------|-------------|------|-----|-----|---------------|
| 1.1 | Customer Cloud Service Management | 24×7 managed cloud services for 340 enterprise clients; 99.99% SLA commitments | 4 hours | 2 hours | 1 hour | Tier 1 |
| 1.2 | Enterprise Technical Support (P1/P2) | Critical and high-priority incident resolution for enterprise clients; contractual response SLAs | 4 hours | 2 hours | 1 hour | Tier 1 |
| 1.3 | Security Operations Monitoring | 24×7 SOC monitoring and alerting for 180 enterprise clients; any gap creates direct liability | 2 hours | 1 hour | 0 hours (real-time) | Tier 1 |
| 1.4 | Financial Transaction Processing | Payment processing, payroll, and regulatory financial reporting; $180M monthly throughput | 4 hours | 4 hours | 2 hours | Tier 1 |

### Tier 2 — Business Critical (RTO ≤ 24 hours)

| # | Business Function | Description | MTPD | RTO | RPO | Priority Tier |
|---|-------------------|-------------|------|-----|-----|---------------|
| 2.1 | Sales Operations and CRM Access | Opportunity management, customer records, and revenue pipeline visibility | 24 hours | 8 hours | 4 hours | Tier 2 |
| 2.2 | HR and Payroll Processing | Employee administration and payroll execution; time-critical around pay cycle | 48 hours | 24 hours | 24 hours | Tier 2 |
| 2.3 | Email and Collaboration | Internal and external email, video conferencing, document collaboration | 8 hours | 4 hours | 2 hours | Tier 2 |

### Tier 3 — Business Important (RTO ≤ 72 hours)

| # | Business Function | Description | MTPD | RTO | RPO | Priority Tier |
|---|-------------------|-------------|------|-----|-----|---------------|
| 3.1 | Laptop Manufacturing Operations | Hardware assembly and quality assurance; feeds order fulfilment pipeline | 72 hours | 48 hours | 24 hours | Tier 3 |
| 3.2 | Procurement and Supply Chain | Vendor management, purchase orders, and logistics coordination | 5 days | 72 hours | 24 hours | Tier 3 |
| 3.3 | Marketing and Communications | Brand management, campaign execution, and external communications | 7 days | 72 hours | 48 hours | Tier 3 |

### Tier 4 — Business Support (RTO ≤ 5 days)

| # | Business Function | Description | MTPD | RTO | RPO | Priority Tier |
|---|-------------------|-------------|------|-----|-----|---------------|
| 4.1 | Non-Critical Internal IT Services | Internal tooling, intranet, non-production environments | 10 days | 5 days | 48 hours | Tier 4 |
| 4.2 | Documentation and Knowledge Management | Internal knowledge bases, wiki systems, document repositories | 30 days | 5 days | 72 hours | Tier 4 |

**RTO and RPO Breach Escalation:** If recovery is not achieved within 50% of the stated RTO (e.g., 1 hour for a 2-hour RTO), the IT Recovery Lead must escalate to the BC Manager with a revised projected recovery time. If the stated RTO is breached, the BC Manager must notify the Incident Commander (CEO) and initiate the customer notification process per Section 5.2.

---

## 4. Crisis Management Team

The Crisis Management Team (CMT) is the authorised decision-making body during an active BCP incident. All CMT members must be accessible within 30 minutes of notification and must have confirmed their availability to act in their role or nominated their alternate.

CMT members maintain a physical copy of this plan at their primary and alternate contact locations. Updated copies are distributed by the BC Manager within 5 days of any revision.

| # | Role | Primary | Alternate | Contact Details | Key Responsibilities |
|---|------|---------|-----------|-----------------|---------------------|
| 1 | Incident Commander | Chief Executive Officer | Chief Operating Officer | Phone: [REDACTED] / Email: [REDACTED] | Overall command authority; approves major decisions; external stakeholder engagement at board/investor level; approves customer-facing media statements |
| 2 | Business Continuity Manager | Susan Orwell | VP Operations | Phone: [REDACTED] / Email: [REDACTED] | Plan activation and deactivation; CMT coordination; maintains status log; briefs Incident Commander hourly; manages recovery timeline; triggers vendor escalations |
| 3 | IT Recovery Lead | Chief Technology Officer | VP Engineering | Phone: [REDACTED] / Email: [REDACTED] | Executes technical recovery procedures (Section 8); manages DR failover; coordinates infrastructure vendors; reports recovery status every 30 minutes to BC Manager |
| 4 | Communications Lead | VP Communications | Senior Communications Manager | Phone: [REDACTED] / Email: [REDACTED] | Manages internal and external communications; drafts customer notifications; coordinates media response; maintains public communications log |
| 5 | HR Lead | Chief Human Resources Officer | HR Director | Phone: [REDACTED] / Email: [REDACTED] | Staff welfare and headcount; activates remote working protocols; manages personnel succession register; coordinates staff communication cascade |
| 6 | Legal Lead | General Counsel | Deputy General Counsel | Phone: [REDACTED] / Email: [REDACTED] | Regulatory notification obligations; reviews external statements; manages IR firm engagement; advises on contractual liability; coordinates law enforcement liaison if required |
| 7 | Security Lead | Chief Information Security Officer | Deputy CISO | Phone: [REDACTED] / Email: [REDACTED] | Cyber incident response; directs forensic investigation; confirms malware eradication before system restoration; approves cyber-incident public disclosures; manages IR firm retainer activation |
| 8 | Operations Lead | Chief Operating Officer | VP Manufacturing | Phone: [REDACTED] / Email: [REDACTED] | Operational continuity across business units; activates alternative sites; manages supplier escalations; coordinates manufacturing and logistics recovery |

**CMT Quorum:** A minimum of 4 CMT members (or their alternates) is required to constitute a quorum for major recovery decisions. The Incident Commander always counts toward quorum.

**CMT Meeting Cadence During Activation:**
- **First 4 hours:** Hourly virtual or in-person briefings
- **Hours 4–24:** Two-hourly briefings
- **Beyond 24 hours:** Three-hourly briefings or as directed by the Incident Commander

**Virtual CMT Bridge:** A dedicated conference bridge is maintained and tested quarterly. Details are held by the BC Manager and distributed to CMT members via the emergency distribution list.

---

## 5. Communication Plan

### 5.1 Internal Notification Tree

The following sequence governs internal notification upon plan activation. All notifications must be logged with timestamp, method, and recipient confirmation.

**Notification Sequence:**

```
Step 1: BC Manager activates plan → notifies IT Recovery Lead and Security Lead simultaneously
        Method: Phone (primary) / Encrypted SMS (backup)
        Target: Within 15 minutes of activation decision

Step 2: Incident Commander (CEO) notified by BC Manager
        Method: Phone (primary) / Direct email (backup)
        Target: Within 30 minutes of activation

Step 3: Remaining CMT members notified by BC Manager
        Method: ServiceNow Major Incident notification + direct phone
        Target: Within 30 minutes of activation

Step 4: Department Heads notified by their respective CMT lead
        Method: Email to department distribution list + phone for Tier 1 function owners
        Target: Within 1 hour of activation

Step 5: All affected staff notified by HR Lead
        Method: Company-wide email + intranet alert + (if email unavailable) manager cascade
        Target: Within 2 hours of activation, or sooner if safety-relevant
```

**Primary Notification Channel:** ServiceNow Major Incident process — auto-generates tickets, assigns recovery tasks, and maintains audit log of all notifications and status updates.

**Backup Notification Channel:** Direct phone contact using the CMT contact list (Section 4) followed by the emergency email distribution list held by the BC Manager. The emergency distribution list includes all CMT members, alternates, department heads, and IT recovery team members.

**If email systems are unavailable:** HR Lead activates the manager cascade phone tree. Each manager is responsible for confirming contact with their direct reports within 2 hours.

### 5.2 External Notification — Customers

All external customer communications during an active incident require approval from the Communications Lead and are logged in the Customer Notification Register maintained in ServiceNow.

| Scenario | Notification Trigger | Responsible Party | Method | Template |
|----------|---------------------|-------------------|--------|----------|
| RTO breach — Tier 1 managed service | RTO for affected function breached | Account Management (directed by Comms Lead) | Email + phone to named customer contacts | Template EXT-01 (below) |
| Planned maintenance during recovery | Prior to any maintenance window extending downtime | Account Management | Email | Template EXT-02 |
| Recovery confirmed | Function restored to full service | Account Management | Email | Template EXT-03 |
| SLA credit notification | Post-incident within 5 business days | Account Management + Finance | Formal letter | Template EXT-04 |

**Template EXT-01 — RTO Breach Notification (Draft):**
> Subject: Service Impact Notification — [Service Name] — [Date]
>
> Dear [Customer Name],
>
> We are writing to inform you that Emyzer Technology is currently experiencing a service disruption affecting [Service Name]. Our teams are actively working to restore service. We will provide an update within [1/2] hour(s). We apologise for any inconvenience and thank you for your patience.
>
> For urgent assistance, please contact your designated Account Manager at [REDACTED] or our incident line at [REDACTED].
>
> — Emyzer Technology Crisis Management Team

**Template EXT-03 — Recovery Confirmation (Draft):**
> Subject: Service Restored — [Service Name] — [Date]
>
> Dear [Customer Name],
>
> We are pleased to confirm that [Service Name] has been fully restored as of [Time] on [Date]. The incident affecting your service has been resolved. A full post-incident report will be provided within 5 business days. If you have any questions or concerns, please contact your Account Manager.
>
> — Emyzer Technology Crisis Management Team

**Affected client list:** Maintained by Account Management in Salesforce CRM. During a system outage, the BC Manager holds an offline backup export (last updated at each DR test).

### 5.3 Regulatory Notification

The Legal Lead is responsible for assessing and executing regulatory notification obligations. Notification must not be delayed pending full incident analysis; partial notifications with updates are acceptable where full information is not yet available.

| Regulation | Trigger | Authority | Deadline | Owner | Notes |
|------------|---------|-----------|----------|-------|-------|
| GDPR Article 33 [VERIFY] | Confirmed or suspected personal data breach | Lead supervisory authority (ICO for UK; relevant EU DPA for EU operations) | 72 hours from becoming aware of breach | Legal Lead + CISO | Notification must include: nature of breach; categories and approximate number of data subjects; likely consequences; measures taken. Data processor obligation: notify Emyzer Technology (as controller) without undue delay |
| EU AI Act Article 73 [VERIFY] | Serious incident involving a high-risk AI system | National market surveillance authority | As specified in implementing acts [VERIFY]; presently within 15 working days for serious incidents [VERIFY] | Legal Lead + CISO | Applies if Veridian AI systems integrated into Emyzer Technology operations. Coordinate with AI Governance Committee |
| Financial regulations | Any incident affecting financial reporting systems for a material period | FCA / relevant national financial regulator | Per regulatory requirements [VERIFY] | Legal Lead + CFO | Legal Lead to assess applicability per jurisdiction |
| Employment / health and safety | Incidents involving workplace injury or safety risk | HSE or relevant national authority | As required by applicable law [VERIFY] | Legal Lead + HR Lead | Immediate notification if serious injury involved |

**Regulatory Notification Log:** All notifications are recorded in ServiceNow with timestamp, authority notified, method, content summary, and follow-up actions.

### 5.4 Media and Public Communications

All external statements to media, social media, or public channels require:

1. Draft prepared by Communications Lead
2. Review and approval by Legal Counsel (for all statements)
3. Additional approval by CISO for any statement relating to a cyber incident or data breach

**No CMT member, employee, or contractor is authorised to make public statements about an active incident without following this approval process.**

The Communications Lead maintains a media monitoring log during active incidents and alerts the CMT to any emerging media coverage that may require response. The CEO may be required to make statements for incidents assessed as high reputational risk; the Communications Lead will brief the CEO in advance of any media engagement.

---

## 6. Recovery Strategies by Disruption Type

### 6.1 Technology / IT Disruption

**Scenario:** Unplanned outage, system failure, data corruption, or infrastructure unavailability affecting Tier 1 or Tier 2 systems.

**Primary Recovery Strategy — AWS Failover:**
- Tier 1 systems are pre-configured for active-active or active-passive failover to the AWS secondary region (designated DR region, maintained at parity with production).
- Failover is automated for Tier 1 systems (Cloud Service Management, Security Operations); manual invocation is required for Tier 2 systems.
- Target: Tier 1 system recovery within 2 hours of activation; Tier 2 within 8 hours.
- DNS failover is pre-configured; propagation window of 5–15 minutes is included in RTO calculations.

**Backup Recovery Strategy — Restore from Immutable Backup:**
- All critical systems maintain immutable backups in AWS S3 with Object Lock enabled (WORM configuration).
- Backup frequency and RPO alignment per system are documented in Section 8.2.
- Restore process is invoked if failover to secondary region fails or if the outage affects both primary and secondary environments simultaneously.
- CISO must confirm absence of active malware before any restore from backup is initiated following a cyber incident.

**Manual Fallback Procedures:**
- Documented manual procedures exist for all Tier 1 functions and are valid for up to 8 hours of system unavailability.
- Manual procedures are held in printed form at each recovery site and in the BC Manager's offline recovery pack.
- Manual fallback covers: customer incident logging via phone, financial transaction approval via manual sign-off, and security monitoring via manual log review from isolated terminal.

**Escalation — DR Environment Unavailable:**
- If both primary and DR environments are unavailable, the IT Recovery Lead invokes the Emergency Change Process to provision temporary infrastructure using pre-approved AWS CloudFormation templates.
- Emergency provisioning target: basic Tier 1 capability within 4 hours.
- Emergency infrastructure costs are pre-approved up to [REDACTED] without additional CFO authorisation.

### 6.2 Premises Loss / Workplace Disruption

**Scenario:** Office, facility, or data centre rendered inaccessible or unsafe due to fire, flooding, civil emergency, utility failure, or other cause.

**Remote Working Capability:**
- All Emyzer Technology staff are equipped for full remote working capability. Laptops issued to all employees include pre-configured VPN client, MDM enrollment, and collaboration tools.
- VPN infrastructure is sized to support 100% concurrent remote operation.
- The HR Lead confirms remote working readiness at each annual communication cascade test.

**Alternative Recovery Sites:**
- **Recovery Site A — [Region A]:** Designated recovery facility with capacity for [REDACTED] critical team members, equipped with secure workstations, dedicated MPLS connectivity, and conference facilities. Maintained under standing arrangement with facilities provider.
- **Recovery Site B — [Region B]:** Secondary recovery facility as above. Used where Region A is also affected or at capacity.
- Allocation of seats at recovery sites is prioritised by business function tier: Tier 1 functions receive first allocation; Tier 2 receive second; Tier 3 and 4 staff work remotely where possible.
- Recovery site activation is managed by the Operations Lead in coordination with the HR Lead.

**Manufacturing Site Disruption:**
- Hardware production requires physical facilities and cannot be fully replicated remotely.
- Production line recovery procedures are documented in the Manufacturing Business Continuity Plan (Annex C to this document).
- In the event of manufacturing site loss, the Operations Lead engages pre-identified contract manufacturing partners (details in Annex C) to maintain minimum production capacity.
- Financial impact of manufacturing disruption above the Tier 3 MTPD is escalated to the CFO for insurance notification.

### 6.3 Cyber Incident / Ransomware

**Scenario:** Confirmed ransomware deployment, destructive malware, data exfiltration, or other cyber attack requiring isolation of production systems.

**Step-by-step strategy:**

1. **Immediate actions (0–30 minutes):** CISO activates Incident Management Policy procedures simultaneously with this BCP. Security Operations team isolates affected systems per the Incident Response Playbook (Annex D).
2. **Containment (0–2 hours):** Affected systems isolated from production network. CISO confirms scope of compromise. BC Manager activates CMT.
3. **Clean-room environment activation:** IT Recovery Lead provisions a clean-room recovery environment in a separate AWS account with no connectivity to potentially compromised systems.
4. **Forensic preservation:** CISO or appointed IR firm preserves forensic images of affected systems before any remediation.
5. **Malware eradication confirmation:** CISO must provide written confirmation (email to BC Manager) that malware has been eradicated from all affected systems before any restore from backup is initiated.
6. **Restore from immutable backup:** IT Recovery Lead initiates restore from immutable S3 backup (pre-confirmed clean state) per Section 8.2.
7. **Validation and controlled re-introduction:** Restored systems validated against known-good configuration baselines before re-introduction to production.
8. **External IR firm:** A retainer agreement with an external Incident Response firm is in place (contract held by Legal Counsel). The CISO has authority to activate the retainer without CEO pre-approval up to the value specified in the retainer agreement.

**Note:** Ransomware recovery does not involve payment of any ransom without explicit CEO and board-level authorisation and Legal Counsel review of jurisdictional implications.

### 6.4 Key Person Unavailability

**Scenario:** Simultaneous unavailability of 3 or more members of the Executive Leadership Team due to illness, travel disruption, or other cause.

**Succession strategy:**

- All critical roles have documented successors and formally delegated authority, reviewed and updated annually by HR.
- The Succession Register is maintained by the HR Lead and is stored in a location accessible offline (held by BC Manager in recovery pack).
- For each Tier 1 business function, a Minimum Viable Team is documented, identifying the minimum number of staff and the minimum seniority required to execute recovery procedures.
- Where a succession gap is identified (i.e., both primary and alternate for a CMT role are unavailable), the BC Manager escalates to the Incident Commander to appoint a temporary role-holder from the available senior leadership population.

**Preventing key-person dependency:**
- Recovery runbooks (Sections 7 and 8) are written to be executable by trained alternates without reliance on primary role-holder knowledge.
- Recovery procedures are tested annually with alternates in lead roles to validate succession capability.

### 6.5 Supplier / Third-Party Failure

**Scenario:** A Tier 1 supplier (defined as a supplier whose failure would directly impair a Tier 1 or Tier 2 business function) is unable to deliver services or components.

**Mitigation and response strategy:**

- **Contractual BCP requirements:** All Tier 1 supplier contracts include provisions requiring the supplier to maintain and test a BCP, to notify Emyzer Technology of any activation or material disruption risk within 4 hours, and to provide annual BCP attestations.
- **Backup suppliers:** Pre-identified backup suppliers exist for each critical dependency. Backup supplier contracts are maintained at a minimum of pre-qualification status, enabling rapid activation. Current backup supplier register is maintained by the Operations Lead.
- **Manual workarounds:** Documented manual workarounds exist for each Tier 1 supplier dependency, valid for a minimum of 48 hours. These are reviewed at each supplier BCP validation exercise.
- **Supplier escalation:** Upon activation, the Operations Lead initiates direct escalation to the supplier's account director and BCP coordinator. The BC Manager may invoke contractual SLA remedies concurrently.
- **Extended supplier failure:** If supplier failure is projected to exceed the Tier MTPD, the Operations Lead and Legal Lead jointly assess contract termination and emergency procurement options.

---

## 7. Recovery Procedures by Tier

### 7.1 Tier 1 Recovery Procedures (0–4 Hours)

Tier 1 recovery procedures are to be initiated immediately upon BCP activation. The IT Recovery Lead is the execution owner; each step must be completed and confirmed before proceeding to the next. All steps are logged in ServiceNow with timestamps.

---

#### 7.1.1 Customer Cloud Service Management Recovery

**Recovery owner:** IT Recovery Lead
**Support:** Cloud Platform Team (minimum 4 engineers)
**RTO:** 2 hours | **RPO:** 1 hour

| Step | Action | Owner | Acceptance Criteria | Target Time |
|------|--------|-------|---------------------|-------------|
| 1 | Confirm scope of outage — identify affected services, customer accounts, and geographic regions; document in ServiceNow incident ticket | IT Recovery Lead | Scope confirmed and documented | T+0:15 |
| 2 | Activate AWS regional failover — execute pre-validated failover runbook for cloud service stack (CloudFormation stack set, Route 53 failover routing policy) | Cloud Platform Team | Failover initiated; confirmation in AWS Console and runbook checklist | T+0:30 |
| 3 | Confirm DNS propagation — verify failover DNS records are resolving correctly from at least 3 external monitoring locations | Cloud Platform Team | DNS propagation confirmed; no resolution errors | T+0:45 |
| 4 | Validate core service functionality — execute smoke tests against all Tier 1 managed service components in DR environment | Cloud Platform Team | All smoke tests pass; no critical errors in application logs | T+1:15 |
| 5 | Restore from backup (if failover insufficient or data inconsistency detected) — identify latest clean recovery point; initiate restore from immutable S3 backup | IT Recovery Lead | RPO confirmed as met; data integrity verified | T+1:30 |
| 6 | Notify affected managed services clients — Account Management to send Template EXT-01 to all affected customer contacts; log in Customer Notification Register | Communications Lead / Account Management | All affected clients notified; notification log updated | T+1:30 |
| 7 | Validate monitoring dashboards — confirm CloudWatch, Datadog, and ServiceNow dashboards are receiving telemetry from DR environment; alert thresholds verified | Cloud Platform Team | All dashboards operational; no false alert suppression | T+1:45 |
| 8 | Confirm recovery to BC Manager — IT Recovery Lead provides written status update confirming recovery completion or revised ETA | IT Recovery Lead | Written update sent and acknowledged | T+2:00 |
| 9 | Begin post-incident logging — document timeline, actions taken, and deviations from this procedure | BC Manager | Incident log updated in ServiceNow | Ongoing |

**Manual fallback (if DR environment unavailable):** Activate manual client management procedure — assign dedicated account managers to all P1 clients; log incidents via phone; maintain manual status board; valid for maximum 8 hours pending emergency infrastructure provisioning.

---

#### 7.1.2 Security Operations Monitoring Recovery

**Recovery owner:** Security Lead (CISO)
**Support:** SOC Team (minimum 3 analysts + 1 senior engineer)
**RTO:** 1 hour | **RPO:** Real-time (0 hours — no monitoring gap acceptable)

| Step | Action | Owner | Acceptance Criteria | Target Time |
|------|--------|-------|---------------------|-------------|
| 1 | Activate bridge call — CISO convenes SOC team and confirms incident scope; assess whether primary SIEM is unavailable or compromised | CISO | All available SOC staff on bridge; scope documented | T+0:10 |
| 2 | Redirect SIEM ingestion — configure log sources (firewalls, EDR, cloud logs) to forward to secondary SIEM collector in DR environment; validate syslog/API forwarding | Senior SOC Engineer | All Tier 1 log sources confirmed forwarding to secondary collector | T+0:25 |
| 3 | Activate DR SIEM environment — bring up secondary SIEM (pre-configured warm standby) in isolated AWS account; confirm platform health | Senior SOC Engineer | DR SIEM platform responding; ingestion confirmed | T+0:35 |
| 4 | Validate alert thresholds and detection rules — confirm correlation rules, alert thresholds, and watchlist feeds are active and correctly configured in DR SIEM | Senior SOC Engineer | Rule set confirmed; test alert generated and received | T+0:45 |
| 5 | Brief on-call security engineer — CISO or senior analyst briefs on-call engineer on current incident context, known indicators of compromise, and any concurrent threat intelligence | CISO | Briefing confirmed and logged | T+0:50 |
| 6 | Notify managed security clients of monitoring continuity — if any monitoring gap occurred, notify affected clients per communication template | CISO / Account Management | Client notifications sent and logged | T+1:00 |
| 7 | Confirm recovery to BC Manager | CISO | Written confirmation sent | T+1:00 |

**Monitoring gap protocol:** If any monitoring gap occurs (no matter how brief), the CISO must assess whether any security events may have been missed during the gap and conduct a compensating review of available logs from adjacent systems.

---

#### 7.1.3 Financial Transaction Processing Recovery

**Recovery owner:** CFO
**Support:** Finance Operations Team (minimum 3 staff)
**RTO:** 4 hours | **RPO:** 2 hours

| Step | Action | Owner | Acceptance Criteria | Target Time |
|------|--------|-------|---------------------|-------------|
| 1 | Assess impact — confirm which financial systems are affected; determine if outage is infrastructure-layer or application-layer; confirm last clean backup timestamp | CFO / IT Recovery Lead | Impact scope confirmed; backup timestamp documented | T+0:20 |
| 2 | Switch to read-only mode — instruct all finance staff to take no transactional actions in any partially available systems; confirm in writing | CFO | All finance staff confirmed on read-only standing; log entry created | T+0:30 |
| 3 | Activate manual approval process — for all transactions greater than £10,000, CFO manual sign-off required via documented paper or secure email; designated finance manager for sub-£10K | CFO | Manual approval process communicated to all Finance staff | T+0:45 |
| 4 | Isolate payment processing — instruct banking partner to hold all automated payment runs pending system recovery; obtain confirmation reference | CFO / Finance Director | Banking partner hold confirmed in writing | T+1:00 |
| 5 | Initiate system recovery — IT Recovery Lead activates ERP failover to DR instance; confirm data integrity at RPO point | IT Recovery Lead | ERP DR instance online; RPO validated (last clean checkpoint within 2 hours) | T+2:00 |
| 6 | Reconcile transactions since RPO — Finance team manually reconciles any transactions that occurred after RPO checkpoint using paper records and bank statements | Finance Director | Reconciliation log completed and reviewed by CFO | T+3:00 |
| 7 | Resume automated processing — CFO confirms all manual transaction records reconciled before re-enabling automated payment runs | CFO | Authorisation confirmation signed and filed | T+4:00 |
| 8 | Confirm recovery to BC Manager | CFO | Written confirmation sent | T+4:00 |

---

### 7.2 Tier 2 Recovery Procedures (4–24 Hours)

Tier 2 recovery is initiated in parallel with Tier 1 where resources allow, but must not delay Tier 1 completion. The IT Recovery Lead and Operations Lead share ownership of Tier 2 recovery.

---

#### 7.2.1 Email and Collaboration Recovery (RTO: 4 hours)

| Step | Action | Owner | Target Time |
|------|--------|-------|-------------|
| 1 | Confirm scope — assess whether outage is Microsoft 365 tenancy-wide, regional, or application-specific | IT Recovery Lead | T+0:30 |
| 2 | Engage Microsoft support — open Sev-A support case; obtain ETA for platform restoration | IT Operations | T+0:45 |
| 3 | Activate backup communication channels — staff directed to use personal mobile for urgent calls; BC Manager activates emergency distribution lists via secondary email provider | HR Lead | T+1:00 |
| 4 | Restore from backup (if tenant-side issue) — initiate restore of mailbox data from immutable backup; validate RPO | IT Recovery Lead | T+2:00 |
| 5 | Validate collaboration tools — confirm Teams / SharePoint / OneDrive accessible from DR environment | IT Operations | T+3:30 |
| 6 | Confirm recovery to BC Manager | IT Recovery Lead | T+4:00 |

---

#### 7.2.2 Sales Operations and CRM Access Recovery (RTO: 8 hours)

| Step | Action | Owner | Target Time |
|------|--------|-------|-------------|
| 1 | Confirm CRM availability — assess Salesforce (or primary CRM) accessibility; determine if platform-side or integration issue | IT Recovery Lead | T+1:00 |
| 2 | Activate offline CRM export — distribute most recent CRM data export (maintained by Sales Operations; updated weekly) to sales leadership; sales activity continues against offline record | VP Sales | T+2:00 |
| 3 | Restore CRM integrations — re-establish data flows from ERP and email to CRM; validate integration health | IT Operations | T+5:00 |
| 4 | Reconcile offline activity — sales staff log any CRM activity conducted offline; data reconciliation completed post-recovery | Sales Operations | T+8:00 |
| 5 | Confirm recovery to BC Manager | Operations Lead | T+8:00 |

---

#### 7.2.3 HR and Payroll Processing Recovery (RTO: 24 hours)

| Step | Action | Owner | Target Time |
|------|--------|-------|-------------|
| 1 | Assess pay cycle proximity — HR Lead determines whether payroll run is due within 48 hours; if yes, escalate to Tier 1 treatment | HR Lead | T+1:00 |
| 2 | Notify payroll provider — if using managed payroll service, notify provider of system unavailability; obtain commitment for manual payroll processing if required | HR Lead | T+2:00 |
| 3 | Activate HR data offline pack — HR Lead holds encrypted offline copy of employee master data and current payroll configuration | HR Lead | T+2:00 |
| 4 | Restore HRIS from DR — IT Recovery Lead initiates HRIS restore from immutable backup; validate data integrity | IT Recovery Lead | T+12:00 |
| 5 | Confirm recovery and reconcile any offline changes | HR Lead | T+24:00 |

---

### 7.3 Tier 3 and Tier 4 Recovery

Tier 3 and Tier 4 recovery procedures are documented in the following departmental annexes and are activated by the relevant department head under direction of the Operations Lead:

| Annex | Function | Document | Owner |
|-------|----------|----------|-------|
| Annex A | Procurement and Supply Chain Recovery | Procurement BCP Annex | Operations Lead |
| Annex B | Marketing and Communications Recovery | Marketing BCP Annex | Communications Lead |
| Annex C | Manufacturing Operations Recovery | Manufacturing BCP | VP Manufacturing |
| Annex D | Incident Response Playbooks (Cyber) | IR Playbook Pack | CISO |

Tier 3 and 4 recovery is not initiated until all Tier 1 and Tier 2 functions are confirmed recovered or are actively progressing toward recovery with a confirmed revised ETA.

---

## 8. IT Recovery Procedures

### 8.1 System Recovery Priority Order

Systems are recovered in the sequence determined by the business function tier they support. No lower-tier system is to be recovered before all higher-tier supporting systems are confirmed operational.

| Priority | Business Function | Supporting Systems | Recovery Owner |
|----------|------------------|--------------------|----------------|
| 1 | Security Operations Monitoring | Primary/DR SIEM, EDR management console, log aggregation platform, SOC tooling | CISO / Senior SOC Engineer |
| 2 | Customer Cloud Service Management | Virtualisation platform, cloud orchestration layer, customer-facing APIs, DNS / load balancer, monitoring (CloudWatch / Datadog) | Cloud Platform Team |
| 3 | Enterprise Technical Support (P1/P2) | CRM (support module), knowledge base platform, remote access tooling, ticketing system (ServiceNow) | IT Operations |
| 4 | Financial Transaction Processing | ERP (finance module), banking integration APIs, payroll platform | IT Recovery Lead + Finance |
| 5 | Email and Collaboration | Microsoft 365 (Exchange, Teams, SharePoint), email gateway | IT Operations |
| 6 | Sales Operations / CRM | Salesforce (or primary CRM), CRM integrations | IT Operations |
| 7 | HR / Payroll | HRIS platform, payroll engine | IT Operations |
| 8 | Manufacturing / ERP | ERP (manufacturing module), MES, QMS | IT Operations + Operations Lead |
| 9 | Non-critical internal services | Intranet, wikis, non-production environments | IT Operations (after business hours if possible) |

### 8.2 Database Recovery

Databases supporting Tier 1 systems must be recovered before dependent application layers are brought online. The IT Recovery Lead confirms RPO is met for each database before any application depending on it is restored.

| Database | Supporting System | Backup Type | Backup Frequency | RPO Target | Recovery Procedure | Recovery Validation |
|----------|------------------|-------------|-----------------|------------|-------------------|---------------------|
| Cloud Services DB (Primary) | Customer cloud platform | Continuous replication + hourly snapshot | Continuous (WAL); hourly full snapshot | 1 hour | Promote DR replica or restore from S3 snapshot | Query data timestamp; run integrity check script |
| SIEM Events DB | Security Operations | Real-time replication to secondary | Real-time | 0 (real-time) | Failover to secondary collector; no restore required | Confirm log ingestion resumed; validate event counts |
| Financial Ledger DB | ERP (finance module) | Incremental every 15 min; full daily | 15-minute incremental; daily full | 2 hours | Restore from latest pre-incident snapshot + apply transaction logs to RPO point | CFO sign-off on data integrity; reconcile against payment gateway records |
| CRM DB | Salesforce / CRM | Platform-native backup (daily export + Salesforce Backup) | Daily | 4 hours | Restore from Salesforce Backup or daily export | Validate record counts; confirm integrations reconnected |
| HRIS DB | HR platform | Daily full backup | Daily | 24 hours | Restore from daily backup | HR Lead validates employee count and payroll configuration |
| ServiceNow Ticketing | Support / ITSM | ServiceNow cloud SaaS — provider-managed | Per platform SLA | Per platform SLA | Engage ServiceNow support; activate offline ticket log | Confirm ticket routing and assignment rules active |

**Database recovery protocol:**
1. IT Recovery Lead identifies latest clean backup point (verified as pre-incident and free from corruption).
2. For cyber incidents: CISO confirms backup is from a pre-compromise snapshot before restore is initiated.
3. Restore initiated in isolated environment; integrity checks run before DR database is promoted to production.
4. RPO achievement confirmed in writing (email from IT Recovery Lead to BC Manager) before dependent applications are started.

### 8.3 Application Recovery Sequence

Applications are brought online in dependency order. No application is started until all databases and services it depends on have been confirmed operational.

| Seq | Application | Depends On | Start Procedure | Health Check |
|-----|-------------|-----------|-----------------|--------------|
| 1 | SIEM / SOC platform | SIEM Events DB, network connectivity | Initiate DR SIEM stack via runbook; validate agent connectivity | Log ingestion confirmed; test alert received |
| 2 | Cloud orchestration layer | Cloud Services DB, virtualisation platform | Execute CloudFormation stack deployment in DR region | Stack health check passes; VMs online |
| 3 | Customer-facing cloud APIs | Cloud orchestration layer | Restart API gateway services; validate endpoint health | API smoke tests pass; latency within SLA |
| 4 | ServiceNow (ITSM) | Network, identity platform | Platform SaaS — verify access; if unavailable engage support | Ticket creation and routing verified |
| 5 | Remote access / VPN | Network, identity platform (AD/AAD) | Validate VPN concentrator health; confirm capacity for full remote load | VPN connectivity test from 3 external locations |
| 6 | Microsoft 365 | Exchange Online, network | Platform SaaS — verify access; if tenant-side restore required, initiate from backup | Email send/receive test; Teams call test |
| 7 | ERP — finance module | Financial Ledger DB, network | Restart ERP application services; load balanced across DR nodes | CFO test transaction; reconciliation report runs |
| 8 | CRM | CRM DB, ERP integration | Restart CRM application; re-establish API integrations | Record retrieval test; integration pipeline validated |
| 9 | ERP — manufacturing module | ERP finance module, MES | Restart manufacturing module; validate production schedule data | Operations Lead validates production data accuracy |
| 10 | Non-critical internal apps | All above | Restore to normal operations schedule | Standard UAT by application owners |

### 8.4 Network Recovery

Network recovery is prerequisite to all application recovery. The IT Recovery Lead coordinates with the network team for the following:

**DNS Recovery:**
1. Confirm DNS failover routing policy is active in Route 53 (or equivalent).
2. Validate TTL values have propagated — confirm resolution from at least 3 external resolvers.
3. If DNS provider is unavailable, activate backup DNS provider (pre-configured secondary zone).
4. Update firewall rules to reflect DR environment IP ranges where applicable.

**Load Balancer Recovery:**
1. Confirm load balancer health checks are targeting DR environment nodes.
2. Validate SSL certificates are valid and not expiring within 72 hours.
3. Test end-to-end traffic routing through load balancer to application tier.

**VPN Recovery:**
1. Confirm VPN concentrator is operational and accessible from external networks.
2. Validate split-tunnel configuration to ensure corporate traffic routes correctly.
3. Test capacity — run concurrent connection stress test to validate 100% remote working capacity.
4. Confirm MFA is enforced for all VPN connections.

**Emergency network access:**
- If corporate network is entirely unavailable, authorised staff may use personal internet with mandatory MFA and endpoint security validation.
- The CISO must authorise any exception to standard network security controls.

### 8.5 Endpoint Recovery

**Device replacement:**
- All replacement devices are provisioned via MDM (Microsoft Intune or equivalent).
- MDM auto-enrollment profile is pre-staged; new devices join the correct security group automatically.
- Security baseline policies, encryption (BitLocker), EDR agent, and VPN client are applied automatically upon enrollment.

**Recovery kit contents** (held at each recovery site and by BC Manager):
- Pre-imaged spare laptops (minimum 10 units per recovery site, refreshed annually)
- Power adapters (multi-country)
- Mobile hotspot devices (network-independent connectivity)
- Encrypted USB drives containing: offline MFA backup codes, offline recovery procedure documents, CMT contact list
- Printed copies of this BCP, Tier 1 and 2 recovery runbooks, and CMT contact list

**Endpoint rebuild time target:** 30 minutes per device from recovery kit; 2 hours via MDM enrollment for newly ordered hardware.

---

## 9. Testing and Exercising

ISO 22301:2019 Clause 8.5 [VERIFY] requires organisations to validate their business continuity plans and capabilities through a programme of exercises. Emyzer Technology maintains the following exercise schedule, designed to progressively validate all elements of this BCP.

### 9.1 Exercise Schedule

| Exercise Type | Frequency | Scope | Participants | Last Conducted | Next Scheduled | Owner |
|---------------|-----------|-------|--------------|----------------|----------------|-------|
| Plan walkthrough (tabletop) | Annual | Full CMT; all BCP sections reviewed against current organisational state | All CMT members and alternates | 2024-03-15 | 2025-03-15 | BC Manager |
| Technical DR test (live failover) | Semi-annual | Tier 1 systems; live failover to DR environment and failback; RTO and RPO validation | IT Recovery Lead, Cloud Platform Team, CISO, SOC Team | 2024-06-30 | 2024-12-30 | IT Recovery Lead |
| Communication cascade test | Annual | All staff; test internal notification tree and backup channels | BC Manager, HR Lead, Communications Lead, all department heads | 2024-09-01 | 2025-09-01 | Communications Lead |
| Full business continuity exercise (simulation) | Biennial | All business functions; simulated major incident scenario involving multiple disruption types; CMT and recovery teams participate | All CMT, all department heads, recovery team leads | Not yet conducted | 2025-06-01 | BC Manager |
| Supplier BCP validation | Annual | All Tier 1 suppliers; review supplier BCP attestations and test supplier notification procedures | Operations Lead, Vendor Risk Manager | 2024-05-01 | 2025-05-01 | Vendor Risk Manager |
| Key person succession test | Annual | Tier 1 function recovery procedures executed by alternates only, with primary role-holders excluded | BC Manager, HR Lead, all alternates | 2024-09-01 | 2025-09-01 | BC Manager |

### 9.2 Exercise Objectives and Pass/Fail Criteria

Each exercise must have pre-defined objectives and measurable pass/fail criteria agreed by the BC Manager before the exercise is conducted. At minimum, technical DR tests must validate:

- RTO achieved for all Tier 1 systems within stated targets
- RPO confirmed for all Tier 1 databases
- Failback to primary environment completed without data loss
- Monitoring dashboards operational in DR environment within 1 hour of failover

Tabletop exercises must validate:
- All CMT roles filled (primary or alternate)
- Communication cascade completed within stated notification windows
- All Tier 1 recovery decisions correctly escalated per this BCP

### 9.3 Exercise Reporting and Finding Management

1. **Exercise Report:** Within 10 business days of each exercise, the exercise owner produces a written exercise report documenting: objectives; participants; scenario; outcomes against pass/fail criteria; findings; recommended plan updates.
2. **Finding Classification:** Findings are classified as Critical (plan unable to achieve Tier 1 RTO), Major (plan would achieve RTO but with significant difficulty), or Minor (improvements to efficiency or clarity).
3. **Remediation:** Critical findings must be remediated and retested within 60 days. Major findings within 90 days. Minor findings addressed at the next scheduled plan review.
4. **Plan Update Trigger:** Any Critical or Major finding triggers an out-of-cycle plan review per Section 10. The updated plan is distributed to all CMT members within 5 days of approval.
5. **Trend Analysis:** The BC Manager reviews cumulative exercise findings annually to identify systemic weaknesses and update training priorities.

---

## 10. Plan Maintenance

### 10.1 Scheduled Review

This plan is subject to formal annual review by the BC Manager, due on or before the anniversary of the effective date (2025-09-01). The annual review considers:

- Organisational changes (new business units, acquisitions, staff changes)
- Changes to critical technology infrastructure
- Changes to regulatory requirements
- Exercise findings from the preceding 12 months
- Changes to Tier 1 supplier arrangements
- Lessons learned from any activated incidents

### 10.2 Trigger-Based Review

In addition to the scheduled annual review, a trigger-based review must be initiated within 15 business days of any of the following events:

- Major organisational change (including acquisition, merger, or significant restructuring)
- Activation of this plan in response to a real incident
- Critical or Major exercise finding
- Significant change to critical technology infrastructure (e.g., cloud migration, data centre change)
- Change to the CMT structure (new members, departures)
- Material change to regulatory obligations

### 10.3 Change Authority

| Change Classification | Examples | Approval Required | Notification |
|----------------------|----------|------------------|-------------|
| Minor update | Contact details; correction of factual errors; clarification of procedures; schedule updates | BC Manager authority | CMT notified within 5 days |
| Moderate update | Revised recovery procedures; updated system names; new annex content | BC Manager sign-off + CTO/CISO review | CMT notified within 5 days |
| Major update | Revised recovery objectives (RTO/RPO); changes to CMT structure; changes to activation criteria; changes to recovery strategy | CEO approval required | Full CMT notified; re-briefing within 10 days |

### 10.4 Version Control and Distribution

- This plan is maintained in the GRC document repository with full version history.
- Each release is version-numbered (major.minor format: e.g., 1.0, 1.1, 2.0).
- The distribution list is maintained by the BC Manager.
- The plan is classified Restricted and is distributed only to named CMT members and their named alternates.
- Electronic distribution is via encrypted email; physical copies are held at each recovery site.
- Recipients must confirm receipt and acknowledge any major version update.
- Superseded versions are retained in the document repository for audit purposes; only the current version is distributed to CMT members.

---

## 11. Framework Alignment

### 11.1 [ISO 22301:2019](https://www.iso.org/standard/75106.html) Mapping

| ISO 22301:2019 Clause | Clause Description | BCP Section | Notes |
|-----------------------|--------------------|-------------|-------|
| Cl. 4.1 | Understanding the organisation and its context | Section 1.2 (Scope) | Organisational context defined in BC/DR Policy |
| Cl. 4.2 | Understanding the needs and expectations of interested parties | Sections 5.2, 5.3 | Customer and regulatory notification obligations |
| Cl. 6.1 | Actions to address risks and opportunities | Section 2 (Activation Criteria) | Risk-based activation thresholds |
| Cl. 8.2 | Business impact analysis and risk assessment | Section 3 (Recovery Objectives) | RTO/RPO/MTPD derived from BIA Report BC-BIA-001 [VERIFY] |
| Cl. 8.3 | Business continuity strategy and solutions | Section 6 (Recovery Strategies) | Technology, premises, cyber, people, and supplier strategies documented |
| Cl. 8.4 | Business continuity plans and procedures | Sections 4–8 | CMT, communications, and recovery procedures |
| Cl. 8.5 | Exercise programme | Section 9 (Testing and Exercising) | Multi-type exercise programme with defined frequencies and pass/fail criteria |
| Cl. 8.6 | Evaluation of business continuity documentation and capabilities | Section 10 (Plan Maintenance) | Annual and trigger-based review; change authority matrix |
| Cl. 9.1 | Monitoring, measurement, analysis and evaluation | Section 9.2 (Pass/Fail Criteria) | Measurable exercise criteria; KPI tracking |
| Cl. 9.3 | Management review | Section 10.1 (Scheduled Review) | Annual review includes CMT and executive sign-off |
| Cl. 10.1 | Nonconformity and corrective action | Section 9.3 (Finding Management) | Exercise findings classified and remediated within defined timeframes |

### 11.2 [NIST SP 800-34 Rev. 1](https://csrc.nist.gov/publications/detail/sp/800-34/rev-1/final) Mapping

| NIST SP 800-34 Phase | Description | BCP Section |
|---------------------|-------------|-------------|
| Phase 1 — Develop Contingency Planning Policy | Policy framework for continuity | BC/DR Policy (parent document) |
| Phase 2 — Conduct Business Impact Analysis | Identify critical systems, outage impacts, recovery priorities | BIA Report (BC-BIA-001); Recovery Objectives (Section 3) |
| Phase 3 — Identify Preventive Controls | Controls to reduce likelihood and impact of disruption | Section 6 (Recovery Strategies); IT DR configuration |
| Phase 4 — Create Contingency Strategies | Alternative processing strategies | Sections 6.1–6.5 |
| Phase 5 — Develop Contingency Plan | Documented recovery procedures | Sections 4–8 |
| Phase 6 — Plan Testing and Exercises | Validate plan effectiveness | Section 9 |
| Phase 7 — Plan Maintenance | Keep plan current | Section 10 |

---

## 12. Related Documents

| Document | Document ID | Location | Owner |
|----------|-------------|----------|-------|
| Business Continuity and Disaster Recovery Policy | KB-PORTFOLIO-0006 | [https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/bcdr-policy.md](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/bcdr-policy.md) | BC Manager |
| Business Impact Analysis Report | BC-BIA-001 | [https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/business-continuity/business-impact-analysis-report.md](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/business-continuity/business-impact-analysis-report.md) | BC Manager |
| Asset Risk Register | RISK-REG-001 | GRC Repository (ServiceNow) | CISO |
| Incident Management Policy | IMP-001 | [https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/incident-management-policy.md](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/incident-management-policy.md) | CISO |
| Data Classification Policy | DCP-001 | [https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/data-classification-policy.md](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/data-classification-policy.md) | CISO |
| Manufacturing BCP | BC-MFG-001 | Annex C (restricted; held by Operations Lead) | VP Manufacturing |
| IT Disaster Recovery Runbooks | IT-DR-RUN-001 onwards | Secure IT repository (restricted) | IT Recovery Lead |
| Incident Response Playbooks | IR-PLAY-001 onwards | Annex D (restricted; held by CISO) | CISO |

---

## 13. Evidence Index

The following evidence types are maintained to demonstrate ongoing compliance with ISO 22301:2019 and to support audit readiness. All records are retained for a minimum of 7 years, consistent with ISO 22301 documentation retention guidance [VERIFY].

| # | Evidence Type | Description | System of Record | Owner | Retention Period | Collection Frequency |
|---|---------------|-------------|-----------------|-------|-----------------|----------------------|
| 1 | Plan activation records | Log of all BCP activations including trigger, timestamp, CMT members notified, and deactivation confirmation | ServiceNow | BC Manager | 7 years | Per activation |
| 2 | Exercise reports | Written reports for all exercises per Section 9.3, including objectives, outcomes, findings, and remediation actions | GRC Document Repository | Exercise Owner | 7 years | Per exercise |
| 3 | Technical DR test results | RTO and RPO measurement data from live failover tests; system logs; pass/fail outcomes | ServiceNow + AWS CloudWatch export | IT Recovery Lead | 7 years | Semi-annual |
| 4 | Recovery time validation records | Timestamped logs confirming RTO and RPO achievement per function during exercises and real activations | ServiceNow | IT Recovery Lead | 7 years | Per exercise / activation |
| 5 | Supplier BCP attestations | Annual written confirmations from Tier 1 suppliers that their BCP is current, tested, and covers the services provided to Emyzer Technology | Vendor Risk Register (ServiceNow) | Vendor Risk Manager | 7 years | Annual |
| 6 | Plan review records | Signed annual review documentation confirming review scope, participants, changes made, and approval | GRC Document Repository | BC Manager | 7 years | Annual |
| 7 | CMT notification logs | Records of all CMT member notifications during activations and tests, with timestamps and delivery confirmations | ServiceNow | BC Manager | 7 years | Per activation / test |
| 8 | Customer notification records | Log of all customer notifications sent during incidents, including content, timestamp, and delivery confirmation | ServiceNow CRM | Communications Lead | 7 years | Per incident |
| 9 | Regulatory notification records | Records of all regulatory notifications made under GDPR Art.33, EU AI Act Art.73, or other obligations | Legal Management System | Legal Counsel | 7 years (or longer per regulatory requirement) [VERIFY] | Per incident |
| 10 | Finding remediation records | Evidence of closure for all Critical and Major exercise findings, including retesting confirmation | ServiceNow | BC Manager | 7 years | Per finding |
| 11 | CMT contact list version history | Archived versions of the CMT contact list, demonstrating currency at each distribution date | GRC Document Repository | BC Manager | 7 years | Annual / as changed |
| 12 | BCP distribution acknowledgements | Signed or email-confirmed receipt of BCP by all CMT members upon each major version release | GRC Document Repository | BC Manager | 7 years | Per major version |

---

## 14. Approval History

| Version | Date | Author | Changes | Approved By | Approval Date |
|---------|------|--------|---------|-------------|---------------|
| 0.1 (Draft) | 2024-07-01 | Susan Orwell, BC Manager | Initial draft for CMT review | — | — |
| 0.2 (Draft) | 2024-08-01 | Susan Orwell, BC Manager | Incorporated CMT review feedback; added Tier 2 procedures | — | — |
| 1.0 | 2024-09-01 | Susan Orwell, BC Manager | First approved version | Chief Executive Officer | 2024-09-01 |

---

## Document Control

| Attribute | Value |
|-----------|-------|
| **Document ID** | BC-PLAN-001 |
| **Version** | 1.0 |
| **Status** | Active |
| **Classification** | Restricted — Distribution Limited to Crisis Management Team and Named Alternates |
| **Owner** | Business Continuity Manager (Susan Orwell) |
| **Approved By** | Chief Executive Officer |
| **Effective Date** | 2024-09-01 |
| **Next Review** | 2025-09-01 |
| **Storage Location** | GRC Document Repository; Physical copies at Recovery Sites A and B |
| **Distribution** | CMT members and named alternates only — see distribution list held by BC Manager |

> This document is part of Emyzer Technology's Business Continuity Management System (BCMS) and is aligned to ISO 22301:2019 [VERIFY]. It must be reviewed annually and following any BCP activation, significant exercise finding, or material organisational change.

---

*BC-PLAN-001 v1.0 | Emyzer Technology | Business Continuity Management System | 2024-09-01*

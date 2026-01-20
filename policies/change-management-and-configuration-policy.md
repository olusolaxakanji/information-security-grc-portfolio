# Change Management and Configuration Policy

**Emyzer Technology: Governance, Risk, and Compliance**

---

## Policy Metadata

| Attribute | Value |
|-----------|-------|
| **Policy Name** | Change Management and Configuration Policy |
| **Type** | Policy |
| **Owner** | Information Security Officer (Susan Orwell) |
| **Owning Group** | App Engine Admins |
| **State** | Published |
| **Valid From** | 2026-01-13 |
| **Valid To** | 2027-01-13 |
| **Approvers** | Chief Information Security Officer |
| **Reviewers** | GRC Analyst |
| **Knowledge Base** | Governance, Risk, and Compliance |
| **Published Policy** | KB-PORTFOLIO-0009 |

---

## Description

This policy establishes a framework for managing changes to information systems, applications, infrastructure, and configurations to minimize service disruption, maintain system integrity, ensure security, and support operational stability.

**Impact:** Reduces unplanned outages and security incidents caused by unauthorized or poorly planned changes, maintains system integrity and availability, supports audit compliance through documented change history, and ensures configuration consistency across environments.

**Relevant Standards:** ISO/IEC 27001 (A.8.32), NIST SP 800-53 (CM-1 through CM-11, SA-10), ITIL 4 Change Enablement, COBIT 2019 (BAI06, BAI10)

---

## Policy Snapshot

| Dimension | Summary |
|-----------|---------|
| **Applies to** | All changes to production systems, applications, infrastructure, networks, databases, and security configurations |
| **Covers** | Change request, assessment, approval, implementation, verification, and documentation across all IT environments |
| **Change Types** | Standard (pre-approved), Normal (CAB review), Emergency (expedited), Major (executive approval) |
| **Review Cadence** | Annual policy review; weekly Change Advisory Board meetings; post-implementation reviews within 5 business days |
| **Key Governance** | Change Manager coordinates process; CAB reviews Normal/Major changes; ISO assesses security impact; IT Operations implements changes |
| **Exceptions Process** | Emergency change process for urgent situations; retrospective documentation within 24 hours; quarterly review of emergency changes |
| **Evidence Maintained** | Change requests, approvals, implementation records, test results, rollback documentation, configuration baselines (all with defined retention periods) |

---

## A. Purpose

To establish a structured framework for requesting, assessing, approving, implementing, and documenting changes to information systems and configurations. This policy ensures that changes are evaluated for risk, properly authorized, thoroughly tested, and carefully implemented to minimize service disruption, prevent security vulnerabilities, maintain system stability, and support regulatory compliance. Effective change management protects the organization from unplanned outages, security incidents, and compliance failures resulting from unauthorized or poorly controlled changes.

---

## B. Scope

This policy applies to all changes affecting:

- Production servers, workstations, and endpoints
- Network infrastructure (routers, switches, firewalls, load balancers)
- Cloud infrastructure and services (IaaS, PaaS, SaaS configurations)
- Applications and software (custom developed and commercial)
- Databases and data structures
- Security systems and configurations (firewalls, IDS/IPS, SIEM, antivirus)
- Identity and access management systems
- Middleware and integration platforms
- Storage systems and backup infrastructure
- Telecommunications and voice systems
- Physical infrastructure affecting IT systems (power, cooling, cabling)

**Environments covered:**
- Production environments (mandatory full process)
- Pre-production/staging environments (standard process)
- Development environments (lightweight process)
- Disaster recovery environments (aligned with production)

**Exclusions:** Routine operational tasks that do not alter system configuration (e.g., password resets, user provisioning for approved access requests, log reviews) are excluded from change management requirements.

---

## C. Definitions

1. **Change:** Any addition, modification, or removal of hardware, software, configuration, documentation, or process that could affect IT services.

2. **Change Request (CR):** A formal submission documenting a proposed change, including justification, impact assessment, implementation plan, and rollback procedures.

3. **Change Advisory Board (CAB):** A cross-functional group responsible for reviewing, assessing, and approving or rejecting change requests.

4. **Emergency Change Advisory Board (ECAB):** A subset of CAB members authorized to review and approve emergency changes outside normal CAB meetings.

5. **Configuration Item (CI):** Any component that needs to be managed to deliver an IT service, including hardware, software, documentation, and service components.

6. **Configuration Management Database (CMDB):** A repository containing information about configuration items and their relationships.

7. **Baseline:** A documented and approved configuration of a system or environment at a specific point in time, used as a reference for future changes.

8. **Rollback:** The process of reverting a system to its previous state following an unsuccessful change implementation.

9. **Change Window:** A designated time period during which changes may be implemented, typically during low-activity periods to minimize user impact.

10. **Forward Schedule of Change (FSC):** A schedule containing details of all approved changes and their planned implementation dates.

---

## D. Policy Statement

Emyzer Technology requires all changes to information systems and configurations to follow a controlled process that ensures proper assessment, authorization, testing, and documentation. To achieve this, the organization shall:

1. Require all changes to production systems to be submitted through the formal change request process **before** implementation.

2. Prohibit unauthorized changes to production systems; all changes must be documented and approved according to their classification.

3. Classify changes as Standard, Normal, Emergency, or Major based on risk, impact, and urgency.

4. Require risk and security impact assessments for all Normal, Emergency, and Major changes.

5. Convene the Change Advisory Board **weekly** to review and approve Normal and Major change requests.

6. Require testing in non-production environments before production implementation for all Normal and Major changes.

7. Maintain documented rollback procedures for all changes to enable rapid recovery if implementation fails.

8. Conduct post-implementation reviews **within 5 business days** for all Major changes and failed changes.

9. Maintain configuration baselines for all critical systems and validate configurations against baselines **quarterly**.

10. Document all changes in the CMDB and retain change records according to defined retention periods.

11. Review and update this policy **annually** to address evolving operational requirements and security threats.

---

## E. Change Classification

### E.1 Standard Changes

**Definition:** Pre-approved, low-risk changes that follow established procedures and have predictable outcomes.

**Characteristics:**
- Routine and repetitive
- Low risk with minimal potential for negative impact
- Well-documented procedures exist
- Outcomes are predictable and tested

**Examples:**
- Scheduled patch deployment per approved patch management process
- Addition of user accounts per approved access request
- Standard software installation from the approved software catalog
- Scheduled backup configuration changes
- Certificate renewals following documented procedures

**Approval:** Pre-approved by CAB; no individual approval required if procedures are followed.

**Documentation:** Logged in change management system; no formal change request required.

### E.2 Normal Changes

**Definition:** Changes that require assessment and approval through the standard change management process.

**Characteristics:**
- Moderate risk or impact
- Require planning and coordination
- May affect multiple systems or users
- Require testing before implementation

**Examples:**
- Application version upgrades
- Server hardware replacements
- Network configuration modifications
- Database schema changes
- New system deployments
- Security tool configuration changes

**Approval:** CAB approval required; implementation during approved change windows.

**Documentation:** Full change request with impact assessment, test plan, implementation plan, and rollback procedures.

### E.3 Emergency Changes

**Definition:** Changes required to resolve critical incidents or address imminent security threats that cannot wait for normal CAB review.

**Characteristics:**
- Urgent resolution of critical incidents
- Imminent security threat requiring immediate action
- Cannot wait for the scheduled CAB meeting
- Higher risk due to compressed timeline

**Examples:**
- Critical security patches for actively exploited vulnerabilities
- Fixes for production system outages
- Emergency firewall rule changes to block active attacks
- Critical database repairs
- Disaster recovery activations

**Approval:** ECAB approval (minimum two members: Change Manager plus ISO or IT Director); retrospective CAB review required.

**Documentation:** Abbreviated change request before implementation; full documentation within 24 hours of implementation.

### E.4 Major Changes

**Definition:** High-risk or high-impact changes requiring extensive planning, testing, and executive approval.

**Characteristics:**
- Significant potential for service disruption
- Affects critical business systems
- Requires an extended implementation window
- May require business process changes
- High financial or reputational risk if unsuccessful

**Examples:**
- Core infrastructure migrations
- ERP or critical application replacements
- Data center moves or consolidations
- Major network architecture changes
- Cloud platform migrations
- Mergers and acquisitions system integrations

**Approval:** CAB approval plus executive sponsor approval (CIO or CISO); formal project governance required.

**Documentation:** Comprehensive change request with detailed project plan, risk assessment, test results, communication plan, and executive sign-off.

### E.5 Change Classification Matrix

| Attribute | Standard | Normal | Emergency | Major |
|-----------|----------|--------|-----------|-------|
| **Risk Level** | Low | Medium | Variable | High |
| **Impact Scope** | Limited | Moderate | Variable | Significant |
| **Approval Authority** | Pre-approved | CAB | ECAB | CAB + Executive |
| **Lead Time** | None | 5 business days | Immediate | 15+ business days |
| **Testing Required** | Procedure-based | Yes | Best effort | Extensive |
| **Rollback Plan** | Standard procedure | Required | Required | Required + tested |
| **Post-Implementation Review** | Not required | If failed | Required | Required |

---

## F. Change Management Process

### F.1 Change Request Submission

All change requests shall include:

1. **Description:** Clear explanation of what is being changed and why.
2. **Business Justification:** Reason for the change and expected benefits.
3. **Risk Assessment:** Potential risks and their likelihood and impact.
4. **Security Impact Assessment:** Evaluation of security implications (completed by ISO for Normal/Major changes).
5. **Affected Systems:** List of configuration items and services affected.
6. **Implementation Plan:** Step-by-step implementation procedures with estimated duration.
7. **Test Plan:** Testing approach and acceptance criteria.
8. **Rollback Plan:** Procedures to revert changes if implementation fails.
9. **Communication Plan:** Stakeholders to be notified and timing.
10. **Requested Implementation Window:** Preferred date/time for implementation.

### F.2 Change Assessment

Upon submission, changes shall be assessed for:

1. **Completeness:** All required information provided.
2. **Risk Level:** Potential for service disruption, data loss, or security impact.
3. **Resource Requirements:** Personnel, tools, and time needed.
4. **Dependencies:** Relationships with other changes or systems.
5. **Conflicts:** Scheduling conflicts with other approved changes.
6. **Compliance Impact:** Regulatory or policy implications.

The Change Manager shall classify the change and route it for appropriate approval.

### F.3 Change Approval

| Change Type | Approval Process | Timeline |
|-------------|------------------|----------|
| Standard | Automatic (pre-approved) | Immediate |
| Normal | CAB review and approval | Weekly CAB meeting |
| Emergency | ECAB approval (2 members minimum) | Within 2 hours of request |
| Major | CAB approval + executive sponsor | Scheduled CAB + executive review |

**CAB Composition:**
- Change Manager (Chair)
- Information Security Officer
- IT Operations Manager
- Application Development Manager
- Network/Infrastructure Manager
- Business representatives (as needed based on change scope)

**Approval Criteria:**
- Business justification is valid
- Risk assessment is complete and acceptable
- Implementation and rollback plans are adequate
- Testing has been completed successfully
- Resources are available
- No unresolved conflicts with other changes

### F.4 Change Implementation

Approved changes shall be implemented according to the following requirements:

1. **Implementation Window:** Changes shall be implemented during approved change windows unless otherwise authorized.
   - Standard change window: Saturday 22:00 to Sunday 06:00 (local time)
   - Secondary window: Wednesday 22:00 to Thursday 02:00 (local time)
   - Emergency changes: As needed with ECAB approval

2. **Pre-Implementation:**
   - Verify all approvals are in place
   - Confirm resources and personnel are available
   - Validate rollback procedures are ready
   - Notify affected stakeholders
   - Create a backup/snapshot of affected systems

3. **Implementation:**
   - Follow the approved implementation plan
   - Document any deviations from the plan
   - Monitor system behavior during implementation
   - Execute verification tests

4. **Post-Implementation:**
   - Verify change was successful against acceptance criteria
   - Update CMDB with configuration changes
   - Notify stakeholders of completion
   - Close change request with implementation notes

### F.5 Change Verification

All changes shall be verified upon completion:

1. **Functional Testing:** Confirm the change achieves the intended outcome.
2. **Regression Testing:** Verify no unintended impacts to related systems.
3. **Security Validation:** Confirm security controls remain effective.
4. **Performance Verification:** Validate system performance meets requirements.
5. **User Acceptance:** Obtain business confirmation for user-facing changes.

### F.6 Rollback Execution

If verification fails or critical issues are discovered:

1. Change implementer initiates rollback within **30 minutes** of failure determination.
2. Follow documented rollback procedures.
3. Notify Change Manager and affected stakeholders.
4. Document rollback actions and outcomes.
5. Restore the system to the previous baseline.
6. Conduct failed change review within **24 hours**.

### F.7 Post-Implementation Review

Post-implementation reviews shall be conducted:

- **Required for:** All Major changes, all failed changes, all Emergency changes
- **Timeline:** Within 5 business days of implementation
- **Participants:** Change owner, implementers, Change Manager, affected stakeholders

**Review shall document:**
- Whether the change achieved objectives
- Any issues encountered during implementation
- Lessons learned and improvement opportunities
- Updates to procedures or documentation
- Recommendations for future similar changes

---

## G. Configuration Management

### G.1 Configuration Management Database (CMDB)

The organization shall maintain a CMDB containing:

1. **Configuration Items:** Hardware, software, documentation, and service components.
2. **CI Attributes:** Ownership, location, status, version, relationships.
3. **Relationships:** Dependencies and connections between CIs.
4. **Change History:** Record of changes affecting each CI.

**CMDB Maintenance:**
- Updates within **24 hours** of change implementation
- Quarterly accuracy audits (target: 95% accuracy)
- Annual comprehensive CMDB review and reconciliation

### G.2 Configuration Baselines

Baselines shall be established and maintained for:

1. **Operating Systems:** Standard build configurations for servers and workstations.
2. **Network Devices:** Standard configurations for routers, switches, and firewalls.
3. **Security Systems:** Configurations for security tools and controls.
4. **Applications:** Standard deployment configurations for business applications.
5. **Cloud Resources:** Infrastructure-as-code templates for cloud deployments.

**Baseline Requirements:**
- Document and approve baselines before deployment
- Store baselines in a version-controlled repository
- Review and update baselines **quarterly** or upon significant changes
- Validate production configurations against baselines **quarterly**

### G.3 Configuration Hardening

All systems shall be configured according to security hardening standards:

1. **Hardening Guides:** CIS Benchmarks, vendor security guides, or organizational standards.
2. **Default Credentials:** Remove or change all default passwords and accounts.
3. **Unnecessary Services:** Disable or remove services not required for system function.
4. **Security Settings:** Enable logging, encryption, and access controls per classification.
5. **Patch Levels:** Maintain current patch levels per patch management policy.

**Hardening Validation:**
- Automated scanning **monthly** for critical systems
- Manual review **quarterly** for systems not supporting automated scanning
- Remediation of deviations within **30 days** (critical: 7 days)

### G.4 Configuration Drift Detection

The organization shall monitor for unauthorized configuration changes:

1. **Automated Monitoring:** Deploy tools to detect configuration changes in real-time.
2. **Baseline Comparison:** Compare current configurations to approved baselines.
3. **Alert Generation:** Generate alerts for unauthorized or unexpected changes.
4. **Investigation:** Investigate detected drift within **24 hours**.
5. **Remediation:** Restore unauthorized changes to baseline or document as approved exception.

---

## H. Roles and Responsibilities

### H.1 Chief Information Security Officer (CISO)
Provides executive oversight of security-related change management. Shall approve Major changes affecting security infrastructure. Shall serve on ECAB for emergency security-related changes. Shall review change management metrics **quarterly** as part of security program oversight.

### H.2 Information Security Officer (ISO)
Shall assess security impact for all Normal, Emergency, and Major changes. Shall participate in CAB meetings and ECAB as needed. Shall validate security configurations and hardening compliance. Shall review security-related changes and configuration drift reports **monthly**.

### H.3 Change Manager
Shall coordinate the end-to-end change management process. Shall chair CAB meetings and facilitate ECAB approvals. Shall maintain the Forward Schedule of Change. Shall report change management metrics to leadership **monthly**. Shall ensure change documentation is complete and accurate.

### H.4 Change Advisory Board (CAB)
Shall meet **weekly** to review and approve Normal and Major change requests. Shall assess change risk, impact, and readiness. Shall resolve scheduling conflicts between changes. Shall review failed changes and emergency changes retrospectively.

### H.5 Emergency Change Advisory Board (ECAB)
Shall be available to review emergency changes **24/7**. Shall consist of a minimum of two members: a Change Manager and an ISO or IT Director. Shall approve or reject emergency changes within **2 hours** of request. Shall ensure emergency changes are documented within **24 hours**.

### H.6 IT Operations
Shall implement approved changes in accordance with documented plans. Shall maintain and update the CMDB within **24 hours** of changes. Shall monitor systems during and after change implementation. Shall execute rollback procedures when required.

### H.7 Application Development
Shall submit change requests for application deployments. Shall provide test results and deployment documentation. Shall support implementation and troubleshooting. Shall participate in post-implementation reviews.

### H.8 Change Requesters
Shall submit complete and accurate change requests. Shall provide business justification and impact assessment. Shall coordinate testing and obtain necessary approvals. Shall participate in post-implementation reviews for their changes.

---

## I. Compliance and Monitoring

### I.1 Change Management Metrics

| Metric | Target | Measurement Frequency |
|--------|--------|----------------------|
| Change success rate | ≥95% | Monthly |
| Unauthorized changes detected | 0 | Monthly |
| Emergency change percentage | <10% of total changes | Monthly |
| Changes implemented on schedule | ≥90% | Monthly |
| Post-implementation reviews completed on time | 100% | Monthly |
| CMDB accuracy | ≥95% | Quarterly |
| Configuration baseline compliance | ≥95% | Quarterly |
| Average change lead time (Normal) | <7 days | Monthly |

### I.2 Monitoring Activities

- **Daily:** Review of change implementation results and pending approvals
- **Weekly:** CAB meeting; review of change schedule and conflicts
- **Monthly:** Change management metrics reporting; unauthorized change investigation
- **Quarterly:** CMDB accuracy audit; baseline compliance review; process improvement review
- **Annual:** Policy effectiveness review; process maturity assessment

### I.3 Non-Compliance

Non-compliance with this policy shall be addressed through:

- **Unauthorized Changes:** Immediate investigation; disciplinary action; remediation or rollback
- **Incomplete Documentation:** Change request returned; mandatory completion before approval
- **Bypassing Approval:** Escalation to management; documented warning; repeat violations result in disciplinary action
- **Failed Changes Without Review:** Mandatory post-implementation review; process improvement actions

---

## J. Policy Exceptions

### J.1 Exception Request Process
Stakeholders requiring deviation from standard change management procedures shall:
1. Submit exception requests via **ServiceNow GRC workflow** with detailed business justification and risk assessment.
2. Obtain approval from the Change Manager for minor procedural exceptions or the CISO for security-related exceptions.
3. Document compensating controls implemented during the exception period.
4. Accept exceptions valid for a maximum of **90 days** unless formally renewed.

### J.2 Emergency Change Exception
Emergency changes represent a pre-approved exception to normal timelines. Emergency changes shall:
- Be limited to resolving critical incidents or imminent security threats
- Receive ECAB approval before implementation (minimum 2 members)
- Be documented fully within **24 hours** of implementation
- Undergo retrospective CAB review at next scheduled meeting
- Be tracked and reported monthly; excessive emergency changes trigger process review

### J.3 Exception Governance
- All active exceptions shall be reviewed **quarterly** by the Change Manager.
- Exception renewals shall require updated business justification.
- Exception tracking shall be maintained in the GRC platform with status updates provided to leadership **monthly**.

---

## K. Related Policies

This policy is supported by and supports the following policies:

1. [**Information Security Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/information-security-policy.md): Parent policy establishing the ISMS framework and governance structure.

2. [**Access Control Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/access-control-policy.md): Defines access requirements for systems and change management tools.

3. [**Incident Management Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/incident-management-policy.md): Defines incident response procedures that may trigger emergency changes.

4. [**Risk Management Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/risk-management-policy.md): Integrates change risk assessment into enterprise risk management.

5. [**Business Continuity and Disaster Recovery Policy**](https://github.com/olusolaxakanji/information-security-grc-portfolio/blob/main/policies/bcdr-policy.md): Defines continuity requirements affecting change scheduling and rollback.

6. **Patch Management Policy**: Defines specific procedures for security and software patches (subset of change management).

---

## L. Related Documents

1. Change Request Form Template
2. Change Advisory Board Charter
3. Standard Change Catalog
4. Emergency Change Procedures
5. Configuration Management Database Schema
6. System Hardening Standards (CIS Benchmarks)
7. Rollback Procedure Templates
8. Post-Implementation Review Template

---

## M. Review and Revision

This policy shall be reviewed **annually** or when significant changes occur (major incidents caused by changes, regulatory updates, organizational restructuring, technology changes) to ensure continued relevance and effectiveness. The Change Manager shall assess policy effectiveness based on change success rates, incident trends, and audit findings. All revisions require CISO approval and notification to executive leadership.

---

## N. Framework Alignment

| Framework | Alignment |
|-----------|-----------|
| **ISO/IEC 27001** | A.8.32 (Change management), A.8.9 (Configuration management), A.8.19 (Installation of software on operational systems), A.8.31 (Separation of development, test and production environments) |
| **NIST SP 800-53** | CM-1 (Policy and Procedures), CM-2 (Baseline Configuration), CM-3 (Configuration Change Control), CM-4 (Impact Analyses), CM-5 (Access Restrictions for Change), CM-6 (Configuration Settings), CM-7 (Least Functionality), CM-8 (System Component Inventory), CM-9 (Configuration Management Plan), SA-10 (Developer Configuration Management) |
| **NIST Cybersecurity Framework** | PR.IP-1 (Baseline configuration), PR.IP-3 (Configuration change control), PR.DS-7 (Development and testing separate from production), DE.CM-7 (Monitoring for unauthorized changes) |
| **ITIL 4** | Change Enablement practice; Service Configuration Management practice |
| **COBIT 2019** | BAI06 (Manage IT Changes), BAI10 (Manage Configuration) |
| **PCI DSS v4.0** | Requirement 6.4 (Change control processes), Requirement 6.5 (Address vulnerabilities in development) |
| **SOC 2** | CC8.1 (Change management), CC6.1 (Logical and physical access controls for changes) |

**Note:** This policy aligns with these standards; specific implementation controls are documented in the Change Management Procedures Manual.

---

## O. Organizational Benefit

| Benefit Area | Description |
|--------------|-------------|
| **Service Stability** | Structured change process reduces unplanned outages and service disruptions |
| **Security Posture** | Security impact assessments prevent changes that introduce vulnerabilities |
| **Audit Compliance** | Documented change history and approvals demonstrate control to auditors and regulators |
| **Operational Efficiency** | Standardized processes reduce implementation errors and rework |
| **Risk Reduction** | Risk assessment and testing requirements minimize failed changes |
| **Accountability** | Clear approval workflows establish ownership and responsibility for changes |
| **Configuration Integrity** | Baseline management and drift detection maintain known-good configurations |
| **Incident Prevention** | Controlled changes reduce incidents caused by unauthorized or untested modifications |

---

## P. Evidence of Compliance

The organization shall maintain the following compliance evidence with defined retention periods:

### Evidence Index

| Evidence Type | System of Record | Owner | Retention Period |
|---------------|------------------|-------|------------------|
| Change Requests | ServiceNow / Change Management System | Change Manager | 5 years |
| CAB Meeting Minutes | Document Repository | Change Manager | 5 years |
| Approval Records | Change Management System | Change Manager | 5 years |
| Implementation Logs | Change Management System / ITSM | IT Operations | 3 years |
| Test Results | Change Management System | Change Requester | 3 years |
| Rollback Documentation | Change Management System | IT Operations | 3 years |
| Post-Implementation Reviews | Document Repository | Change Manager | 5 years |
| Configuration Baselines | Version Control / CMDB | IT Operations | Indefinite (current + 2 prior versions) |
| CMDB Records | CMDB | IT Operations | Indefinite |
| Drift Detection Reports | Security Tools | Information Security | 1 year |
| Compliance Audit Reports | GRC Platform | Information Security | 5 years |

---

### P.1 Change Request Evidence
- **Change Request Records:** Complete change requests documenting description, justification, risk assessment, implementation plan, test plan, and rollback procedures. Retained for 5 years.
- **Security Impact Assessments:** ISO assessments of security implications for Normal, Emergency, and Major changes. Retained for 5 years.
- **Business Justifications:** Documented business need and expected benefits for each change. Retained for 5 years.

### P.2 Approval Evidence
- **CAB Meeting Minutes:** Records of CAB discussions, decisions, and voting for change approvals. Retained for 5 years.
- **Approval Workflows:** System records showing approval chain, approvers, timestamps, and decisions. Retained for 5 years.
- **ECAB Approvals:** Documentation of emergency change approvals, including approvers and rationale. Retained for 5 years.
- **Executive Approvals:** Sign-offs from executive sponsors for Major changes. Retained for 5 years.

### P.3 Implementation Evidence
- **Implementation Logs:** Step-by-step records of change implementation activities, including timestamps and personnel involved. Retained for 3 years.
- **Deviation Documentation:** Records of any deviations from approved implementation plans. Retained for 3 years.
- **Verification Results:** Evidence of functional, regression, and security testing following implementation. Retained for 3 years.
- **Stakeholder Notifications:** Records of communications to affected parties before and after changes. Retained for 3 years.

### P.4 Rollback Evidence
- **Rollback Procedures:** Documented rollback plans for each change, tested where required. Retained for 3 years.
- **Rollback Execution Records:** Documentation of rollback activities when changes fail, including actions taken and outcomes. Retained for 5 years.
- **System Backups/Snapshots:** Evidence of pre-change backups or snapshots enabling rollback. Retained per backup retention schedule.

### P.5 Post-Implementation Review Evidence
- **PIR Reports:** Completed post-implementation review documentation for Major, failed, and emergency changes. Retained for 5 years.
- **Lessons Learned:** Documented improvement opportunities and corrective actions from PIRs. Retained for 5 years.
- **Failed Change Analysis:** Root cause analysis for changes that did not achieve intended outcomes. Retained for 5 years.

### P.6 Configuration Management Evidence
- **CMDB Records:** Current and historical configuration item data, relationships, and change history. Retained indefinitely for current state; historical changes retained for 5 years.
- **Configuration Baselines:** Approved baseline configurations for operating systems, applications, and infrastructure. Current version plus 2 prior versions retained.
- **Baseline Compliance Reports:** Quarterly validation of production configurations against approved baselines. Retained for 3 years.
- **Drift Detection Alerts:** Records of detected configuration drift, investigation results, and remediation actions. Retained for 1 year.

### P.7 Metrics and Governance Evidence
- **Change Management Metrics:** Monthly reports on change success rate, emergency change percentage, lead times, and compliance. Retained for 3 years.
- **Forward Schedule of Change:** Weekly schedules of approved changes and implementation windows. Retained for 1 year.
- **Audit Reports:** Internal and external audit findings related to change management and configuration controls. Retained for 5 years.
- **Exception Records:** Approved exceptions to change management procedures with justification and compensating controls. Retained for exception duration plus 3 years.

---

## Approval History

| Date | Approver | Status | Comments |
|------|----------|--------|----------|
| 2026-01-13 | Chief Information Security Officer | Approved | "Comprehensive change management framework that balances operational agility with appropriate controls. The tiered approach ensures rigor where needed while enabling efficient handling of routine changes. Approved for implementation." |

---

## Document Control

- **Document ID:** KB-PORTFOLIO-0009
- **Version:** 1.0
- **Classification:** Internal
- **Last Updated:** 2026-01-13
- **Next Review Date:** 2027-01-13

---

*This policy document was generated from ServiceNow GRC and formatted for portfolio presentation.*

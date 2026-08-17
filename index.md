---
layout: default
title: "GRC Portfolio: Olusola B. Akanji"
permalink: /
---

# Olusola B. Akanji
**Information Security and GRC Professional**

![Olusola B. Akanji]({{ site.baseurl }}/assets/images/headshot.jpg){: style="float: right; margin: 0 0 1.5em 1.5em; width: 150px; border-radius: 6px;"}

I design and build information security governance programmes. The first is a live GRC programme I built and maintain as Compliance Officer for the Idowu Ajiri Foundation, a US-Nigeria nonprofit operating under five simultaneous regulatory frameworks across two jurisdictions. The second is an end-to-end case study built in ServiceNow GRC: Emyzer Technology acquires Veridian AI and forms Emyzer Nexus, navigating EU AI Act compliance for inherited High-Risk AI systems alongside M&A policy integration. Every artefact in both programmes has an evidence index, a framework mapping, and documented open gaps.

[GitHub](https://github.com/olusolaxakanji) · [LinkedIn](https://www.linkedin.com/in/olusola-b-akanji/) · [GRC Writing](https://akanjitechnicalwriting.com/blog)

---

[![NIST CSF 2.0](https://img.shields.io/badge/NIST_CSF_2.0-003366?style=flat-square)](https://www.nist.gov/cyberframework)
[![ISO 27001](https://img.shields.io/badge/ISO_27001%3A2022-1A73E8?style=flat-square)](https://www.iso.org/standard/82875.html)
[![ISO 22301](https://img.shields.io/badge/ISO_22301%3A2019-1A73E8?style=flat-square)](https://www.iso.org/standard/75106.html)
[![SOC 2](https://img.shields.io/badge/SOC_2_Type_II-2D7D46?style=flat-square)](https://www.aicpa-cima.com/resources/landing/system-and-organization-controls-soc-suite-of-services)
[![EU AI Act](https://img.shields.io/badge/EU_AI_Act-FF6B35?style=flat-square)](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32024R1689)
[![GDPR](https://img.shields.io/badge/GDPR-FF6B35?style=flat-square)](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32016R0679)
[![NIST AI RMF](https://img.shields.io/badge/NIST_AI_RMF-003366?style=flat-square)](https://www.nist.gov/artificial-intelligence/ai-risk-management-framework)
[![ServiceNow GRC](https://img.shields.io/badge/ServiceNow_GRC-00C7B7?style=flat-square)](https://www.servicenow.com/products/governance-risk-and-compliance.html)

---

## Live Programme: Idowu Ajiri Foundation

**[View the programme repository →](https://github.com/olusolaxakanji/idowu-ajiri-grc-program)**

This is not a simulation. The Idowu Ajiri Foundation is a nonprofit in pre-operational [IRS 501(c)(3)](https://www.irs.gov/charities-non-profits) formation in the United States and registered with the [Corporate Affairs Commission (CAC)](https://www.cac.gov.ng) in Nigeria. I built this programme and maintain it as Compliance Officer. The conflict-of-interest disclosure memo in the repository is in my name.

The Nigerian entity is active under CAC registration. The US entity is in pre-operational formation under IRS 501(c)(3). The compliance programme covers both jurisdictions proactively: governance architecture was built ahead of full US operational activity, not after it became urgent.

The regulatory environment creates specific compliance problems that a single-jurisdiction programme cannot solve. OFAC sanctions screening must cover donors, vendors, and grantees across both countries. SCUML classifies Nigerian nonprofits as Designated Non-Financial Businesses and Professions, which triggers formal AML/CFT obligations most NGOs are not prepared for. Cross-border fund flows create simultaneous CBN and FinCEN exposure. The Nigeria Data Protection Act and US state privacy laws apply to the same donor records.

| Framework | Governing Body | Jurisdiction |
|---|---|---|
| [IRS 501(c)(3) Tax-Exempt Compliance](https://www.irs.gov/charities-non-profits) | [Internal Revenue Service](https://www.irs.gov/) | United States |
| [Corporate Affairs Commission (CAC)](https://www.cac.gov.ng) | [CAC Nigeria](https://www.cac.gov.ng) | Nigeria |
| [SCUML / NFIU: AML/CFT](https://www.nfiu.gov.ng) | [Nigerian Financial Intelligence Unit](https://www.nfiu.gov.ng) | Nigeria |
| [Nigeria Data Protection Act 2023](https://ndpc.gov.ng) | [Nigeria Data Protection Commission](https://ndpc.gov.ng) | Nigeria |
| [OFAC Sanctions Compliance](https://ofac.treas.gov) | [U.S. Dept. of the Treasury: OFAC](https://ofac.treas.gov) | United States (cross-border) |

**What I built:**

- A full control framework mapped to US (OFAC, FinCEN, FCPA, state charity registration) and Nigerian (SCUML, CBN, EFCC, CAC) obligations
- 11 governance policies across three tiers: global, US-specific, and Nigeria-specific
- A 10-entry master risk register with two HIGH risks (OFAC sanctions exposure, SCUML deregistration) escalated to the board quarterly
- OFAC and SCUML-integrated donor, vendor, and grantee screening with exception logging
- Quarterly board compliance reports with control testing results, risk register summaries, and upcoming regulatory deadline tracking
- Jurisdiction-specific AML/CFT programs aligned to FinCEN 31 CFR Part 1010 (US) and SCUML obligations (Nigeria)

---

## Case Study: Emyzer Technology and Emyzer Nexus

**[View the case study repository →](https://github.com/olusolaxakanji/information-security-grc-portfolio)**

This case study models a governance problem that GRC teams face regularly: an acquisition closes and the acquired entity has no formal compliance programme. Emyzer Technology acquires Veridian AI, an AI-native startup with two production AI systems that had never been assessed under the EU AI Act. Phase 2 covers what happens next: classifying inherited High-Risk systems, closing GDPR data processor gaps, establishing a post-acquisition policy hierarchy, and maintaining policy continuity through the integration.

Phase 1 built the foundational GRC programme for Emyzer Technology before the acquisition. Phase 2 is the Emyzer Nexus parent entity programme after it. Both phases were built and implemented in ServiceNow GRC.

| Section | Contents | Frameworks |
|---|---|---|
| **[Controls Library →](https://github.com/olusolaxakanji/information-security-grc-portfolio/tree/main/controls)** | 8 operational controls with testing procedures, cadence definitions, and evidence indexes — covering access management (CC6), incident response (CC7), change management (CC8), vendor risk (CC9), and additional Common Criteria categories | NIST CSF 2.0, ISO 27001, SOC 2 TSC |
| **[Policies →](https://github.com/olusolaxakanji/information-security-grc-portfolio/tree/main/policies)** | 10 Phase 1 enterprise security policies implemented in ServiceNow GRC, plus 4 Phase 2 AI governance policies — policy library, evidence indexes, and version control structures aligned to SOC 2 audit requirements | ISO 27001, SOC 2 TSC, EU AI Act, GDPR |
| **[Risk Assessments →](https://github.com/olusolaxakanji/information-security-grc-portfolio/tree/main/risk-assessments)** | Hybrid 5x5 risk methodology, 15-entry asset register with one budget-blocked Critical risk documented at actual status, and a risk appetite statement | ISO 31000, NIST SP 800-30 |
| **[Business Continuity →](https://github.com/olusolaxakanji/information-security-grc-portfolio/tree/main/business-continuity)** | Business Impact Analysis and a full Business Continuity Plan with activation criteria, CMT runbook, five recovery scenarios, and exercise programme | ISO 22301, NIST SP 800-34 |
| **[AI Governance →](https://github.com/olusolaxakanji/information-security-grc-portfolio/tree/main/ai-governance)** | EU AI Act Articles 9-15, 72, 73 control mapping; system inventory for two inherited AI systems; 8-risk assessment with 2 Critical findings | EU AI Act, NIST AI RMF, ISO 42001 |
| **[Veridian AI →](https://github.com/olusolaxakanji/information-security-grc-portfolio/tree/main/veridian-ai)** | Due diligence risk assessment at acquisition (4 Critical findings, governance maturity Level 1) and AI Vendor Due Diligence Addendum | EU AI Act, GDPR, NIST AI RMF |

---

## Competencies

| Competency | Evidence in this portfolio |
|---|---|
| **Live compliance programme management** | IAF dual-jurisdiction programme: active OFAC and SCUML screening, AML/CFT programmes for two regulatory regimes, board-level reporting, active Compliance Officer role |
| **Nonprofit and cross-border compliance** | Dual-jurisdiction AML/CFT under FinCEN and SCUML. OFAC sanctions screening. CBN fund management. IRS 501(c)(3) compliance posture built before US operations begin. |
| **AI governance** | EU AI Act article-by-article control mapping (Articles 9-15, 72, 73); High-Risk classification of two inherited systems; 8-entry AI risk assessment with 2 Critical findings |
| **M&A GRC integration** | Integration Charter establishing Day-0 policy hierarchy; Rationalization Roadmap tracking policy updates; 15-entry M&A risk register with treatment owners |
| **Risk programme design** | End-to-end hybrid methodology; 15-entry asset register with a budget-blocked Critical risk documented at actual status; domain-specific risk appetite thresholds |
| **Security policy development and SOC 2 alignment** | 14 enterprise security policies (10 Phase 1 + 4 Phase 2) with evidence indexes, framework tables, and ServiceNow platform exports — policy library structure aligned to SOC 2 Type II audit requirements across Common Criteria categories CC1-CC9 |
| **Business continuity** | Full ISO 22301 BCP with CMT runbook, 5-scenario recovery strategies, multi-type exercise programme, and clause-level framework alignment |
| **GRC platform proficiency** | Policies, risk registers, and compliance workflows built in ServiceNow GRC; raw PDF platform exports as direct evidence |

---

> **Practitioner disclaimer.** The Emyzer Technology, Emyzer Nexus, and Veridian AI case study is fictional. All personnel, systems, risk entries, vendor relationships, and regulatory scenarios in it are invented. Framework references are accurate as of the document publication dates. `[VERIFY]` tags flag regulatory citations that require legal confirmation before use in a real context. The Idowu Ajiri Foundation is a real organisation; that section documents live, operational work.

---

[View full portfolio repository on GitHub →](https://github.com/olusolaxakanji/information-security-grc-portfolio)

# Risk Assessment Methodology

| Field | Value |
|---|---|
| Document ID | RAM-001 |
| Version | 1.1 |
| Status | Approved |
| Owner | GRC Analyst |
| Approved By | Information Security Officer |
| Effective Date | January 2026 |
| Next Review | January 2027 |

---

## 1. Purpose

This document defines the organization's methodology for identifying, analyzing, evaluating, and treating information security risks. It establishes a repeatable, consistent approach that supports compliance with HIPAA, FERPA, NIST CSF, and ISO 27001 requirements.

---

## 2. Scope

This methodology applies to:
- All information assets that process, store, or transmit organizational data (including ePHI and student records)
- All systems, applications, infrastructure, and third-party services in scope
- All risk assessment activities conducted by internal staff or external assessors

---

## 3. Risk Assessment Framework

This methodology aligns with:
- **NIST SP 800-30 Rev. 1** — Guide for Conducting Risk Assessments
- **ISO/IEC 27005** — Information Security Risk Management
- **HIPAA Security Rule** — 45 CFR § 164.308(a)(1) — Security Management Process

---

## 4. Risk Assessment Process

### Phase 1: Scope and Context

Before beginning any risk assessment, define:

| Input | Description |
|---|---|
| Assessment Scope | Systems, processes, or organizational units being assessed |
| Data Types In Scope | PHI, PII, student records, financial data, etc. |
| Regulatory Context | Applicable regulations (HIPAA, FERPA, SOX, etc.) |
| Assessment Trigger | Scheduled annual review, system change, incident, new vendor |
| Assessment Owner | GRC Analyst or delegated assessor |

Document the scope in the Risk Assessment Scope Statement prior to data collection.

---

### Phase 2: Asset Inventory and Threat Identification

**Step 1 — Build Asset Inventory**

Identify all in-scope information assets:

| Asset Category | Examples |
|---|---|
| Hardware | Servers, workstations, laptops, mobile devices, network equipment |
| Software | EHR systems, SIS platforms, email, cloud services, custom applications |
| Data | ePHI, PII, student records, financial data, credentials |
| People | Employees, contractors, vendors, students |
| Facilities | Data centers, server rooms, remote work locations |

Assign each asset:
- A unique asset ID
- A data classification level (Public / Internal / Confidential / Restricted)
- A designated data owner
- A criticality rating (Critical / High / Medium / Low)

**Step 2 — Identify Threat Sources**

For each asset, identify applicable threat sources:

| Threat Category | Examples |
|---|---|
| External Adversary | Hackers, nation-state actors, organized crime, phishing campaigns |
| Internal Threat | Disgruntled employee, negligent user, contractor with excessive access |
| Environmental | Natural disaster, power failure, hardware failure |
| Third Party | Vendor breach, misconfigured cloud service, supply chain compromise |

**Step 3 — Identify Threat Events**

Map threat events to each asset:
- Unauthorized access to ePHI via compromised credentials
- Ransomware deployment encrypting critical servers
- Accidental disclosure of student records via misdirected email
- Data exfiltration via unencrypted portable device
- Exploitation of unpatched vulnerability
- Social engineering / phishing of workforce member

---

### Phase 3: Vulnerability Assessment

For each threat-asset pair, identify existing vulnerabilities:

| Vulnerability Type | Assessment Method |
|---|---|
| Technical vulnerabilities | Vulnerability scanning (Qualys), penetration testing results, patch status |
| Configuration weaknesses | Security baseline review, CIS Benchmark comparison |
| Process gaps | Policy review, control testing, audit findings |
| Training gaps | Training completion records, phishing simulation results |
| Third-party weaknesses | Vendor questionnaire, BAA review, prior incident history |

---

### Phase 4: Likelihood and Impact Analysis

**Likelihood Scoring**

| Score | Level | Criteria |
|---|---|---|
| 1 | Rare | Threat is theoretically possible but no known occurrence; strong controls in place |
| 2 | Unlikely | Limited historical occurrence; controls reduce probability significantly |
| 3 | Possible | Occurs periodically in the industry; controls partially effective |
| 4 | Likely | Occurs regularly in the industry; controls have gaps |
| 5 | Almost Certain | Occurs frequently; minimal or ineffective controls |

**Impact Scoring**

| Score | Level | Criteria |
|---|---|---|
| 1 | Negligible | No operational impact, no regulatory consequence, no data exposure |
| 2 | Minor | Limited impact, manageable internally, no regulatory notification required |
| 3 | Moderate | Noticeable operational disruption, possible regulatory attention, limited data exposure |
| 4 | Major | Significant financial, operational, or reputational harm; regulatory notification likely |
| 5 | Critical | Severe harm to individuals or organization; mandatory regulatory reporting; potential litigation |

**Inherent Risk Score = Likelihood × Impact**

| Score Range | Rating | Description |
|---|---|---|
| 1–4 | Low | Acceptable risk; monitor annually |
| 5–9 | Medium | Mitigation recommended; quarterly review |
| 10–15 | High | Immediate mitigation plan required |
| 16–25 | Critical | Escalate to leadership; immediate executive action |

---

### Phase 5: Control Evaluation

For each identified risk, evaluate existing controls:

**Control Categories:**

| Category | Description | Examples |
|---|---|---|
| Preventive | Stop the threat from occurring | MFA, encryption, firewall rules, access controls |
| Detective | Identify when a threat event occurs | SIEM alerts, log review, IDS/IPS, audit logging |
| Corrective | Reduce impact after occurrence | Incident response plan, backup and recovery, patch management |
| Administrative | Policy and process controls | Security awareness training, access review procedures, vendor agreements |

**Control Effectiveness Rating:**

| Rating | Description |
|---|---|
| Fully Effective | Control consistently applied and tested; significant risk reduction |
| Partially Effective | Control in place but inconsistently applied or not tested |
| Not Effective | Control documented but not implemented or confirmed non-functional |
| Not Present | No control exists for this risk |

---

### Phase 6: Residual Risk Scoring

After evaluating controls, assign residual risk:

**Residual Likelihood** = Inherent Likelihood adjusted down based on control effectiveness
**Residual Impact** = Inherent Impact adjusted down based on corrective controls
**Residual Risk Score** = Residual Likelihood × Residual Impact

If residual risk exceeds acceptable thresholds, a risk treatment action is required.

---

### Phase 7: Risk Treatment Selection

For each risk, select a treatment strategy:

| Strategy | Description | When to Use |
|---|---|---|
| Mitigate | Implement controls to reduce likelihood or impact | Risk is above acceptable threshold; control is cost-effective |
| Accept | Document and accept the risk at current level | Residual risk is Low or Medium; cost to mitigate exceeds benefit |
| Transfer | Shift risk to a third party (insurance, contract) | Financial risk that can be covered by cyber insurance or contractual indemnification |
| Avoid | Eliminate the activity or asset creating the risk | Risk is too high and cannot be mitigated to acceptable level |

---

### Phase 8: Risk Treatment Planning

For each risk requiring mitigation or corrective action, document:

| Field | Description |
|---|---|
| Risk ID | Unique identifier from the risk register |
| Treatment Action | Specific control improvement or remediation step |
| Responsible Owner | Person or team accountable for implementation |
| Target Completion Date | Deadline for treatment completion |
| Priority | Critical / High / Medium / Low (based on residual risk score) |
| Status | Not Started / In Progress / Completed / Deferred |
| Verification Method | How completion will be confirmed (audit, scan, policy review) |

---

### Phase 9: Documentation and Reporting

All risk assessments must produce the following artifacts:

| Deliverable | Description |
|---|---|
| Risk Assessment Report | Summary of methodology, findings, and recommendations |
| Risk Register | Itemized list of all identified risks with scores and treatment plans |
| Risk Heatmap | Visual representation of risks by likelihood and impact |
| Executive Summary | Non-technical summary for leadership review |
| Evidence Package | Supporting documentation (scan results, control test evidence, asset inventory) |

---

### Phase 10: Review and Continuous Monitoring

Risk assessments are not one-time events. Reassessment is required:

| Trigger | Action |
|---|---|
| Annual cycle | Full risk assessment for all in-scope systems |
| Significant system change | Scoped reassessment for affected systems |
| Security incident | Post-incident risk review; update affected risk entries |
| New regulation or audit finding | Review of compliance-related risks |
| New third-party vendor | Vendor-specific risk assessment prior to onboarding |
| Change in threat landscape | Update threat identification for affected risk categories |

---

## 5. Roles and Responsibilities

| Role | Responsibility |
|---|---|
| GRC Analyst | Facilitate risk assessment process, maintain risk register, produce reports |
| Information Security Officer | Approve risk register, set risk tolerance thresholds, escalate critical risks |
| IT Department | Provide technical findings, validate control status, implement mitigation actions |
| Data Owners | Provide asset classification, validate threat scenarios for their assets |
| Compliance Officer | Ensure regulatory alignment, coordinate external audit findings |
| Executive Leadership | Review critical and high risks; approve risk acceptance decisions |

---

## 6. Risk Tolerance Thresholds

| Risk Rating | Treatment Requirement | Escalation Required |
|---|---|---|
| Critical (16–25) | Immediate executive action | Yes — C-suite and Board |
| High (10–15) | Mitigation plan within 30 days | Yes — Information Security Officer |
| Medium (5–9) | Mitigation plan within 90 days | No — GRC Analyst manages |
| Low (1–4) | Annual review; accept if justified | No — Document acceptance |

---

## Version History

| Version | Date | Author | Changes |
|---|---|---|---|
| 1.0 | January 2025 | B. Santiago | Initial draft |
| 1.1 | January 2026 | B. Santiago | Expanded control evaluation section, added residual risk guidance |

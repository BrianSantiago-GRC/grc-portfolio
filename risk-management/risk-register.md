# Risk Register

**Organization:** Sample Organization (Healthcare/Education Sector)
**Last Review:** March 2026
**Owner:** GRC Analyst
**Classification:** Internal Use Only

---

## Risk Scoring Methodology

Risks are scored using a 5x5 qualitative matrix.

**Likelihood Scale**
| Score | Level | Description |
|---|---|---|
| 1 | Rare | May occur once in 10+ years |
| 2 | Unlikely | May occur once in 3-10 years |
| 3 | Possible | May occur once in 1-3 years |
| 4 | Likely | May occur once per year |
| 5 | Almost Certain | May occur multiple times per year |

**Impact Scale**
| Score | Level | Description |
|---|---|---|
| 1 | Negligible | Minimal operational impact, no regulatory consequence |
| 2 | Minor | Limited impact, manageable internally |
| 3 | Moderate | Noticeable disruption, possible regulatory attention |
| 4 | Major | Significant operational/financial/reputational harm |
| 5 | Critical | Severe harm, regulatory action, possible litigation |

**Risk Score = Likelihood x Impact**

| Score Range | Rating | Response Required |
|---|---|---|
| 1-4 | Low | Monitor, annual review |
| 5-9 | Medium | Mitigate, quarterly review |
| 10-15 | High | Immediate mitigation plan |
| 16-25 | Critical | Escalate to leadership, immediate action |

---

## Risk Register

### RISK-001: Unauthorized Access to PHI via Compromised Credentials

| Field | Value |
|---|---|
| Category | Cybersecurity |
| Description | An attacker obtains valid employee credentials through phishing and gains unauthorized access to systems containing protected health information |
| Threat Source | External attacker, phishing campaign |
| Inherent Likelihood | 4 |
| Inherent Impact | 5 |
| Inherent Risk Score | 20 (Critical) |
| Current Controls | MFA enforced on all remote access; security awareness training annually; email filtering in place |
| Residual Likelihood | 2 |
| Residual Impact | 5 |
| Residual Risk Score | 10 (High) |
| Risk Owner | IT Security Manager |
| Treatment | Mitigate |
| Status | Open - MFA coverage gap exists on internal systems |
| Next Review | June 2026 |

---

### RISK-002: Ransomware Attack on Critical Systems

| Field | Value |
|---|---|
| Category | Cybersecurity |
| Description | Ransomware encrypts critical servers or endpoints, causing operational disruption and potential data loss or exposure |
| Threat Source | External attacker, malicious email attachment or RDP exploitation |
| Inherent Likelihood | 3 |
| Inherent Impact | 5 |
| Inherent Risk Score | 15 (High) |
| Current Controls | Endpoint detection via NinjaOne; backup procedures in place; network segmentation partial |
| Residual Likelihood | 2 |
| Residual Impact | 4 |
| Residual Risk Score | 8 (Medium) |
| Risk Owner | IT Operations Manager |
| Treatment | Mitigate |
| Status | Open - backup recovery testing not documented |
| Next Review | June 2026 |

---

### RISK-003: HIPAA Breach Due to Unencrypted Portable Device

| Field | Value |
|---|---|
| Category | Compliance |
| Description | An employee loses a laptop or USB drive containing unencrypted PHI, triggering a HIPAA reportable breach and OCR investigation |
| Threat Source | Employee negligence, theft |
| Inherent Likelihood | 3 |
| Inherent Impact | 4 |
| Inherent Risk Score | 12 (High) |
| Current Controls | Full-disk encryption policy exists; not uniformly enforced on all devices |
| Residual Likelihood | 2 |
| Residual Impact | 4 |
| Residual Risk Score | 8 (Medium) |
| Risk Owner | Compliance Officer |
| Treatment | Mitigate |
| Status | Open - encryption compliance not verified on all endpoints |
| Next Review | May 2026 |

---

### RISK-004: Third-Party Vendor Data Breach

| Field | Value |
|---|---|
| Category | Third-Party |
| Description | A business associate or vendor with access to organization data suffers a breach, exposing patient or student records and triggering notification obligations |
| Threat Source | External attacker targeting vendor; vendor negligence |
| Inherent Likelihood | 3 |
| Inherent Impact | 4 |
| Inherent Risk Score | 12 (High) |
| Current Controls | BAAs in place with primary vendors; no formal annual vendor security review process |
| Residual Likelihood | 3 |
| Residual Impact | 3 |
| Residual Risk Score | 9 (Medium) |
| Risk Owner | Compliance Officer |
| Treatment | Mitigate |
| Status | Open - TPRM program under development |
| Next Review | June 2026 |

---

### RISK-005: Failure to Provide Timely HIPAA Breach Notification

| Field | Value |
|---|---|
| Category | Compliance |
| Description | Organization fails to notify affected individuals, HHS, or media within required HIPAA timeframes following a confirmed breach, resulting in regulatory penalties |
| Threat Source | Internal process failure, inadequate incident response procedures |
| Inherent Likelihood | 2 |
| Inherent Impact | 4 |
| Inherent Risk Score | 8 (Medium) |
| Current Controls | Incident response plan documented; notification checklist exists but not tested |
| Residual Likelihood | 2 |
| Residual Impact | 3 |
| Residual Risk Score | 6 (Medium) |
| Risk Owner | Compliance Officer / Legal |
| Treatment | Mitigate |
| Status | Open - IR tabletop exercise needed |
| Next Review | June 2026 |

---

### RISK-006: Excessive User Privileges (Privilege Creep)

| Field | Value |
|---|---|
| Category | Cybersecurity / Compliance |
| Description | Users accumulate access rights over time beyond what their role requires, increasing the attack surface and violating least privilege principles |
| Threat Source | Inadequate access governance processes, role changes without access review |
| Inherent Likelihood | 4 |
| Inherent Impact | 3 |
| Inherent Risk Score | 12 (High) |
| Current Controls | Provisioning/deprovisioning procedures exist; no formal periodic access review cycle |
| Residual Likelihood | 3 |
| Residual Impact | 3 |
| Residual Risk Score | 9 (Medium) |
| Risk Owner | IT Security / HR |
| Treatment | Mitigate |
| Status | Open - quarterly access review process being established |
| Next Review | April 2026 |

---

### RISK-007: Unpatched Vulnerabilities on Critical Systems

| Field | Value |
|---|---|
| Category | Cybersecurity |
| Description | Critical security patches are not applied within SLA, leaving known vulnerabilities exploitable by attackers |
| Threat Source | External attacker, automated exploitation tools |
| Inherent Likelihood | 3 |
| Inherent Impact | 4 |
| Inherent Risk Score | 12 (High) |
| Current Controls | Patch management via NinjaOne; patches applied but no formal SLA tracked |
| Residual Likelihood | 2 |
| Residual Impact | 3 |
| Residual Risk Score | 6 (Medium) |
| Risk Owner | IT Operations |
| Treatment | Mitigate |
| Status | In Progress - SLA documentation underway |
| Next Review | May 2026 |

---

### RISK-008: Insider Threat - Unauthorized Data Exfiltration

| Field | Value |
|---|---|
| Category | Cybersecurity |
| Description | A current or former employee intentionally copies or transmits sensitive data to unauthorized destinations |
| Threat Source | Disgruntled employee, departing employee |
| Inherent Likelihood | 2 |
| Inherent Impact | 5 |
| Inherent Risk Score | 10 (High) |
| Current Controls | Offboarding procedure includes account deprovisioning; no DLP controls in place |
| Residual Likelihood | 2 |
| Residual Impact | 4 |
| Residual Risk Score | 8 (Medium) |
| Risk Owner | IT Security / HR |
| Treatment | Mitigate |
| Status | Open - DLP solution evaluation pending budget approval |
| Next Review | June 2026 |

---

### RISK-009: Loss of Key Compliance Personnel

| Field | Value |
|---|---|
| Category | Operational |
| Description | Departure of the primary compliance or security officer creates gaps in regulatory knowledge, ongoing audit obligations, and program continuity |
| Threat Source | Voluntary resignation, medical leave |
| Inherent Likelihood | 2 |
| Inherent Impact | 3 |
| Inherent Risk Score | 6 (Medium) |
| Current Controls | Some documentation exists; no formal succession or cross-training plan |
| Residual Likelihood | 2 |
| Residual Impact | 3 |
| Residual Risk Score | 6 (Medium) |
| Risk Owner | HR / Executive Leadership |
| Treatment | Mitigate |
| Status | Open - cross-training plan to be developed Q2 2026 |
| Next Review | June 2026 |

---

### RISK-010: Inadequate Business Continuity / Disaster Recovery

| Field | Value |
|---|---|
| Category | Operational |
| Description | A significant disruption (system outage, natural disaster, cyberattack) renders critical systems unavailable for an extended period with no tested recovery plan |
| Threat Source | Ransomware, infrastructure failure, natural disaster |
| Inherent Likelihood | 2 |
| Inherent Impact | 5 |
| Inherent Risk Score | 10 (High) |
| Current Controls | Data backups in place; no formal BCP/DRP documented or tested |
| Residual Likelihood | 2 |
| Residual Impact | 4 |
| Residual Risk Score | 8 (Medium) |
| Risk Owner | IT Operations / Executive Leadership |
| Treatment | Mitigate |
| Status | Open - BCP development scheduled Q2 2026 |
| Next Review | June 2026 |

---

### RISK-011: Social Engineering / Phishing

| Field | Value |
|---|---|
| Category | Cybersecurity |
| Description | Employees are deceived via phishing, vishing, or pretexting into disclosing credentials or authorizing fraudulent transactions |
| Threat Source | External attacker, targeted phishing campaign |
| Inherent Likelihood | 4 |
| Inherent Impact | 3 |
| Inherent Risk Score | 12 (High) |
| Current Controls | Annual security awareness training; email filtering; simulated phishing tested once |
| Residual Likelihood | 3 |
| Residual Impact | 3 |
| Residual Risk Score | 9 (Medium) |
| Risk Owner | IT Security |
| Treatment | Mitigate |
| Status | Open - quarterly phishing simulations planned |
| Next Review | April 2026 |

---

### RISK-012: Non-Compliant Handling of Student Records (FERPA)

| Field | Value |
|---|---|
| Category | Compliance |
| Description | Student education records are disclosed to unauthorized parties or not secured appropriately, violating FERPA requirements and risking loss of federal funding |
| Threat Source | Employee error, process gap |
| Inherent Likelihood | 2 |
| Inherent Impact | 4 |
| Inherent Risk Score | 8 (Medium) |
| Current Controls | FERPA training provided at onboarding; no annual refresher; access to records not reviewed regularly |
| Residual Likelihood | 2 |
| Residual Impact | 3 |
| Residual Risk Score | 6 (Medium) |
| Risk Owner | Compliance Officer / School Administration |
| Treatment | Mitigate |
| Status | Open - annual FERPA refresher training to be implemented |
| Next Review | May 2026 |

---

### RISK-013: Cloud Misconfiguration Exposing Sensitive Data

| Field | Value |
|---|---|
| Category | Cybersecurity |
| Description | Misconfigured cloud storage (e.g., public S3 bucket, open SharePoint permissions) exposes sensitive organizational or patient/student data to unauthorized access |
| Threat Source | Configuration error, lack of cloud security controls |
| Inherent Likelihood | 3 |
| Inherent Impact | 4 |
| Inherent Risk Score | 12 (High) |
| Current Controls | Microsoft 365 tenant in use; no formal cloud security configuration review or CSPM tool |
| Residual Likelihood | 3 |
| Residual Impact | 3 |
| Residual Risk Score | 9 (Medium) |
| Risk Owner | IT Security |
| Treatment | Mitigate |
| Status | Open - M365 security posture review planned |
| Next Review | May 2026 |

---

### RISK-014: Failure to Maintain Audit Evidence

| Field | Value |
|---|---|
| Category | Compliance |
| Description | Insufficient or disorganized audit evidence results in findings during an external audit, potential non-compliance determinations, or inability to demonstrate control effectiveness |
| Threat Source | Inadequate documentation processes, staff turnover |
| Inherent Likelihood | 3 |
| Inherent Impact | 3 |
| Inherent Risk Score | 9 (Medium) |
| Current Controls | Evidence collected manually; stored in shared drive with inconsistent naming conventions |
| Residual Likelihood | 2 |
| Residual Impact | 3 |
| Residual Risk Score | 6 (Medium) |
| Risk Owner | Compliance / GRC Analyst |
| Treatment | Mitigate |
| Status | In Progress - standardized evidence repository being built |
| Next Review | April 2026 |

---

## Risk Summary

| Rating | Count |
|---|---|
| Critical (16-25) | 0 |
| High (10-15) | 7 |
| Medium (5-9) | 7 |
| Low (1-4) | 0 |

**Top 3 Priority Risks:** RISK-001 (Credential Compromise), RISK-002 (Ransomware), RISK-003 (Unencrypted Device)

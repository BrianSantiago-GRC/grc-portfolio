# HIPAA Security Rule Audit Checklist

**Regulation:** 45 CFR Parts 160 and 164
**Audit Scope:** Administrative, Physical, and Technical Safeguards
**Auditor:** Brian Santiago
**Review Date:** March 2026
**Status Key:** Implemented | Partial | Not Implemented | N/A

---

## Administrative Safeguards (45 CFR § 164.308)

| Ref | Requirement | Status | Evidence Required | Notes |
|---|---|---|---|---|
| 164.308(a)(1)(i) | Security Management Process: Risk analysis performed | Implemented | Most recent risk analysis report with date | Annual or when significant changes occur |
| 164.308(a)(1)(ii)(A) | Risk analysis covers all ePHI systems | Implemented | Risk analysis scope documentation | Must include all systems, not just EHR |
| 164.308(a)(1)(ii)(B) | Risk management plan addresses identified risks | Partial | Risk register with treatment plans | Risk register exists; treatment tracking incomplete |
| 164.308(a)(1)(ii)(C) | Sanction policy for workforce violations | Implemented | HR policy document, employee handbook section | Include documentation of sanctions applied |
| 164.308(a)(1)(ii)(D) | Information system activity review (log review) | Partial | Log review procedure and evidence of reviews | Procedure documented; log review not consistently performed |
| 164.308(a)(2) | Assigned Security Responsibility - designated security official | Implemented | Job description or designation letter | Name and contact on file |
| 164.308(a)(3)(i) | Workforce Security: authorization procedures for ePHI access | Implemented | Access control SOP | Included in Access Control Policy |
| 164.308(a)(3)(ii)(A) | Authorization/supervision of workforce members | Implemented | Onboarding checklist, manager approval records | |
| 164.308(a)(3)(ii)(B) | Workforce clearance procedures before granting access | Implemented | HR screening policy, access request forms | Background check process documented |
| 164.308(a)(3)(ii)(C) | Termination procedures for revoking access | Implemented | Offboarding checklist with IT sign-off | Verify same-day deprovisioning for involuntary terms |
| 164.308(a)(4)(i) | Information Access Management: policies for authorizing ePHI access | Implemented | Access control policy | Role-based access documented |
| 164.308(a)(4)(ii)(A) | Isolating healthcare clearinghouse functions | N/A | N/A | Not applicable to this organization type |
| 164.308(a)(4)(ii)(B) | Access authorization procedures | Implemented | Access request/approval workflow | Tickets reviewed quarterly |
| 164.308(a)(4)(ii)(C) | Access establishment and modification procedures | Implemented | IAM procedures, AD group policy documentation | |
| 164.308(a)(5)(i) | Security Awareness Training: program for all workforce members | Partial | Training records, attendance logs | Training completed annually; no phishing simulation |
| 164.308(a)(5)(ii)(A) | Security reminders (periodic updates) | Partial | Evidence of newsletters/email alerts | Ad hoc; no formal schedule |
| 164.308(a)(5)(ii)(B) | Protection from malicious software training | Implemented | Training records showing malware/phishing content | |
| 164.308(a)(5)(ii)(C) | Log-in monitoring training | Not Implemented | Training records | Not currently covered in awareness program |
| 164.308(a)(5)(ii)(D) | Password management training | Implemented | Training content showing password policy section | |
| 164.308(a)(6)(i) | Security Incident Procedures: policies for addressing incidents | Implemented | Incident response plan | IR plan documented; tabletop not yet performed |
| 164.308(a)(6)(ii) | Incident response and reporting procedures | Partial | IR playbooks, reporting chain of command | Response procedures documented; reporting timelines need formalization |
| 164.308(a)(7)(i) | Contingency Plan: data backup plan | Implemented | Backup policy, evidence of backup execution | Recovery testing not documented |
| 164.308(a)(7)(ii)(A) | Disaster recovery plan | Partial | DRP document | Exists in draft; not formally approved or tested |
| 164.308(a)(7)(ii)(B) | Emergency mode operation plan | Partial | Emergency operations procedure | High-level only; needs detail |
| 164.308(a)(7)(ii)(C) | Testing and revision procedures for contingency plans | Not Implemented | Test schedules, test results | No documented test has been performed |
| 164.308(a)(7)(ii)(D) | Applications and data criticality analysis | Not Implemented | Asset inventory with criticality ratings | Asset inventory in progress |
| 164.308(a)(8) | Evaluation: periodic technical/non-technical security evaluations | Partial | Vulnerability scan results, last evaluation date | Qualys scans performed; formal evaluation report not produced |
| 164.308(b)(1) | Business Associate Contracts: BAAs in place with all BAs | Implemented | BAA log with vendor names and execution dates | Annual review of BAA list recommended |

---

## Physical Safeguards (45 CFR § 164.310)

| Ref | Requirement | Status | Evidence Required | Notes |
|---|---|---|---|---|
| 164.310(a)(1) | Facility Access Controls: policies to limit physical access | Implemented | Physical security policy, badge access logs | |
| 164.310(a)(2)(i) | Contingency operations for facility access during emergency | Partial | Emergency access procedure | Procedure exists but not tested |
| 164.310(a)(2)(ii) | Facility security plan (protect facility from unauthorized access) | Implemented | Physical security plan, visitor log | |
| 164.310(a)(2)(iii) | Access control and validation procedures (visitor management) | Implemented | Visitor sign-in log, escort policy | |
| 164.310(a)(2)(iv) | Maintenance records for physical security components | Partial | Maintenance logs | Badge access logs kept; no formal hardware maintenance log |
| 164.310(b) | Workstation Use: policies specifying proper use and location | Implemented | Acceptable use policy, workstation use standards | |
| 164.310(c) | Workstation Security: physical safeguards for workstations | Implemented | Screen lock policy, physical security inspection records | Auto-lock policy enforced via GPO |
| 164.310(d)(1) | Device and Media Controls: policies for hardware/media disposal | Implemented | Media disposal policy, destruction certificates | |
| 164.310(d)(2)(i) | Disposal procedures for hardware and media containing ePHI | Implemented | Destruction vendor certificates | Third-party destruction vendor used |
| 164.310(d)(2)(ii) | Media reuse procedures | Implemented | Sanitization procedure (NIST 800-88) | Documented in media disposal policy |
| 164.310(d)(2)(iii) | Accountability for hardware and electronic media movement | Partial | Asset tracking log | Asset tracking not fully current |
| 164.310(d)(2)(iv) | Data backup before movement of equipment | Implemented | Backup procedure requiring backup before repurposing | |

---

## Technical Safeguards (45 CFR § 164.312)

| Ref | Requirement | Status | Evidence Required | Notes |
|---|---|---|---|---|
| 164.312(a)(1) | Access Controls: technical policies to allow only authorized access | Implemented | Active Directory access controls, RBAC documentation | |
| 164.312(a)(2)(i) | Unique user identification for all users | Implemented | AD policy, no shared account policy | Confirm no shared/generic accounts in use |
| 164.312(a)(2)(ii) | Emergency access procedure | Partial | Break-glass account procedure | Procedure documented; access not routinely reviewed |
| 164.312(a)(2)(iii) | Automatic logoff | Implemented | GPO settings showing screen lock/logoff timeout | 15-minute timeout enforced |
| 164.312(a)(2)(iv) | Encryption and decryption of ePHI | Partial | Encryption policy, BitLocker deployment status | Policy exists; not uniformly enforced on all devices |
| 164.312(b) | Audit Controls: mechanisms to record and examine ePHI activity | Partial | Log sources, log retention policy | Splunk used for log collection; retention policy formal documentation pending |
| 164.312(c)(1) | Integrity: protect ePHI from improper alteration or destruction | Implemented | Data integrity controls, checksums, backup verification | |
| 164.312(c)(2) | Electronic mechanisms to corroborate ePHI integrity | Partial | File integrity monitoring documentation | Not implemented for all systems |
| 164.312(d) | Person or Entity Authentication: verify identity before granting access | Implemented | MFA policy, MFA deployment evidence | MFA enforced on remote access and M365 |
| 164.312(e)(1) | Transmission Security: protect ePHI during electronic transmission | Implemented | TLS configuration documentation, email encryption policy | |
| 164.312(e)(2)(i) | Integrity controls for transmission | Implemented | TLS version/cipher documentation | TLS 1.2+ enforced |
| 164.312(e)(2)(ii) | Encryption of transmitted ePHI | Implemented | Email encryption policy, VPN requirement for remote access | |

---

## Audit Summary

| Safeguard Category | Implemented | Partial | Not Implemented | Total Controls |
|---|---|---|---|---|
| Administrative | 16 | 8 | 4 | 28 |
| Physical | 8 | 3 | 0 | 11 |
| Technical | 7 | 4 | 0 | 11 |
| **Total** | **31** | **15** | **4** | **50** |

**Compliance Rate (Fully Implemented):** 62%
**Priority Gaps:** Log review, contingency plan testing, full-disk encryption enforcement, security awareness program completeness

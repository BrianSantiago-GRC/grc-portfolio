# Incident Response Plan

| Field | Value |
|---|---|
| Document ID | IRP-001 |
| Version | 1.1 |
| Status | Approved |
| Owner | Information Security Officer |
| Approved By | Executive Leadership |
| Effective Date | January 2026 |
| Next Review | January 2027 |
| Framework | NIST SP 800-61 Rev. 2 |

---

## 1. Purpose

This Incident Response Plan (IRP) defines the organization's procedures for preparing for, detecting, analyzing, containing, eradicating, and recovering from information security incidents. It ensures a coordinated, effective response that minimizes impact to operations, protects sensitive data, and meets regulatory notification requirements under HIPAA, FERPA, and other applicable regulations.

---

## 2. Scope

This plan applies to:
- All information security incidents involving organizational systems, networks, and data
- All workforce members involved in incident response activities
- All third parties who must be notified of or participate in incident response

---

## 3. Definitions

**Security Incident:** Any actual or suspected event that threatens the confidentiality, integrity, or availability of organizational information assets.

**Data Breach:** A security incident that results in unauthorized access, acquisition, use, or disclosure of sensitive data (PHI, PII, student records, etc.).

**Reportable Breach (HIPAA):** An impermissible use or disclosure of PHI that compromises the privacy or security of the information, unless an exception applies.

**Security Event:** Any observable occurrence in a system or network (may or may not be an incident).

**Indicators of Compromise (IoC):** Artifacts or behaviors that suggest a system has been compromised (unusual login times, unexpected outbound traffic, modified system files, etc.).

**CSIRT:** Computer Security Incident Response Team — the group responsible for coordinating incident response activities.

---

## 4. Incident Classification

All incidents must be classified by severity to determine response priority and escalation:

| Severity | Level | Criteria | Response Time |
|---|---|---|---|
| SEV-1 | Critical | Active breach of PHI/PII; ransomware deployment; system-wide outage affecting patient/student safety; confirmed APT activity | Immediate — 24/7 response |
| SEV-2 | High | Suspected PHI exposure; successful phishing with credential compromise; significant system compromise; active malware spread | Within 2 hours |
| SEV-3 | Medium | Phishing attempt (no credential compromise); malware contained to single endpoint; policy violation with potential exposure; failed brute-force attack | Within 24 hours |
| SEV-4 | Low | Minor policy violation; unsuccessful attack attempt; suspicious email reported; single endpoint anomaly (no data exposure) | Within 72 hours |

---

## 5. Incident Response Team (CSIRT)

### Core Team

| Role | Responsibility | Primary Contact |
|---|---|---|
| Incident Commander | Overall coordination, escalation decisions, executive communication | Information Security Officer |
| IT Lead | Technical containment, forensic evidence collection, system recovery | IT Security Manager |
| Compliance Lead | Regulatory reporting, HIPAA/FERPA notification requirements, legal coordination | Compliance Officer |
| Communications Lead | Internal and external communication, public statement coordination | Executive Director / PR |
| HR Lead | Workforce-related incidents, insider threat coordination | Human Resources Director |

### Extended Team (as needed)

| Role | Activation Criteria |
|---|---|
| Legal Counsel | Any incident involving potential litigation, law enforcement involvement, or regulatory investigation |
| Forensics Vendor | Any SEV-1 or SEV-2 incident requiring digital forensics or chain of custody |
| Cyber Insurance Carrier | Any SEV-1 or SEV-2 incident; notify carrier per policy requirements |
| External PR Firm | Any incident involving media inquiries or required public notification |

---

## 6. NIST SP 800-61 Incident Response Lifecycle

```
┌─────────────┐    ┌─────────────┐    ┌─────────────┐    ┌─────────────┐
│ PREPARATION │ ──▶│  DETECTION  │ ──▶│ CONTAINMENT │ ──▶│  RECOVERY   │
│             │    │  & ANALYSIS │    │ ERADICATION │    │             │
└─────────────┘    └─────────────┘    └─────────────┘    └─────────────┘
                                              │
                                              ▼
                                   ┌─────────────────────┐
                                   │  POST-INCIDENT       │
                                   │  ACTIVITY           │
                                   └─────────────────────┘
```

---

## 7. Phase 1: Preparation

### 7.1 Preventive Measures

Before incidents occur, the organization must maintain:
- Up-to-date asset inventory with criticality ratings
- Current contact list for all CSIRT members (updated quarterly)
- Documented network topology and data flow diagrams
- Pre-approved communication templates for internal/external notification
- Tested backup and recovery procedures
- Cyber insurance policy with carrier contact information
- Relationships with forensics vendors and legal counsel

### 7.2 Detection Capabilities

The organization must maintain the following detection mechanisms:
- SIEM / log aggregation (Splunk) with configured alerts
- Endpoint protection with alerting (NinjaOne EDR)
- Email security with phishing reporting capability
- Vulnerability scanning (Qualys) on a defined schedule
- User reporting mechanism (IT helpdesk / direct ISO contact)

### 7.3 Preparedness Activities

| Activity | Frequency | Responsible |
|---|---|---|
| Tabletop exercise | Annually (minimum) | ISO + CSIRT |
| Contact list review | Quarterly | ISO |
| Backup recovery test | Annually | IT Operations |
| Forensics retainer review | Annually | ISO + Legal |
| Cyber insurance policy review | Annually | ISO + Finance |
| Training on IR procedures | At onboarding + annually | ISO |

---

## 8. Phase 2: Detection and Analysis

### 8.1 Incident Sources

Incidents may be detected through:
- SIEM alerts (Splunk)
- Endpoint alerts (NinjaOne)
- User reports (IT helpdesk, direct to ISO)
- Email security alerts
- Third-party notifications (vendor, CISA, law enforcement)
- Regulatory complaint or audit finding

### 8.2 Initial Triage

Upon receiving an alert or report:

**Step 1 — Validate:** Determine if the event is a confirmed incident or a false positive.
- Review alert details, logs, and corroborating evidence
- Interview reporting user if applicable
- Check asset criticality and data sensitivity

**Step 2 — Classify Severity:** Assign SEV-1 through SEV-4 based on classification criteria in Section 4.

**Step 3 — Notify CSIRT:** Activate the appropriate CSIRT members based on severity:
- SEV-1/2: Immediate notification of full CSIRT
- SEV-3: Notify IT Lead and ISO within 2 hours
- SEV-4: IT Lead documents and monitors; ISO informed in daily summary

**Step 4 — Open Incident Ticket:** Create a ticket in the IT helpdesk/ITSM system immediately. All subsequent actions must be documented in the ticket.

### 8.3 Evidence Collection and Documentation

All evidence must be preserved from the point of detection:
- Do not power off affected systems without forensics guidance (disk encryption may prevent recovery)
- Capture screenshots, log exports, and system state before any containment actions
- Document time, date, system, and action taken for every step
- Treat all evidence as potentially needed for litigation (chain of custody applies)

Evidence to collect:
- System logs (auth logs, application logs, network logs)
- Email headers and message content
- Screenshots of malicious activity or messages
- Network traffic captures (if available)
- Memory dumps (for active malware investigations)
- File system timeline data

---

## 9. Phase 3: Containment, Eradication, and Recovery

### 9.1 Containment Strategy

Containment must be calibrated to the incident type. The goal is to stop the spread without destroying evidence.

| Incident Type | Short-Term Containment | Long-Term Containment |
|---|---|---|
| Compromised account | Disable account, revoke active sessions, reset credentials | Audit for unauthorized actions, review access logs |
| Ransomware | Isolate infected system(s) from network immediately | Identify patient zero, assess spread, preserve for forensics |
| Phishing (credential harvest) | Reset affected credentials, block sender, alert workforce | Review email logs for additional affected users |
| Data exfiltration | Block outbound connections from suspected source | Identify scope of exposed data, preserve logs |
| Insider threat | Preserve account access logs, notify HR and legal | Revoke access, secure affected data, prepare for HR action |
| Malware (non-ransomware) | Isolate endpoint, run full scan | Verify clean state before returning to production |

**Critical Rule:** Do NOT reimage or wipe a system before forensic evidence has been collected, unless authorized by the Incident Commander.

### 9.2 Eradication

After containment, eliminate the root cause:
- Remove malware from affected systems
- Patch exploited vulnerabilities
- Revoke and rotate compromised credentials (including service accounts)
- Remove unauthorized accounts or access
- Verify that no persistence mechanisms remain (scheduled tasks, registry keys, startup entries)

### 9.3 Recovery

Restore systems to normal operations:
- Restore from last known-good backup (verify integrity before restoring)
- Rebuild affected systems from scratch if compromise is deep
- Validate system integrity before returning to production
- Monitor restored systems closely for 30 days post-incident for signs of reinfection
- Update security controls and signatures before returning to service

Recovery validation checklist:
- [ ] Clean scan results from endpoint protection
- [ ] Verified backup integrity before restore
- [ ] All compromised credentials rotated
- [ ] Patches applied
- [ ] Monitoring configured on recovered systems
- [ ] Business unit sign-off before returning to production

---

## 10. Regulatory Notification Requirements

### 10.1 HIPAA Breach Notification

If the incident involves a potential breach of PHI:

| Notification Required | Timeline | Method |
|---|---|---|
| Affected individuals | Within 60 days of discovery | Written letter (first-class mail) |
| HHS (≥500 individuals) | Within 60 days of discovery | HHS online portal |
| HHS (<500 individuals) | Within 60 days of the end of the calendar year | HHS online portal |
| Prominent media (≥500 in a state) | Within 60 days of discovery | Press release |

**Breach Exceptions (HIPAA Safe Harbors):**
- PHI was encrypted and the decryption key was not compromised
- PHI was inadvertently accessed by authorized workforce members
- Organization demonstrates low probability PHI was compromised (4-factor risk assessment required)

The Compliance Officer must conduct a written HIPAA breach risk assessment for all incidents involving PHI.

### 10.2 FERPA Notification

If the incident involves student education records:
- Notify the institution's FERPA compliance officer immediately
- Notification to affected students and parents is handled on a case-by-case basis under FERPA's legitimate educational interest provisions
- State breach notification laws may require independent notification within 30–45 days

### 10.3 Law Enforcement

Incidents involving:
- Ransomware
- Suspected criminal activity
- Nation-state activity
- Extortion

Should be reported to the **FBI (IC3.gov)** and **CISA (us-cert.cisa.gov)**. Legal counsel must be consulted before reporting.

---

## 11. Communication Guidelines

### 11.1 Internal Communication

| Audience | Communication Method | Content |
|---|---|---|
| CSIRT | Secure channel (encrypted messaging or in-person) | Full technical details, status updates |
| Executive Leadership | Email / phone (SEV-1/2 only) | Severity, business impact, decision points |
| Affected Workforce | Internal email (IT helpdesk notice) | What to do / not do; no specifics on attack method |
| All Staff (if needed) | All-staff email approved by Incident Commander | Phishing reminders; policy reminders |

### 11.2 External Communication

**Do not communicate incident details externally without Incident Commander approval.**

| Audience | Who Communicates | Approval Required |
|---|---|---|
| Regulators (HHS, DOE) | Compliance Officer + Legal | Incident Commander |
| Law enforcement | Legal Counsel | Incident Commander |
| Media / press | Communications Lead + PR | Executive Leadership |
| Affected individuals | Compliance Officer (HIPAA letter) | Incident Commander + Legal |
| Vendors / partners | Incident Commander | ISO |

---

## 12. Post-Incident Activity

### 12.1 Post-Incident Review

A post-incident review (PIR) must be conducted for all SEV-1, SEV-2, and SEV-3 incidents within 14 days of closure. The PIR must cover:

1. Timeline of events (detection through recovery)
2. Root cause analysis
3. What worked well
4. What needs improvement
5. Control gaps identified
6. Corrective actions with owners and due dates

### 12.2 Lessons Learned

Findings from the PIR must be:
- Documented in a Lessons Learned report
- Shared with CSIRT and relevant leadership
- Used to update this IRP, related policies, and security controls
- Tracked in the CAPA log to completion

### 12.3 Incident Closure

Incidents are considered closed when:
- All affected systems are restored and verified
- All regulatory notifications have been sent
- PIR is complete and documented
- Corrective actions have been assigned
- Incident ticket has been formally closed by the Incident Commander

---

## 13. Incident Response Playbooks

### Playbook 1: Phishing / Credential Compromise

1. Receive report from user or email security alert
2. Pull email headers and analyze sender, links, attachments
3. Determine if credentials were entered (check email login history, MFA push logs)
4. If credentials compromised: immediately reset password, revoke active sessions, check for mailbox rules, unauthorized forwarding, or OAuth grants
5. Block malicious sender and URLs at email gateway
6. Notify all staff if broad phishing campaign detected
7. Classify severity and escalate per Section 4
8. Document timeline; open incident ticket
9. Conduct PIR within 14 days

---

### Playbook 2: Ransomware

1. Identify affected system(s) — typically via user report or EDR alert
2. **Immediately isolate**: disconnect from network (disable NIC or physically disconnect cable; do NOT power off)
3. Alert CSIRT; classify SEV-1; activate full CSIRT
4. Notify cyber insurance carrier (follow policy requirements)
5. Identify patient zero: review network traffic logs for initial infection vector
6. Assess spread: check for lateral movement, encrypted network shares
7. Do NOT pay ransom without legal and executive authorization
8. Engage forensics vendor if needed
9. Restore from last clean backup after verifying integrity
10. Patch vulnerability exploited in the attack before restoring to production
11. Notify regulators if PHI or student data was accessed
12. PIR within 14 days

---

### Playbook 3: Unauthorized PHI Access

1. Detect via log review, SIEM alert, or user report
2. Identify: which system, which data, how many records, which individuals
3. Preserve all access logs — do not allow log rotation before export
4. Determine if access was intentional (insider threat) or accidental
5. If insider threat: coordinate with HR and Legal; preserve without alerting subject
6. Conduct HIPAA breach risk assessment (4-factor analysis)
7. If breach confirmed: notify ISO, Compliance Officer, Legal within 24 hours
8. Initiate HIPAA notification timeline (60 days)
9. Document full scope for HHS notification
10. PIR within 14 days; update access controls to prevent recurrence

---

### Playbook 4: Lost or Stolen Device

1. Receive report from employee
2. Confirm device inventory record — asset tag, last known user, data stored
3. Determine if device was encrypted (check MDM enrollment, BitLocker status)
4. If encrypted: document risk assessment; breach probability low if key not compromised
5. If unencrypted: treat as confirmed breach — escalate to Compliance Officer immediately
6. Remotely wipe device via MDM if capability exists
7. Revoke all credentials associated with the device
8. Report to local law enforcement if theft
9. Initiate HIPAA/FERPA breach analysis if sensitive data was present
10. PIR; update MDM enforcement procedures

---

## 14. Escalation Matrix

| Severity | Notify Immediately | Notify Within 2 Hours | Notify Same Day |
|---|---|---|---|
| SEV-1 Critical | ISO, IT Lead, Compliance, Executive Director | Legal, Cyber Insurance, Forensics Vendor | HR (if insider) |
| SEV-2 High | ISO, IT Lead, Compliance | Executive Director | Legal |
| SEV-3 Medium | IT Lead | ISO | Compliance |
| SEV-4 Low | IT Helpdesk | IT Lead | — |

---

## Version History

| Version | Date | Author | Changes |
|---|---|---|---|
| 1.0 | January 2025 | B. Santiago | Initial draft |
| 1.1 | January 2026 | B. Santiago | Added playbooks, HIPAA notification timeline, escalation matrix |

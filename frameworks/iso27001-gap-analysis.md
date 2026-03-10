# ISO/IEC 27001:2022 Gap Analysis

**Standard:** ISO/IEC 27001:2022
**Organization:** Sample Organization (Healthcare/Education Sector)
**Analyst:** Brian Santiago
**Analysis Date:** March 2026
**Status Key:** Implemented | Partial | Not Implemented | N/A

---

## Gap Analysis Scope

This gap analysis assesses the organization's current security controls against ISO/IEC 27001:2022 Annex A controls and selected clause requirements. The analysis identifies gaps, estimates implementation effort, and provides a prioritized remediation roadmap.

**Assessment Method:** Document review, stakeholder interviews, and technical configuration review.

---

## ISO 27001:2022 Clause Assessment (Clauses 4–10)

| Clause | Requirement | Status | Notes |
|---|---|---|---|
| 4.1 | Understanding the organization and its context | Partial | High-level context understood; not formally documented |
| 4.2 | Understanding needs of interested parties | Partial | Regulatory requirements documented; customer/employee needs not formally captured |
| 4.3 | Scope of the ISMS defined | Partial | Scope understood by leadership; not formally documented |
| 5.1 | Leadership commitment to ISMS | Partial | Executive support present; no formal ISMS policy signed by leadership |
| 5.2 | Information security policy established | Implemented | ISP-001 approved and in effect |
| 5.3 | Roles and responsibilities defined | Implemented | ISO and Compliance Officer designated |
| 6.1 | Risk assessment process defined | Partial | Risk register started; formal methodology documented but not fully executed |
| 6.2 | Information security objectives defined | Not Implemented | No documented IS objectives with measurable targets |
| 7.1 | Resources provided | Partial | Some resources allocated; no formal resource plan |
| 7.2 | Competence requirements documented | Partial | Certifications tracked; competency framework not defined |
| 7.3 | Awareness program in place | Partial | Annual training; no quarterly phishing or formal awareness schedule |
| 7.4 | Communication procedures defined | Not Implemented | No formal internal/external security communication procedure |
| 7.5 | Documented information managed | Partial | Policies and procedures documented; no document control register |
| 8.1 | Operational planning and control | Partial | Controls defined in policy; not all verified as implemented |
| 8.2 | Risk assessments performed | Partial | Initial risk register completed; not all assets covered |
| 8.3 | Risk treatment plans implemented | Partial | Treatment plans outlined; not all tracked to completion |
| 9.1 | Monitoring and measurement | Not Implemented | No formal KPI/KRI tracking for security controls |
| 9.2 | Internal audit conducted | Not Implemented | No internal ISMS audit performed |
| 9.3 | Management review conducted | Not Implemented | No formal management review meeting documented |
| 10.1 | Nonconformities managed | Not Implemented | No CAPA process for ISMS nonconformities |
| 10.2 | Continual improvement process | Not Implemented | No formal improvement tracking |

---

## Annex A Controls Gap Analysis

### A.5 — Organizational Controls

| Ref | Control | Status | Priority | Notes |
|---|---|---|---|---|
| A.5.1 | Policies for information security | Implemented | — | ISP-001, ACP-001 approved |
| A.5.2 | Information security roles and responsibilities | Implemented | — | Defined in ISP-001 Section 13 |
| A.5.3 | Segregation of duties | Partial | High | Documented in policy; not verified in all systems |
| A.5.4 | Management responsibilities | Partial | Medium | Managers briefed; no formal attestation process |
| A.5.5 | Contact with authorities | Not Implemented | Medium | No documented contacts with law enforcement, regulators |
| A.5.6 | Contact with special interest groups | Not Implemented | Low | No membership in ISACs or threat-sharing communities |
| A.5.7 | Threat intelligence | Not Implemented | High | No formal threat intel program; ad hoc monitoring only |
| A.5.8 | Information security in project management | Not Implemented | Medium | No security requirements in project intake process |
| A.5.9 | Inventory of information and other assets | Partial | High | Asset list exists; not formally maintained |
| A.5.10 | Acceptable use of information assets | Implemented | — | Covered in ISP-001 Section 9 |
| A.5.11 | Return of assets | Partial | Medium | Offboarding checklist includes device recovery; not always verified |
| A.5.12 | Classification of information | Partial | High | Classification scheme defined; not consistently applied to all data |
| A.5.13 | Labelling of information | Not Implemented | Medium | No data labelling practice in place |
| A.5.14 | Information transfer | Partial | High | Email encryption policy exists; no controls on USB/removable media |
| A.5.15 | Access control | Implemented | — | ACP-001 governs access control |
| A.5.16 | Identity management | Implemented | — | AD-managed identities; provisioning process documented |
| A.5.17 | Authentication information | Implemented | — | Password and MFA standards in ACP-001 Section 6 |
| A.5.18 | Access rights | Partial | High | RBAC documented; quarterly access reviews not yet completed |
| A.5.19 | Information security in supplier relationships | Partial | High | BAAs in place; TPRM program under development |
| A.5.20 | Addressing security within supplier agreements | Partial | High | BAAs exist; security requirements not consistently in all contracts |
| A.5.21 | ICT supply chain security | Not Implemented | Medium | No software supply chain security process |
| A.5.22 | Monitoring and review of supplier services | Not Implemented | High | No formal annual vendor review process |
| A.5.23 | Security for cloud services | Partial | High | M365 in use; no formal cloud security configuration review |
| A.5.24 | Information security incident management planning | Partial | High | IRP documented; not tested |
| A.5.25 | Assessment and decision on events | Partial | Medium | Classification criteria defined; not consistently applied |
| A.5.26 | Response to information security incidents | Partial | High | IR plan in place; playbooks partial |
| A.5.27 | Learning from information security incidents | Not Implemented | Medium | No lessons-learned or post-incident review process |
| A.5.28 | Collection of evidence | Not Implemented | Medium | No formal digital forensics/evidence preservation procedure |
| A.5.29 | Business continuity management | Partial | Critical | BCP/DRP in draft; not tested or approved |
| A.5.30 | ICT readiness for business continuity | Not Implemented | High | No RTO/RPO targets defined or tested |
| A.5.31 | Legal requirements | Partial | Medium | HIPAA/FERPA identified; full legal register not maintained |
| A.5.32 | Intellectual property rights | Partial | Low | Software licensing tracked informally |
| A.5.33 | Protection of records | Partial | High | Retention schedules exist for some data; not comprehensive |
| A.5.34 | Privacy and PII protection | Partial | High | FERPA controls documented; PII inventory incomplete |
| A.5.35 | Independent review of information security | Not Implemented | High | No internal audit or independent security assessment performed |
| A.5.36 | Compliance with policies and standards | Partial | Medium | Policy compliance not formally measured |
| A.5.37 | Documented operating procedures | Partial | Medium | Key SOPs exist; coverage incomplete |

---

### A.6 — People Controls

| Ref | Control | Status | Priority | Notes |
|---|---|---|---|---|
| A.6.1 | Screening | Implemented | — | Background check process documented |
| A.6.2 | Terms and conditions of employment | Implemented | — | Security expectations in employment agreements |
| A.6.3 | Information security awareness training | Partial | High | Annual training completed; phishing simulations not quarterly |
| A.6.4 | Disciplinary process | Implemented | — | Sanctions policy in ISP-001 Section 14 |
| A.6.5 | Responsibilities after termination | Implemented | — | NDA and confidentiality obligations documented |
| A.6.6 | Confidentiality agreements | Implemented | — | NDAs required for all workforce members |
| A.6.7 | Remote working | Partial | Medium | Remote work policy exists; MDM compliance not verified |
| A.6.8 | Information security event reporting | Partial | High | Reporting channel defined; informal; not all events escalated |

---

### A.7 — Physical Controls

| Ref | Control | Status | Priority | Notes |
|---|---|---|---|---|
| A.7.1 | Physical security perimeters | Implemented | — | Badge access at all facility entry points |
| A.7.2 | Physical entry | Implemented | — | Visitor sign-in and escort policy in place |
| A.7.3 | Securing offices, rooms, and facilities | Implemented | — | Server room access restricted to authorized IT staff |
| A.7.4 | Physical security monitoring | Partial | Medium | Camera coverage partial; no formal review schedule |
| A.7.5 | Protecting against physical and environmental threats | Partial | Medium | Fire suppression present; flood/environmental risk not assessed |
| A.7.6 | Working in secure areas | Implemented | — | Access restrictions and clean desk expectations documented |
| A.7.7 | Clear desk and clear screen | Partial | Low | Policy exists; compliance not audited |
| A.7.8 | Equipment siting and protection | Implemented | — | Server room environmental controls in place |
| A.7.9 | Security of off-site assets | Partial | High | Laptops issued to remote workers; encryption not uniformly verified |
| A.7.10 | Storage media | Partial | Medium | USB restriction policy exists; not technically enforced |
| A.7.11 | Supporting utilities | Partial | Medium | UPS in place; no formal testing schedule |
| A.7.12 | Cabling security | Implemented | — | Network cabling in locked infrastructure closets |
| A.7.13 | Equipment maintenance | Partial | Low | Maintenance tracked informally |
| A.7.14 | Secure disposal of equipment | Implemented | — | Third-party destruction vendor with certificates |

---

### A.8 — Technological Controls

| Ref | Control | Status | Priority | Notes |
|---|---|---|---|---|
| A.8.1 | User endpoint devices | Partial | High | Endpoint protection deployed; full-disk encryption not uniform |
| A.8.2 | Privileged access rights | Partial | High | Privileged accounts exist; no PAM tool or quarterly review completed |
| A.8.3 | Information access restriction | Implemented | — | RBAC and access controls documented and applied |
| A.8.4 | Access to source code | N/A | — | No custom software development in scope |
| A.8.5 | Secure authentication | Partial | High | MFA enforced on remote and cloud; gaps on internal apps |
| A.8.6 | Capacity management | Not Implemented | Low | No formal capacity monitoring process |
| A.8.7 | Protection against malware | Implemented | — | Endpoint protection deployed via NinjaOne |
| A.8.8 | Management of technical vulnerabilities | Partial | High | Qualys scans performed; no formal SLA tracking |
| A.8.9 | Configuration management | Partial | High | GPO applied; no formal hardening baseline documented |
| A.8.10 | Information deletion | Partial | Medium | Data disposal policy exists; not uniformly applied to cloud storage |
| A.8.11 | Data masking | Not Implemented | Medium | No data masking for non-production environments |
| A.8.12 | Data leakage prevention | Not Implemented | High | No DLP controls in place |
| A.8.13 | Information backup | Partial | High | Backups performed; no documented recovery test |
| A.8.14 | Redundancy of information processing | Partial | High | Some redundancy; no formal high-availability architecture documented |
| A.8.15 | Logging | Partial | High | Splunk in use; retention policy not formalized |
| A.8.16 | Monitoring activities | Partial | High | SIEM alerts configured; no formal triage or escalation process |
| A.8.17 | Clock synchronization | Implemented | — | NTP configured on servers |
| A.8.18 | Use of privileged utility programs | Partial | Medium | Restricted; not formally controlled via PAM |
| A.8.19 | Installation of software | Partial | Medium | No application allowlisting in place |
| A.8.20 | Networks security | Partial | High | Firewall in place; partial segmentation; no formal review |
| A.8.21 | Security of network services | Partial | Medium | ISP and cloud provider SLAs reference security; not reviewed |
| A.8.22 | Segregation of networks | Partial | High | Partial segmentation; ePHI systems not fully isolated |
| A.8.23 | Web filtering | Partial | Medium | DNS filtering in place; no URL categorization policy |
| A.8.24 | Use of cryptography | Partial | High | Encryption policies defined; not uniformly applied |
| A.8.25 | Secure development lifecycle | N/A | — | No custom development in scope |
| A.8.26 | Application security requirements | N/A | — | No custom development in scope |
| A.8.27 | Secure system architecture | Partial | Medium | Architecture documented informally |
| A.8.28 | Secure coding | N/A | — | No custom development in scope |
| A.8.29 | Security testing in development and acceptance | N/A | — | No custom development in scope |
| A.8.30 | Outsourced development | N/A | — | No outsourced development in scope |
| A.8.31 | Separation of development, test, and production | Partial | Medium | Prod/non-prod separation informal |
| A.8.32 | Change management | Partial | Medium | Change process exists; not formally documented for security review |
| A.8.33 | Test information | Partial | Low | No formal policy prohibiting use of production data in testing |
| A.8.34 | Protection of information systems during audit | Partial | Low | Audit access controlled; no formal protocol |

---

## Gap Summary by Category

| Category | Total Controls | Implemented | Partial | Not Implemented | N/A |
|---|---|---|---|---|---|
| Clauses 4–10 | 21 | 3 | 11 | 7 | 0 |
| A.5 — Organizational | 37 | 5 | 19 | 13 | 0 |
| A.6 — People | 8 | 5 | 3 | 0 | 0 |
| A.7 — Physical | 14 | 6 | 8 | 0 | 0 |
| A.8 — Technological | 34 | 4 | 20 | 4 | 6 |
| **Total** | **114** | **23** | **61** | **24** | **6** |

**Compliance Rate (Fully Implemented):** 21% of applicable controls fully implemented
**Partial Implementation:** 56%
**Not Implemented:** 22%

---

## Prioritized Remediation Plan

### Critical Priority (Complete within 30 days)

| Control | Gap | Action |
|---|---|---|
| A.5.29 / BCP | BCP/DRP not tested | Schedule tabletop; approve DRP; test backups |
| A.5.35 | No internal audit | Plan and conduct first internal ISMS audit |
| A.8.12 | No DLP | Implement M365 Purview DLP for sensitive data |
| A.8.13 | Backup not tested | Execute and document recovery test |
| 9.1/9.2/9.3 | No management review or measurement | Schedule management review; establish KPIs |

### High Priority (Complete within 60 days)

| Control | Gap | Action |
|---|---|---|
| A.5.18 | Access reviews not completed | Execute first quarterly privileged access review |
| A.5.22 | Vendor reviews absent | Implement annual vendor review process |
| A.5.7 | No threat intel | Subscribe to CISA AIS; assign monitoring owner |
| A.8.2 | No PAM tool | Evaluate and implement PAM solution |
| A.8.8 | Vuln SLA not tracked | Define and track remediation SLAs in Qualys |
| A.8.15 | Log retention undocumented | Document Splunk retention and review policy |

### Medium Priority (Complete within 90 days)

| Control | Gap | Action |
|---|---|---|
| A.5.9 | Asset inventory incomplete | Complete hardware/software/data inventory |
| A.5.23 | Cloud security not reviewed | Conduct M365 security posture review |
| A.6.8 | Incident reporting informal | Formalize incident reporting procedure and training |
| A.8.5 | MFA gaps | Extend MFA to all internal applications |
| 6.2 | No IS objectives | Define and document measurable security objectives |
| 10.1 | No CAPA process | Implement CAPA tracking for nonconformities |

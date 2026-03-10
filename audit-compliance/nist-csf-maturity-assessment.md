# NIST Cybersecurity Framework (CSF) Maturity Assessment

**Framework Version:** NIST CSF 2.0
**Organization:** Sample Organization (Healthcare/Education Sector)
**Assessor:** Brian Santiago
**Assessment Date:** March 2026
**Methodology:** Capability Maturity Model (1–4 scale)

---

## Maturity Scale

| Level | Name | Description |
|---|---|---|
| 0 | Not Performed | Activity does not exist |
| 1 | Initial | Ad hoc, no documented process, unpredictable outcomes |
| 2 | Developing | Some documentation exists; inconsistently applied |
| 3 | Defined | Documented, consistently applied, and measured |
| 4 | Optimizing | Continuously improved, metrics-driven, integrated across the organization |

**Target State:** Level 3 for all critical controls; Level 4 for Identify and Protect functions.

---

## GV — GOVERN (New in CSF 2.0)

The Govern function establishes organizational context, risk management strategy, roles, and oversight.

| Ref | Control | Current | Target | Gap | Notes |
|---|---|---|---|---|---|
| GV.OC-01 | Organizational mission and risk tolerance defined | 2 | 3 | Yes | Risk tolerance not formally documented |
| GV.OC-02 | Legal and regulatory obligations understood | 3 | 3 | No | HIPAA/FERPA obligations documented |
| GV.OC-03 | Stakeholder needs and expectations integrated | 2 | 3 | Yes | No formal stakeholder risk reporting cadence |
| GV.RM-01 | Risk management policy established and approved | 2 | 4 | Yes | Policy exists but not formally approved or measured |
| GV.RM-02 | Risk management roles and responsibilities defined | 3 | 3 | No | ISO, Compliance Officer, GRC Analyst roles defined |
| GV.RM-06 | Risk management program reviewed and updated | 2 | 3 | Yes | Annual review planned; no completed cycle yet |
| GV.RR-01 | Cybersecurity roles and responsibilities defined | 3 | 3 | No | Defined in security policy Section 13 |
| GV.SC-01 | Supply chain risk management integrated | 1 | 3 | Yes | TPRM program under development |

**Function Average: 2.1 / 4 | Target: 3.1 / 4**

---

## ID — IDENTIFY

The Identify function supports understanding of current cybersecurity risk to organizational systems, people, assets, data, and capabilities.

### ID.AM — Asset Management

| Ref | Control | Current | Target | Gap | Notes |
|---|---|---|---|---|---|
| ID.AM-01 | Hardware asset inventory maintained | 2 | 4 | Yes | Asset list exists; not formally maintained or reviewed |
| ID.AM-02 | Software asset inventory maintained | 2 | 4 | Yes | No formal CMDB; software tracked informally |
| ID.AM-03 | Network topology documented | 2 | 3 | Yes | High-level diagram exists; not current |
| ID.AM-07 | Data inventory and classification performed | 2 | 4 | Yes | Classification scheme defined; data inventory incomplete |
| ID.AM-08 | Systems, hardware, and software managed | 2 | 3 | Yes | Managed via NinjaOne; no formal lifecycle policy |

### ID.RA — Risk Assessment

| Ref | Control | Current | Target | Gap | Notes |
|---|---|---|---|---|---|
| ID.RA-01 | Vulnerabilities identified and documented | 3 | 4 | Yes | Qualys scans performed; no formal SLA for remediation tracking |
| ID.RA-02 | Cyber threat intelligence received and analyzed | 2 | 3 | Yes | Informal monitoring; no structured threat intel process |
| ID.RA-03 | Threats identified and documented | 2 | 3 | Yes | Risk register started; not all assets covered |
| ID.RA-05 | Risk response options identified | 2 | 3 | Yes | Risk register in progress; treatment plans incomplete |
| ID.RA-06 | Risk responses prioritized | 2 | 3 | Yes | Prioritization informal |

### ID.IM — Improvement

| Ref | Control | Current | Target | Gap | Notes |
|---|---|---|---|---|---|
| ID.IM-01 | Improvements identified from evaluations | 2 | 3 | Yes | No formal lessons-learned process after incidents |
| ID.IM-02 | Improvements identified from security tests | 2 | 3 | Yes | Qualys findings not formally tracked to resolution |

**Function Average: 2.1 / 4 | Target: 3.3 / 4**

---

## PR — PROTECT

The Protect function supports the ability to limit or contain the impact of a cybersecurity event.

### PR.AA — Identity Management and Access Control

| Ref | Control | Current | Target | Gap | Notes |
|---|---|---|---|---|---|
| PR.AA-01 | Identities managed for authorized users | 3 | 4 | Yes | Provisioning process documented; no formal lifecycle review |
| PR.AA-02 | Identities verified before access | 3 | 4 | Yes | MFA on remote access and M365; not enforced on internal apps |
| PR.AA-03 | Users, services, hardware authenticated | 3 | 3 | No | MFA policy documented and applied |
| PR.AA-05 | Access permissions managed | 2 | 4 | Yes | RBAC documented; no quarterly access review cycle completed |
| PR.AA-06 | Physical access managed | 3 | 3 | No | Badge access in place; visitor log maintained |

### PR.AT — Awareness and Training

| Ref | Control | Current | Target | Gap | Notes |
|---|---|---|---|---|---|
| PR.AT-01 | Personnel trained in security awareness | 2 | 3 | Yes | Annual training completed; no quarterly phishing simulations yet |
| PR.AT-02 | Privileged users trained | 2 | 3 | Yes | Role-specific training not formally tracked |

### PR.DS — Data Security

| Ref | Control | Current | Target | Gap | Notes |
|---|---|---|---|---|---|
| PR.DS-01 | Data at rest protected | 2 | 4 | Yes | BitLocker policy exists; not enforced on all devices |
| PR.DS-02 | Data in transit protected | 3 | 4 | Yes | TLS 1.2+ enforced; email encryption policy in place |
| PR.DS-10 | Data deletions/modifications logged | 2 | 3 | Yes | Some logging via Splunk; not comprehensive |

### PR.IR — Technology Infrastructure Resilience

| Ref | Control | Current | Target | Gap | Notes |
|---|---|---|---|---|---|
| PR.IR-01 | Networks and environments protected | 2 | 3 | Yes | Partial network segmentation; no full micro-segmentation |
| PR.IR-03 | Backups performed and maintained | 3 | 4 | Yes | Backups in place; recovery testing not documented |
| PR.IR-04 | Adequate capacity ensured | 2 | 3 | Yes | No formal capacity planning process |

### PR.PS — Platform Security

| Ref | Control | Current | Target | Gap | Notes |
|---|---|---|---|---|---|
| PR.PS-01 | Configuration management policies enforced | 2 | 3 | Yes | GPO applied; no formal baseline standard documented |
| PR.PS-02 | Software maintained | 3 | 4 | Yes | NinjaOne patching; no documented SLA compliance tracking |
| PR.PS-04 | Logs generated and retained | 2 | 3 | Yes | Splunk in use; retention policy not formally documented |
| PR.PS-05 | Installation controls applied | 2 | 3 | Yes | No formal application allowlisting |

**Function Average: 2.5 / 4 | Target: 3.4 / 4**

---

## DE — DETECT

The Detect function enables timely discovery of cybersecurity events.

### DE.AE — Adverse Event Analysis

| Ref | Control | Current | Target | Gap | Notes |
|---|---|---|---|---|---|
| DE.AE-02 | Potentially adverse events analyzed | 2 | 3 | Yes | Splunk alerts configured; no formal triage procedure |
| DE.AE-03 | Information correlated from multiple sources | 2 | 3 | Yes | Splunk aggregates logs; correlation rules incomplete |
| DE.AE-06 | Information provided to authorized staff | 2 | 3 | Yes | Alerting to IT; no formal escalation path |
| DE.AE-07 | Cyber threat intelligence integrated | 1 | 3 | Yes | No formal threat intel integration |
| DE.AE-08 | Incidents declared when criteria met | 2 | 3 | Yes | IR plan defines criteria; process not consistently followed |

### DE.CM — Continuous Monitoring

| Ref | Control | Current | Target | Gap | Notes |
|---|---|---|---|---|---|
| DE.CM-01 | Networks monitored to detect events | 2 | 3 | Yes | Partial monitoring; no full IDS/IPS deployment |
| DE.CM-03 | Personnel activity monitored | 1 | 3 | Yes | No DLP or UEBA in place |
| DE.CM-06 | External service provider activities monitored | 1 | 3 | Yes | No vendor monitoring program |
| DE.CM-09 | Computing hardware and software monitored | 2 | 3 | Yes | NinjaOne endpoint monitoring; no behavioral analysis |

**Function Average: 1.7 / 4 | Target: 3.0 / 4**

---

## RS — RESPOND

The Respond function supports the ability to contain the impacts of cybersecurity incidents.

### RS.MA — Incident Management

| Ref | Control | Current | Target | Gap | Notes |
|---|---|---|---|---|---|
| RS.MA-01 | Incident response plan executed | 2 | 3 | Yes | IRP documented; no tabletop exercise performed |
| RS.MA-02 | Incident reported per policy | 2 | 3 | Yes | Reporting chain defined; timelines not formalized |
| RS.MA-03 | Incident categorized and prioritized | 2 | 3 | Yes | Severity categories defined; not consistently applied |
| RS.MA-04 | Incidents escalated appropriately | 2 | 3 | Yes | Escalation matrix exists; not tested |
| RS.MA-05 | Incidents declared resolved | 2 | 3 | Yes | No formal closure process documented |

### RS.AN — Incident Analysis

| Ref | Control | Current | Target | Gap | Notes |
|---|---|---|---|---|---|
| RS.AN-03 | Analysis performed to support recovery | 2 | 3 | Yes | RCA performed informally |
| RS.AN-06 | Actions performed to prevent recurrence | 2 | 3 | Yes | CAPAs created ad hoc; no formal CAPA tracking |
| RS.AN-08 | Magnitude of incidents estimated | 1 | 3 | Yes | No formal impact assessment process |

### RS.CO — Incident Response Reporting and Communication

| Ref | Control | Current | Target | Gap | Notes |
|---|---|---|---|---|---|
| RS.CO-02 | Internal stakeholders notified | 2 | 3 | Yes | Notification process partially defined |
| RS.CO-03 | Information shared with designated parties | 1 | 3 | Yes | No formal process for sharing with ISAC, law enforcement |

**Function Average: 1.8 / 4 | Target: 3.0 / 4**

---

## RC — RECOVER

The Recover function supports timely restoration of normal operations.

### RC.RP — Incident Recovery Plan Execution

| Ref | Control | Current | Target | Gap | Notes |
|---|---|---|---|---|---|
| RC.RP-01 | Recovery plan executed | 1 | 3 | Yes | No tested recovery plan exists |
| RC.RP-02 | Recovery actions validated | 1 | 3 | Yes | Backups not tested |
| RC.RP-03 | Organization recovery communicated | 1 | 3 | Yes | No recovery communication plan |
| RC.RP-05 | Recovery actions documented | 1 | 3 | Yes | No post-incident recovery documentation |
| RC.RP-06 | Recovery plan updated | 1 | 3 | Yes | No plan exists to update |

### RC.CO — Incident Recovery Communication

| Ref | Control | Current | Target | Gap | Notes |
|---|---|---|---|---|---|
| RC.CO-03 | Recovery activities communicated to affected parties | 1 | 3 | Yes | No notification templates or procedures |
| RC.CO-04 | Public updates shared as appropriate | 1 | 3 | Yes | No external communication protocol |

**Function Average: 1.0 / 4 | Target: 3.0 / 4**

---

## Assessment Summary

| Function | Controls | Current Avg | Target Avg | % Gap |
|---|---|---|---|---|
| GV — Govern | 8 | 2.1 | 3.1 | 32% |
| ID — Identify | 12 | 2.1 | 3.3 | 36% |
| PR — Protect | 17 | 2.5 | 3.4 | 26% |
| DE — Detect | 9 | 1.7 | 3.0 | 43% |
| RS — Respond | 10 | 1.8 | 3.0 | 40% |
| RC — Recover | 7 | 1.0 | 3.0 | 67% |
| **Total** | **63** | **1.9** | **3.1** | **39%** |

---

## Overall Maturity Score: 1.9 / 4 (Developing)

---

## Priority Gap Analysis

### Tier 1 — Critical Gaps (Score ≤ 1.5, High Business Impact)

| Gap | Current | Target | Recommended Action |
|---|---|---|---|
| Recovery plans not tested | 1.0 | 3.0 | Schedule backup recovery test; document results |
| No DLP or insider threat monitoring | 1.0 | 3.0 | Evaluate DLP solutions; implement M365 Purview controls |
| No threat intelligence program | 1.0 | 3.0 | Subscribe to FS-ISAC or CISA alerts; integrate into Splunk |
| No tested incident response plan | 1.0 | 3.0 | Conduct tabletop exercise within 60 days |
| Supply chain risk management absent | 1.0 | 3.0 | Implement TPRM questionnaire for all vendors |

### Tier 2 — High Gaps (Score 1.5–2.0)

| Gap | Current | Target | Recommended Action |
|---|---|---|---|
| Asset inventory incomplete | 2.0 | 4.0 | Complete hardware/software/data inventory; integrate with NinjaOne |
| Full-disk encryption not enforced | 2.0 | 4.0 | Deploy BitLocker enforcement via GPO; track compliance |
| No quarterly access reviews | 2.0 | 4.0 | Establish quarterly review cycle; start with privileged accounts |
| No phishing simulations | 2.0 | 3.0 | Launch quarterly simulation program via KnowBe4 or similar |
| Log retention policy undocumented | 2.0 | 3.0 | Document Splunk retention policy; align to HIPAA 6-year requirement |

### Tier 3 — Moderate Gaps (Score 2.0–2.5)

| Gap | Recommended Action |
|---|---|
| Risk register treatment tracking | Add treatment status tracking; assign owners |
| Network segmentation partial | Complete segmentation to isolate ePHI systems |
| MFA gaps on internal apps | Extend MFA to all internal applications |
| No formal CAPA tracking | Implement CAPA log with owners and due dates |

---

## Recommended Remediation Roadmap

### 0–30 Days
- Conduct IR tabletop exercise
- Test backup recovery and document results
- Deploy quarterly phishing simulations
- Document Splunk log retention policy

### 30–60 Days
- Complete asset inventory (hardware + software)
- Enforce full-disk encryption via GPO
- Establish quarterly access review cycle
- Launch vendor security questionnaire program (TPRM)

### 60–90 Days
- Implement CAPA tracking process
- Extend MFA to all internal applications
- Subscribe to threat intelligence feed (CISA AIS, FS-ISAC)
- Develop and approve formal BCP/DRP

### 90–180 Days
- Evaluate DLP solution
- Complete network segmentation review
- Perform full re-assessment and report progress to leadership

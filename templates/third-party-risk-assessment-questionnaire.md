# Third-Party Risk Assessment Questionnaire

**Document ID:** TPRM-001
**Version:** 1.0
**Owner:** GRC Analyst / Compliance Officer
**Purpose:** Evaluate the security posture of vendors, contractors, and business associates prior to onboarding and during annual review cycles.

---

## Instructions

This questionnaire must be completed by the vendor's authorized security or compliance representative. All responses must be factually accurate. Supporting documentation may be requested for any response. Incomplete submissions will delay onboarding approval.

**Scoring:** Each question is weighted by risk domain. Responses are scored 0–2:
- **2:** Fully implemented and documented
- **1:** Partially implemented or in progress
- **0:** Not implemented

**Risk Tiers:**
| Score Range | Risk Tier | Action |
|---|---|---|
| 80–100% | Low | Approve with standard BAA |
| 60–79% | Moderate | Approve with additional contractual controls; semi-annual review |
| 40–59% | High | Conditional approval; corrective action plan required; quarterly review |
| Below 40% | Critical | Do not approve until critical gaps remediated |

---

## Section 1: Vendor Information

| Field | Response |
|---|---|
| Vendor / Company Name | |
| Primary Contact Name and Title | |
| Contact Email | |
| Contact Phone | |
| Services / Products Provided | |
| Contract Start Date | |
| Data Types Accessed (check all that apply) | ☐ PHI  ☐ PII  ☐ Student Records  ☐ Financial  ☐ Credentials  ☐ Internal Only |
| System Access Required? | ☐ Yes  ☐ No |
| Access to Production Systems? | ☐ Yes  ☐ No |
| Sub-processors / Subcontractors Used? | ☐ Yes  ☐ No  (if yes, list in Section 10) |
| Questionnaire Completed By | |
| Date Completed | |

---

## Section 2: Governance and Compliance (Weight: 15%)

**2.1** Does your organization have a documented Information Security Policy approved by senior leadership?
- ☐ Yes — attach policy or summary
- ☐ No
- ☐ In development

**2.2** Is your organization compliant with or certified under any of the following frameworks? (Select all that apply)
- ☐ ISO 27001 (provide certification date and certificate number)
- ☐ SOC 2 Type II (provide report date and scope)
- ☐ HIPAA (confirm BAA willingness)
- ☐ NIST CSF
- ☐ PCI DSS
- ☐ FedRAMP
- ☐ None of the above

**2.3** Does your organization conduct annual security risk assessments?
- ☐ Yes — describe methodology and provide date of most recent assessment
- ☐ No

**2.4** Does your organization have a designated Information Security Officer or equivalent role?
- ☐ Yes — provide name and contact
- ☐ No

**2.5** Does your organization conduct independent third-party security audits or penetration tests?
- ☐ Yes — provide date of most recent; summary of findings available upon request
- ☐ No

**2.6** Does your organization maintain a documented vendor / subprocessor management program?
- ☐ Yes
- ☐ No

---

## Section 3: Data Handling and Privacy (Weight: 20%)

**3.1** Does your organization maintain a data inventory identifying all categories of data collected, processed, and stored on behalf of clients?
- ☐ Yes
- ☐ No

**3.2** Does your organization have a documented data classification policy?
- ☐ Yes — describe classification levels
- ☐ No

**3.3** Is data provided by our organization logically separated from data belonging to other clients?
- ☐ Yes — describe how
- ☐ No

**3.4** Does your organization encrypt data at rest using AES-256 or equivalent?
- ☐ Yes — describe implementation
- ☐ Partial — describe what is not encrypted
- ☐ No

**3.5** Does your organization encrypt data in transit using TLS 1.2 or higher?
- ☐ Yes
- ☐ No

**3.6** Does your organization have a documented data retention and deletion policy?
- ☐ Yes — provide retention schedule summary
- ☐ No

**3.7** Does your organization delete or destroy client data upon contract termination within a defined timeframe?
- ☐ Yes — specify timeframe: ___
- ☐ No

**3.8** Does your organization support data subject rights requests (access, deletion, correction) if required by applicable privacy laws?
- ☐ Yes
- ☐ Partial
- ☐ No

**3.9** Has your organization had any regulatory findings, fines, or enforcement actions related to data privacy in the past 3 years?
- ☐ Yes — describe
- ☐ No

**3.10** Are subprocessors permitted to access client data? If yes, are they bound by the same data protection obligations?
- ☐ Yes, subprocessors access data — describe controls
- ☐ No subprocessors access client data

---

## Section 4: Access Control and Identity Management (Weight: 15%)

**4.1** Does your organization enforce role-based access controls (RBAC) limiting access to client data to only personnel with a documented business need?
- ☐ Yes
- ☐ Partial
- ☐ No

**4.2** Is multi-factor authentication (MFA) required for all personnel accessing systems that process or store client data?
- ☐ Yes — all personnel
- ☐ Partial — describe exceptions
- ☐ No

**4.3** Does your organization enforce unique user accounts? Are shared or generic accounts prohibited?
- ☐ Yes — no shared accounts
- ☐ Shared accounts exist — describe controls
- ☐ No policy in place

**4.4** Are privileged access accounts (administrator accounts) subject to additional controls (separate accounts, PAM tool, enhanced logging)?
- ☐ Yes — describe
- ☐ No

**4.5** Are access rights reviewed periodically to confirm they remain appropriate?
- ☐ Yes — quarterly
- ☐ Yes — annually
- ☐ No formal review

**4.6** Are user accounts deprovisioned immediately upon employee termination?
- ☐ Yes — same day
- ☐ Within 24–72 hours
- ☐ No defined process

**4.7** Does your organization use an Identity Provider (IdP) or Single Sign-On (SSO) solution?
- ☐ Yes — specify provider
- ☐ No

---

## Section 5: Endpoint and Network Security (Weight: 10%)

**5.1** Is endpoint protection software (antivirus/EDR) deployed on all systems that access client data?
- ☐ Yes
- ☐ Partial
- ☐ No

**5.2** Is full-disk encryption enabled on all laptops and portable devices used to access client data?
- ☐ Yes
- ☐ Partial
- ☐ No

**5.3** Does your organization apply security patches within defined SLAs?
- ☐ Yes — Critical: ___ days, High: ___ days
- ☐ No defined SLA

**5.4** Does your organization use firewalls and network segmentation to isolate systems containing client data?
- ☐ Yes — describe
- ☐ Partial
- ☐ No

**5.5** Is remote access to your systems restricted to VPN or equivalent secure access with MFA?
- ☐ Yes
- ☐ Partial
- ☐ No

---

## Section 6: Security Awareness and Training (Weight: 5%)

**6.1** Does your organization conduct security awareness training for all personnel upon hire?
- ☐ Yes
- ☐ No

**6.2** Does your organization conduct annual refresher security awareness training?
- ☐ Yes
- ☐ No

**6.3** Does your organization conduct simulated phishing tests?
- ☐ Yes — frequency: ___
- ☐ No

**6.4** Does your organization provide role-specific security training for personnel with access to PHI, PII, or other regulated data?
- ☐ Yes
- ☐ No

---

## Section 7: Vulnerability and Patch Management (Weight: 10%)

**7.1** Does your organization conduct regular vulnerability scanning on systems that access or store client data?
- ☐ Yes — frequency: ___
- ☐ No

**7.2** Does your organization conduct penetration testing?
- ☐ Yes — annually (or more frequently)
- ☐ Yes — less than annually
- ☐ No

**7.3** Are vulnerability findings tracked to remediation with defined SLAs?
- ☐ Yes — provide SLA tiers
- ☐ No

**7.4** Has your organization experienced a security breach or confirmed compromise in the past 3 years?
- ☐ Yes — describe (date, nature, remediation)
- ☐ No

---

## Section 8: Incident Response and Business Continuity (Weight: 10%)

**8.1** Does your organization have a documented Incident Response Plan?
- ☐ Yes — tested within the past 12 months
- ☐ Yes — not tested
- ☐ No

**8.2** Does your incident response plan include breach notification procedures consistent with HIPAA and applicable state laws?
- ☐ Yes
- ☐ No

**8.3** Does your organization have a documented notification process to alert clients of a security incident affecting their data?
- ☐ Yes — notification within ___ hours of discovery
- ☐ No

**8.4** Does your organization have a documented Business Continuity Plan (BCP) and Disaster Recovery Plan (DRP)?
- ☐ Yes — both tested within the past 12 months
- ☐ Yes — documented but not tested
- ☐ No

**8.5** What are your organization's defined Recovery Time Objective (RTO) and Recovery Point Objective (RPO)?
- RTO: ___
- RPO: ___

**8.6** Does your organization back up client data? How frequently are backups performed and tested?
- Backup frequency: ___
- Last recovery test: ___

---

## Section 9: Physical Security (Weight: 5%)

**9.1** Are data centers and server rooms where client data is processed or stored physically secured with access controls?
- ☐ Yes — describe controls (badge, biometric, etc.)
- ☐ No

**9.2** Does your organization use a third-party data center provider?
- ☐ Yes — specify provider and confirm SOC 2 / ISO 27001 certification
- ☐ No — in-house

**9.3** Are physical media and devices containing client data securely disposed of using NIST 800-88 methods or equivalent?
- ☐ Yes
- ☐ No

---

## Section 10: Sub-Processors and Third-Party Management (Weight: 10%)

**10.1** List all sub-processors or subcontractors that will have access to our organization's data:

| Sub-Processor Name | Service Provided | Data Accessed | ISO 27001 / SOC 2 Certified? |
|---|---|---|---|
| | | | |
| | | | |

**10.2** Are all sub-processors bound by data protection agreements consistent with your obligations to our organization?
- ☐ Yes
- ☐ No

**10.3** Does your organization assess the security posture of sub-processors before granting access to client data?
- ☐ Yes
- ☐ No

**10.4** Will our organization's data ever be transferred outside the United States?
- ☐ Yes — specify jurisdictions and legal basis
- ☐ No

**10.5** Does your organization carry cyber liability insurance?
- ☐ Yes — coverage amount: $___; carrier: ___
- ☐ No

---

## Section 11: Vendor Attestation

By submitting this questionnaire, the undersigned certifies that all responses are accurate and complete to the best of their knowledge. The undersigned acknowledges that providing false or misleading information may result in termination of the vendor relationship and potential legal action.

| Field | Response |
|---|---|
| Authorized Signatory Name | |
| Title | |
| Signature | |
| Date | |

---

## Scoring Worksheet (Internal Use — Do Not Share with Vendor)

| Section | Max Points | Points Earned | Notes |
|---|---|---|---|
| Section 2: Governance & Compliance (15%) | 12 | | |
| Section 3: Data Handling & Privacy (20%) | 20 | | |
| Section 4: Access Control & IAM (15%) | 14 | | |
| Section 5: Endpoint & Network Security (10%) | 10 | | |
| Section 6: Security Awareness (5%) | 8 | | |
| Section 7: Vuln & Patch Management (10%) | 8 | | |
| Section 8: Incident Response & BCP (10%) | 12 | | |
| Section 9: Physical Security (5%) | 6 | | |
| Section 10: Sub-Processors (10%) | 10 | | |
| **Total** | **100** | | |

**Final Score:** ___ / 100
**Risk Tier:** ☐ Low  ☐ Moderate  ☐ High  ☐ Critical
**Recommendation:** ☐ Approve  ☐ Approve with conditions  ☐ Deny pending remediation

**Reviewed By:** _______________
**Review Date:** _______________
**Next Review Date:** _______________

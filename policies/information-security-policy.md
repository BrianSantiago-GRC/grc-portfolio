# Information Security Policy

| Field | Value |
|---|---|
| Document ID | ISP-001 |
| Version | 1.2 |
| Status | Approved |
| Owner | Information Security Officer |
| Approved By | Executive Leadership |
| Effective Date | January 2026 |
| Next Review | January 2027 |

---

## 1. Purpose

This Information Security Policy establishes the organization's commitment to protecting the confidentiality, integrity, and availability of information assets. It sets the baseline requirements for how information is handled, accessed, transmitted, and protected across all systems and by all workforce members.

---

## 2. Scope

This policy applies to:
- All employees, contractors, vendors, and third parties who access organizational systems or data
- All information assets owned, leased, or managed by the organization
- All systems, networks, devices, and applications used to process, store, or transmit organizational data
- All locations where organizational data is accessed, including remote work environments

---

## 3. Definitions

**ePHI:** Electronic Protected Health Information as defined under HIPAA.

**Information Asset:** Any data, system, device, or software that has value to the organization.

**Workforce Member:** Any employee, contractor, intern, or volunteer with access to organizational systems or data.

**Data Custodian:** The individual or team responsible for the day-to-day management of a specific information asset.

**Sensitive Data:** Any data classified as Confidential or Restricted under the organization's data classification scheme.

**Least Privilege:** The principle that users should have only the minimum access rights necessary to perform their job function.

---

## 4. Data Classification

All organizational data must be classified into one of the following categories:

| Classification | Description | Examples | Handling Requirements |
|---|---|---|---|
| Public | Information intended for public distribution | Press releases, marketing materials | No restrictions |
| Internal | General internal information, not for public release | Internal memos, policies, procedures | Access limited to workforce members |
| Confidential | Sensitive business information | Financial records, contracts, personnel files | Need-to-know access, encryption in transit |
| Restricted | Highly sensitive data with regulatory requirements | PHI, PII, student records, credentials | Strict access controls, encryption at rest and in transit, audit logging |

Data owners are responsible for classifying data assets under their ownership. When in doubt, classify at the higher level.

---

## 5. Access Control

5.1 Access to organizational systems and data must be granted based on business need and the principle of least privilege.

5.2 All access requests must be formally submitted and approved by the requesting employee's manager and the IT department.

5.3 User accounts must be provisioned using unique identifiers. Shared accounts are prohibited except for specific service accounts with documented justification and approval.

5.4 Privileged access (administrator rights) must be approved by the Information Security Officer and reviewed quarterly.

5.5 Access rights must be revoked immediately upon termination of employment. For voluntary resignation, access is revoked no later than the last day of employment.

5.6 Periodic access reviews must be conducted at minimum quarterly for privileged accounts and annually for all standard user accounts.

---

## 6. Password and Authentication Standards

6.1 All accounts must use passwords meeting the following minimum requirements:
- Minimum 12 characters
- Combination of uppercase, lowercase, numbers, and special characters
- No reuse of the last 12 passwords
- Maximum age of 90 days for standard accounts; 60 days for privileged accounts

6.2 Multi-factor authentication (MFA) is required for:
- All remote access to organizational systems
- All cloud-based services (Microsoft 365, Google Workspace, etc.)
- All privileged/administrator accounts
- All systems containing Restricted data

6.3 Passwords must not be shared, written down, or stored in unsecured locations.

6.4 Service accounts must have complex passwords rotated at minimum annually and must not be used for interactive logins.

---

## 7. Device and Endpoint Security

7.1 All organization-owned devices must have endpoint protection software installed and active.

7.2 Full-disk encryption is required on all laptops and mobile devices.

7.3 Automatic screen lock must activate after a maximum of 15 minutes of inactivity.

7.4 All devices must receive security patches within the following timeframes:
- Critical patches: 72 hours
- High severity patches: 7 days
- Medium/Low severity patches: 30 days

7.5 Personal devices used to access organizational systems must comply with the organization's Mobile Device Management (MDM) policy.

7.6 USB and removable media use is restricted. Where permitted, devices must be encrypted.

---

## 8. Data Handling and Transmission

8.1 Sensitive and Restricted data must be encrypted using industry-standard protocols (AES-256 for data at rest, TLS 1.2 or higher for data in transit).

8.2 Sensitive data must not be transmitted via unencrypted email. Secure file transfer or encrypted email must be used.

8.3 Sensitive data must not be stored on personal devices, unapproved cloud services, or removable media without explicit approval.

8.4 Physical documents containing Confidential or Restricted information must be stored in locked cabinets when not in use and shredded when no longer needed.

---

## 9. Acceptable Use

9.1 Organizational systems and data are to be used for legitimate business purposes.

9.2 Incidental personal use of systems is permitted provided it does not interfere with business operations, consume significant resources, or violate other policies.

9.3 The following activities are strictly prohibited:
- Accessing, copying, or transmitting data without authorization
- Installing unauthorized software on organization-owned devices
- Circumventing security controls, including disabling antivirus or firewall software
- Using organizational systems to access, store, or transmit illegal content
- Sharing credentials with any other person
- Using organizational resources for personal financial gain

---

## 10. Security Incident Reporting

10.1 All workforce members are required to report suspected security incidents, potential breaches, or policy violations immediately to the IT helpdesk or Information Security Officer.

10.2 Reporting must not be delayed due to uncertainty. When in doubt, report.

10.3 Retaliation against any individual who reports a security concern in good faith is strictly prohibited.

10.4 The Information Security Officer is responsible for triaging, investigating, and escalating incidents per the Incident Response Plan.

---

## 11. Third-Party and Vendor Security

11.1 All third parties with access to organizational data or systems must sign a Business Associate Agreement (BAA) or equivalent data processing agreement prior to being granted access.

11.2 Vendors must be assessed for security posture before onboarding using the organization's Third-Party Risk Assessment Questionnaire.

11.3 Vendor access must be limited to the minimum required for the business purpose and revoked immediately upon contract termination.

11.4 Vendors must be reviewed at minimum annually for continued compliance with security requirements.

---

## 12. Security Awareness and Training

12.1 All workforce members must complete security awareness training within 30 days of hire.

12.2 Annual refresher training is required for all workforce members.

12.3 Role-specific training must be provided to personnel with elevated access or compliance responsibilities (e.g., HIPAA training for healthcare staff, FERPA training for education staff).

12.4 Simulated phishing exercises will be conducted at minimum quarterly.

---

## 13. Roles and Responsibilities

| Role | Responsibility |
|---|---|
| Information Security Officer | Overall ownership of security program, policy enforcement, incident escalation |
| IT Department | Technical implementation of security controls, patch management, access provisioning |
| Managers/Supervisors | Approving access requests, reporting incidents, ensuring team compliance |
| All Workforce Members | Following this policy, completing training, reporting incidents |
| Compliance Officer | Regulatory compliance alignment, audit coordination |

---

## 14. Compliance and Enforcement

Violations of this policy may result in disciplinary action up to and including termination of employment or contract. Violations involving protected data may also result in civil or criminal liability. Workforce members who observe non-compliance are expected to report it.

---

## 15. Review and Update

This policy will be reviewed annually or following any significant change to the organization's environment, a security incident with policy implications, or regulatory/legal changes affecting information security obligations.

---

## Version History

| Version | Date | Author | Changes |
|---|---|---|---|
| 1.0 | January 2025 | B. Santiago | Initial draft |
| 1.1 | July 2025 | B. Santiago | Added MFA requirements, updated patch SLAs |
| 1.2 | January 2026 | B. Santiago | Added vendor security section, revised data classification table |

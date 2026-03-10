# Access Control Policy

| Field | Value |
|---|---|
| Document ID | ACP-001 |
| Version | 1.2 |
| Status | Approved |
| Owner | Information Security Officer |
| Approved By | Executive Leadership |
| Effective Date | January 2026 |
| Next Review | January 2027 |

---

## 1. Purpose

This Access Control Policy establishes requirements for managing access to organizational systems, applications, and data. It defines standards for user provisioning, authentication, privileged access management, access reviews, and deprovisioning to protect the confidentiality, integrity, and availability of information assets.

---

## 2. Scope

This policy applies to:
- All workforce members (employees, contractors, interns, volunteers) who access organizational systems
- All organizational systems, applications, cloud services, and network resources
- All data classified as Internal, Confidential, or Restricted
- Third-party vendors and business associates granted system access

---

## 3. Definitions

**Role-Based Access Control (RBAC):** A method of regulating access based on the roles of users within the organization, ensuring access is aligned to job function.

**Privileged Account:** Any account with elevated permissions, including system administrators, database administrators, and network engineers.

**Service Account:** A non-interactive account used by applications or automated processes to access resources.

**Least Privilege:** The principle that users are granted only the minimum permissions required to perform their job function.

**Need-to-Know:** Access to specific data or systems is granted only when there is a documented, legitimate business need.

**MFA (Multi-Factor Authentication):** Authentication requiring two or more independent verification factors (something you know, something you have, something you are).

**Identity Lifecycle:** The full process of creating, modifying, and removing user accounts from onboarding through offboarding.

---

## 4. Access Control Principles

4.1 All access to organizational systems must be governed by the principle of **Least Privilege**. Users receive only the minimum level of access required to perform their assigned job function.

4.2 Access must be granted on a **Need-to-Know** basis. Job title alone is not sufficient justification for access to Confidential or Restricted data.

4.3 **Separation of Duties** must be enforced for critical functions. No single user should have end-to-end control over a sensitive process (e.g., initiating and approving financial transactions).

4.4 All access must be **uniquely attributable** to an individual. Shared accounts are prohibited except for documented service accounts.

---

## 5. Access Request and Provisioning

5.1 Access requests must be submitted via the organization's IT ticketing system prior to granting access.

5.2 Each access request must include:
- The specific system(s) and access level requested
- Business justification for the access
- Manager approval
- Duration of access (if temporary)

5.3 The IT department is responsible for provisioning access only after receiving documented manager approval.

5.4 Access provisioning must follow defined role templates when available. Custom access grants that deviate from role templates require additional sign-off from the Information Security Officer.

5.5 New user accounts must be provisioned with the minimum access required for their initial role. Additional access may be requested through the standard access request process.

5.6 Contractor and vendor access must also follow this process and must be scoped to the specific systems required for the contracted work only.

---

## 6. Authentication Standards

### 6.1 Password Requirements

All system accounts must use passwords meeting the following minimum requirements:

| Requirement | Standard Users | Privileged Accounts | Service Accounts |
|---|---|---|---|
| Minimum Length | 12 characters | 16 characters | 20 characters |
| Complexity | Upper, lower, number, special | Upper, lower, number, special | Machine-generated random |
| Maximum Age | 90 days | 60 days | 365 days |
| Password History | Last 12 passwords | Last 24 passwords | N/A (rotated on schedule) |
| Account Lockout | 10 failed attempts | 5 failed attempts | N/A |

### 6.2 Multi-Factor Authentication (MFA)

MFA is required for all of the following:

- All remote access to organizational systems (VPN, Remote Desktop, RDP)
- All cloud-based services (Microsoft 365, Google Workspace, Salesforce, etc.)
- All privileged and administrator accounts, regardless of location
- All systems containing Restricted data (PHI, PII, student records)
- The organization's identity provider and SSO platform

Acceptable MFA factors include:
- Hardware security tokens (FIDO2/WebAuthn preferred)
- Authenticator applications (Microsoft Authenticator, Google Authenticator)
- Push notifications via approved authenticator apps

SMS-based one-time passwords (OTP) are acceptable only when stronger methods are not available and must be approved by the Information Security Officer.

### 6.3 Single Sign-On (SSO)

Where available, organizational applications should be integrated with the approved identity provider using SSO. SSO reduces password fatigue and enables centralized access control.

---

## 7. Privileged Access Management

7.1 Privileged accounts must be separate from standard user accounts. Administrators must use their standard account for day-to-day tasks and their privileged account only when administrative functions are required.

7.2 Privileged access must be approved by the Information Security Officer and documented with business justification.

7.3 Privileged account credentials must be stored in the organization's approved Password Vault / PAM solution. Direct use of privileged credentials outside the PAM tool requires documented exception approval.

7.4 All privileged account activity must be logged. Logs must be retained per the organization's log retention policy and reviewed at minimum monthly.

7.5 Privileged access must be reviewed **quarterly** by the Information Security Officer. Accounts with no activity in the prior 30 days must be disabled and reviewed before reactivation.

7.6 Emergency ("break-glass") privileged accounts must be documented, stored in the PAM vault, and accessed only for documented emergency scenarios. All emergency account use must be logged and reviewed post-incident.

7.7 Service accounts must:
- Use complex, machine-generated passwords rotated at minimum annually
- Not be used for interactive logins
- Be documented with business purpose and responsible owner
- Be reviewed annually

---

## 8. Remote Access

8.1 Remote access to organizational systems is permitted only via the organization's approved VPN or secure remote access platform.

8.2 MFA is required for all remote access sessions without exception.

8.3 Remote sessions must be configured with automatic timeout after 15 minutes of inactivity.

8.4 Users accessing organizational systems remotely from personal devices must comply with the Mobile Device Management (MDM) policy.

8.5 Split tunneling on VPN connections is prohibited unless explicitly approved and documented by the Information Security Officer.

---

## 9. Access Reviews

9.1 Access reviews must be conducted on the following schedule:

| Access Type | Review Frequency | Responsible Party |
|---|---|---|
| Privileged accounts | Quarterly | Information Security Officer |
| Standard user accounts | Annually | IT Department + Managers |
| Contractor / vendor accounts | Semi-annually | IT Department + Contract Manager |
| Service accounts | Annually | IT Department |
| Cloud service permissions | Quarterly | IT Security |

9.2 During each access review, the reviewer must confirm:
- The user still requires the access for their current role
- The access level is appropriate and consistent with least privilege
- No terminated users retain active access

9.3 Access that is identified as excessive, inappropriate, or no longer required must be removed within 5 business days of identification.

9.4 Results of access reviews must be documented and retained for audit purposes.

---

## 10. Deprovisioning and Offboarding

10.1 Upon termination of employment (voluntary or involuntary), the following applies:

| Termination Type | Account Deactivation Timeline |
|---|---|
| Involuntary / immediate | Same day — accounts disabled before employee is notified |
| Voluntary resignation | No later than last day of employment |
| Contractor end of engagement | Same day contract ends |
| Leave of absence | Accounts disabled after 30 days of leave |

10.2 The IT department is responsible for executing account deactivation. HR must notify IT of all terminations at minimum 24 hours in advance for voluntary departures.

10.3 Offboarding must include:
- Disabling all active directory accounts
- Revoking all application and cloud service access
- Disabling VPN credentials and MFA tokens
- Recovering organizational devices
- Forwarding email per manager direction (where legally permissible)

10.4 Following offboarding, a manager or designated IT staff member must verify access revocation within 2 business days and document the verification.

---

## 11. Third-Party and Vendor Access

11.1 All third-party access must be requested through the standard access request process with the contract owner as the approving manager.

11.2 Vendor access must be scoped to the minimum required systems and data. Access to Restricted data requires a signed BAA or equivalent data processing agreement.

11.3 Vendors must use unique credentials. Sharing organizational workforce credentials with vendors is prohibited.

11.4 Where possible, vendor access must be provided through a dedicated vendor account or jump server rather than direct access to production systems.

11.5 Vendor accounts must be reviewed semi-annually and deactivated immediately upon contract termination or project completion.

---

## 12. Audit Logging and Monitoring

12.1 All access to systems containing Confidential or Restricted data must be logged.

12.2 The following events must be captured in audit logs:
- Successful and failed login attempts
- Account creation, modification, and deletion
- Password changes and resets
- Privilege escalation events
- Access to Restricted data classifications
- Remote access sessions

12.3 Audit logs must be retained for a minimum of 6 years for systems containing ePHI (HIPAA requirement) and a minimum of 1 year for all other systems.

12.4 Logs must be protected from unauthorized modification. Access to raw log data is restricted to the Information Security Officer and authorized IT Security personnel.

---

## 13. Policy Exceptions

Requests for exceptions to this policy must be submitted in writing to the Information Security Officer. Exceptions must include:
- Business justification for the exception
- Duration of the exception
- Compensating controls in place
- Risk acceptance sign-off from the appropriate executive

All approved exceptions must be documented and reviewed at least annually.

---

## 14. Roles and Responsibilities

| Role | Responsibility |
|---|---|
| Information Security Officer | Policy ownership, PAM oversight, privileged access approval |
| IT Department | Account provisioning/deprovisioning, access review execution, log management |
| HR Department | Timely notification of new hires, terminations, and role changes |
| Managers/Supervisors | Approve access requests, validate access during reviews, report unauthorized access |
| All Workforce Members | Use accounts only for authorized purposes, report suspicious access activity |
| Compliance Officer | Align policy with regulatory requirements, audit evidence management |

---

## 15. Compliance and Enforcement

Violations of this policy may result in disciplinary action up to and including termination. Violations involving unauthorized access to protected data may result in civil or criminal liability. The IT department must report all suspected policy violations to the Information Security Officer immediately.

---

## Version History

| Version | Date | Author | Changes |
|---|---|---|---|
| 1.0 | January 2025 | B. Santiago | Initial draft |
| 1.1 | July 2025 | B. Santiago | Added PAM requirements, updated MFA standards |
| 1.2 | January 2026 | B. Santiago | Added vendor access section, expanded access review schedule |

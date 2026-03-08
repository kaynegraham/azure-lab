# Microsoft Entra ID Identity Management Lab

## Overview

This project documents a cloud identity management lab built to simulate a small business Microsoft Entra ID environment. The lab demonstrates modern identity and access management fundamentals relevant to entry-level helpdesk and MSP environments.

The goal of this lab is to gain hands-on experience with cloud-based user management, group structures, Role-Based Access Control, user lifecycle management, and Conditional Access policies in Microsoft Entra ID.

---

## Lab Architecture

### Environment

- **Platform:** Microsoft Azure / Microsoft Entra ID
- **Organisation:** KG Tech Solutions (mock business)
- **Tenant:** kaynegrahamdevicloud.onmicrosoft.com

---

### Organisation Structure

- 9 mock users across departments
- Security groups: Finance, HumanResources, ITTeam, Staff
- Microsoft 365 groups: Operations, Sales

<img width="1710" height="961" alt="Screenshot of Users in Tenant" src="https://github.com/user-attachments/assets/3985e9c2-95ed-4edb-954d-3bc3bf3e7f9c" />
<img width="1710" height="936" alt="Screenshot of Groups in Tenant" src="https://github.com/user-attachments/assets/36e8cb3c-034d-4bf2-84c7-760fa66dcbbb" />

---

## Purpose

This lab was built to develop practical experience with:

- Cloud-based user provisioning and management
- Department-based security and Microsoft 365 group structure
- Role-Based Access Control (RBAC)
- Least privilege principles
- User onboarding and offboarding workflows
- Group membership audits
- Conditional Access policy design and implementation

---

## Implementation Steps

### 1. Tenant & Organisation Setup

- Created Microsoft Entra ID tenant
- Configured mock organisation — KG Tech Solutions
- Created 9 realistic user accounts across departments

### 2. Group Structure

- Created Security groups for Finance, HR, IT Team and Staff
- Created Microsoft 365 groups for Operations and Sales with shared mailboxes
- Assigned users to appropriate groups based on department

### 3. Role-Based Access Control (RBAC)

- Assigned roles based on least privilege principles
- Ensured users only had access to resources relevant to their role
- Reviewed and audited group memberships

### 4. User Lifecycle Management

- Practiced user onboarding — creating accounts, assigning groups and licenses
- Practiced user offboarding — disabling accounts, removing group memberships
- Practiced mid-lifecycle changes — department transfers, role changes, license updates

 <img width="1710" height="990" alt="Changing expired password" src="https://github.com/user-attachments/assets/9ca36b4b-7cd7-4409-85cc-eea2247a0db1" />


### 5. Conditional Access Policies

Configured four Conditional Access policies in Report-only mode to simulate real-world MSP security baselines without disrupting the lab environment.

<img width="1429" height="931" alt="Conditional Access Policy List" src="https://github.com/user-attachments/assets/4afd09fa-2095-48c2-9d04-6684909a768e" />


#### Device must be in Australia
- Restricts access to sign-ins originating from Australian locations only
- Blocks overseas logins as a baseline security control
- Commonly implemented for Australian businesses to reduce exposure to foreign threat actors

<img width="1430" height="938" alt="Device must be in Australia" src="https://github.com/user-attachments/assets/e1df5c7f-8cf4-409b-a339-64ae3e3477fe" />


#### Legacy Authentication Prevention
- Blocks authentication requests using legacy protocols such as SMTP, IMAP, and POP3
- Legacy protocols do not support MFA making them a common attack vector
- Critical policy implemented by MSPs during client onboarding

<img width="1423" height="932" alt="Preventing old authetication protocols" src="https://github.com/user-attachments/assets/6f4b32c4-8685-4530-85f9-9aed053c943b" />


#### MFA for Admins
- Enforces Multi-Factor Authentication for all administrator accounts
- Admin accounts are the highest value target for attackers
- Aligns with least privilege and zero trust security principles

<img width="1436" height="909" alt="Multi-factor authentication required for administrators." src="https://github.com/user-attachments/assets/a12b7270-aaae-4df4-a1c9-07ea0f3aa0d3" />


#### Require MFA for High-Risk Logins
- Uses Entra ID Protection risk signals to trigger MFA only when suspicious behaviour is detected
- Balances security with user experience — low risk logins are not challenged
- Demonstrates risk-based Conditional Access rather than blanket enforcement

<img width="1411" height="938" alt="Multi-factor authentication required for high-risk logins." src="https://github.com/user-attachments/assets/6ae16765-c089-4e90-892e-e203e46d49ce" />


---

## Skills Developed

- Microsoft Entra ID administration
- Cloud identity and access management
- Security and Microsoft 365 group management
- Role-Based Access Control (RBAC)
- Least privilege implementation
- User lifecycle management
- Conditional Access policy design
- MFA and risk-based authentication
- Technical documentation

---

## Key Takeaways

Proper group structure and role separation are critical for scalable identity management. Designing identity correctly from the start makes onboarding, role changes, and terminations significantly more efficient and secure. This lab reinforced how important it is to apply least privilege consistently rather than granting broad access by default.

Implementing Conditional Access policies highlighted how organisations enforce security controls at the identity layer rather than relying solely on perimeter defences. Report-only mode is a valuable tool for testing policy impact before enforcement.

---

## Next Steps

- Configure Azure AD Connect to sync on-premises Active Directory with Entra ID
- Build a hybrid identity environment bridging on-prem and cloud
- Explore Microsoft Intune for device management and policy enforcement

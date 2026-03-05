# Microsoft Entra ID Identity Management Lab

## Overview

This project documents a cloud identity management lab built to simulate a small business Microsoft Entra ID environment. The lab demonstrates modern identity and access management fundamentals relevant to entry-level helpdesk and MSP environments.

The goal of this lab is to gain hands-on experience with cloud-based user management, group structures, Role-Based Access Control, and user lifecycle management in Microsoft Entra ID.

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
<img width="1710" height="936" alt="Screenshon of Groups in Tenant" src="https://github.com/user-attachments/assets/36e8cb3c-034d-4bf2-84c7-760fa66dcbbb" />

---

## Purpose

This lab was built to develop practical experience with:

- Cloud-based user provisioning and management
- Department-based security and Microsoft 365 group structure
- Role-Based Access Control (RBAC)
- Least privilege principles
- User onboarding and offboarding workflows
- Group membership audits

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

---

## Skills Developed

- Microsoft Entra ID administration
- Cloud identity and access management
- Security and Microsoft 365 group management
- Role-Based Access Control (RBAC)
- Least privilege implementation
- User lifecycle management
- Technical documentation

---

## Key Takeaways

Proper group structure and role separation are critical for scalable identity management. Designing identity correctly from the start makes onboarding, role changes, and terminations significantly more efficient and secure. This lab reinforced how important it is to apply least privilege consistently rather than granting broad access by default.

---

## Next Steps

- Implement Conditional Access policies to enforce MFA and role-based controls
- Configure Azure AD Connect to sync on-premises Active Directory with Entra ID
- Build a hybrid identity environment bridging on-prem and cloud
- Explore Microsoft Intune for device management and policy enforcement

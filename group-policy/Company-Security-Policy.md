# Company Security Policy Lab

**Domain:** corp.local  
**Server:** Windows Server 2022  
**Client:** Windows 11  

---

## Overview

This lab demonstrates the creation and application of a **Group Policy Object (GPO)** to enforce enterprise security policies. The lab focuses on **centralized security management** for domain users in the IT Organizational Unit (OU).

---

## Policies Implemented

- **Disable Control Panel** – Restricts users from changing system settings  
- **Disable Command Prompt** – Prevents users from executing command-line commands that may bypass security  
- **Account Lockout Policy** – Enforces account lockout after multiple failed login attempts  
- **Password Complexity** – Requires strong passwords with uppercase, lowercase, numbers, and symbols  

The GPO is linked to the IT OU and applied to all Windows 11 clients in the domain.

---

## Results

- Security policies successfully applied and verified on client machines  
- Users in the IT OU cannot access Control Panel or Command Prompt  
- Account lockout and password complexity policies are enforced  
- Policies verified using `rsop.msc` and `gpresult /r`  

**Screenshots folder:** [group-policy/screenshots](group-policy/screenshots)  


## Skills Demonstrated

- Group Policy creation, editing, and linking to OUs  
- Active Directory management for enterprise users  
- Security policy enforcement and verification  
- Practical IT administration and system hardening experience  

---

## Notes

This lab highlights **practical security management** in a Windows domain environment and serves as a professional portfolio example for IT administration and support.

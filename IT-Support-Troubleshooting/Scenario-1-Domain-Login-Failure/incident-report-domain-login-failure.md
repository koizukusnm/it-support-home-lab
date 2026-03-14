# Incident Report: Domain Login Failure

## Incident Summary

A domain user reported being unable to access their workstation. During the login attempt, the system displayed an error message stating that the account had been disabled and advising the user to contact the system administrator.  

The incident occurred within a domain environment managed through Active Directory.

---

## Environment

| Component               | Configuration       |
| ----------------------- | ------------------ |
| Virtualization Platform | VMware Workstation |
| Domain Controller       | Windows Server 2022|
| Client System           | Windows 11         |
| Domain                  | corp.local         |
| User Account            | it_support           |

---

## Problem Description

The affected user attempted to authenticate using their domain credentials (`CORP\it_support`) but was unable to log in. The system returned:

*“Your account has been disabled. Please contact your system administrator.”*

---

## Investigation

The issue was investigated by:

- Reviewing the user account status in Active Directory  
- Examining authentication-related logs in Event Viewer  

It was confirmed that the user account had been marked as **disabled**, which blocked domain access.

---

## Root Cause

The user account had been disabled within Active Directory, preventing authentication and access to domain resources.

---

## Resolution

The account was **re-enabled** in Active Directory. After restoring the account status, the user successfully logged in.

---

## Verification

Domain authentication was verified, and the user was able to access the workstation and domain resources successfully.

---

## Evidence (Screenshots)

All screenshots for this scenario are stored in the **Scenario 1 folder**:  
[IT-Support-Troubleshooting/Screenshot Folder – Domain Login Failure](IT-Support-Troubleshooting/Scenario-1-Domain-Login-Failure/)

---

## Skills Demonstrated

- Active Directory User Management  
- Domain Authentication Troubleshooting  
- Windows Event Log Analysis  
- User Access Restoration  
- IT Support Incident Documentation

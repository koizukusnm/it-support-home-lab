# IT Support Home Lab
IT Support Home Lab built using **VMware, Windows Server, Ubuntu, and Windows 11** for security monitoring and troubleshooting practice.

## Overview

This repository contains hands-on labs and documentation from my **IT Support Home Lab**, including:

- **Active Directory & Domain Setup**  
- **Group Policy Practice**  
- **Windows 11 & Server Configuration**  
- **Ubuntu Server Installation & Administration**  
- **Network Configuration & Security Monitoring**

---

## Group Policy Lab

This lab demonstrates the creation and application of a **Group Policy Object (GPO)** in a Windows domain environment.

**Lab Details:**  

- Created a **Company-Security-Policy GPO** in `corp.local` domain.  
- Restricted **Control Panel** and **Command Prompt** for domain users.  
- Configured **Password Policy** and **Account Lockout Policy**.  
- Linked the GPO to the **IT OU**.  
- Tested and verified on a **Windows 11 client VM**.

**Files:**  

- [`group-policy/Company-Security-Policy.md`](group-policy/Company-Security-Policy.md) → Step-by-step instructions.  
- [`group-policy/screenshots/`](group-policy/screenshots/) → Screenshots showing GPO creation and testing.

**Skills Demonstrated:**  

- Active Directory and Group Policy configuration  
- Policy enforcement and testing on client machines  
- Documentation and lab organization for portfolio

---


## Notes

All labs were completed using **virtual machines on VMware Workstation**. This lab environment is designed for **IT support and system administration skill development**, and can be used as a portfolio for prospective employers.

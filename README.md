# IT Support Home Lab

IT Support Home Lab built using **VMware, Windows Server, Ubuntu, and Windows 11** for security monitoring, Active Directory, and troubleshooting practice.

---

## Overview

This repository contains hands-on labs and documentation from my **IT Support Home Lab**, simulating a small enterprise IT environment. The lab environment includes:

- **Windows Server 2022** as Domain Controller and DNS server  
- **Windows 11 clients** joined to the domain  
- **Ubuntu 24.04 LTS server** for Linux administration practice  
- VMware virtual networking simulating a small enterprise network  

All labs are documented with Markdown files and screenshots for clarity and portfolio presentation.

---

## Lab Documentation

- **Lab Setup & Network Architecture**  
  - [`lab-setup.md`](documentation/lab-setup.md) – Overview, host specs, VM configuration, network setup, installation steps, and lab purpose  
  - [`network-architecture.md`](documentation/network-architecture.md) – Network topology, IP configuration, connectivity testing, and security considerations

- **Active Directory Users & Workstations**  
  - [`Active-Directory-users-workstations.md`](documentation/Active-Directory-users-workstations.md) – Domain setup, OUs for IT, Finance, HR, and user/workstation management

- **Group Policy Lab**  
  - [`group-policy/Company-Security-Policy.md`](group-policy/Company-Security-Policy.md) – High-level GPO overview with security restrictions, password and account lockout policies, and   verification
  - Screenshots: [`group-policy/screenshots/`](group-policy/screenshots/)
- **IT Support Troubleshooting**  
  - **Scenario 1 – Domain Login Failure:**
    - [`IT-Support-Troubleshooting/Scenario-1-Domain-Login-Failure`](IT-Support-Troubleshooting/Scenario-1-Domain-Login-Failure/) -Incident where a domain user could not log in due to a disabled account. Covers troubleshooting in Active Directory, Event Viewer analysis, account restoration, and verification of successful login. 
    - Screenshots: [`IT-Support-Troubleshooting/Scenario-1-Domain-Login-Failure/screenshots`](IT-Support-Troubleshooting/Scenario-1-Domain-Login-Failure/screenshots) 
- **Troubleshooting & Common Errors**  
  - [`troubleshooting/errors.md`](troubleshooting/errors.md) – Documentation of errors encountered during lab setup and practical solutions
- **Shared Folder Lab**  
  - [`Shared Folder Lab/shared-folder.md`](Shared-Folder/shared-folder.md) -Setup and configuration of a network shared folder in Windows Server 2022, integrated with Active Directory. Covers folder creation, NTFS and share permissions, mapped drives for clients, and troubleshooting access issues. 
  - Screenshots: [`Shared-Folder/screenshots`](Shared-Folder/screenshots)
  
---

## Skills Demonstrated

- Active Directory and Group Policy configuration  
- Windows Server and Windows 11 administration  
- Ubuntu server installation and Linux administration  
- Network setup, IP addressing, and connectivity testing  
- Shared folder and permission management  
- Troubleshooting and incident reporting  
- Documentation and portfolio organization

---

## Virtual Home Lab Folder Structure

```text
📂 it-support-home-lab
├─ 📄 README.md
├─ 📂 documentation
│   ├─ 📄 lab-setup.md
│   ├─ 📄 network-architecture.md
│   └─ 📄 Active-Directory-users-workstations.md
├─ 📂 group-policy
│   ├─ 📄 Company-Security-Policy.md
│   └─ 📂 screenshots
├─ 📂 troubleshooting
│   └─ 📄 errors.md
├─ 📂 IT-Support-Troubleshooting
│   └─ 📂 Scenario-1-Domain-Login-Failure
│       ├─ 📄 Incident-Report-Domain-Login-Failure.md
│       └─ 📂 screenshots
└─ 📂 Shared-Folder
    ├─ 📄 shared-folder.md
    └─ 📂 screenshots


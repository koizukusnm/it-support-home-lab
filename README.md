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
  - [`group-policy/Company-Security-Policy.md`](group-policy/Company-Security-Policy.md) – Step-by-step GPO creation, restrictions, password policy, account lockout, and testing  
  - Screenshots: [`group-policy/screenshots/`](group-policy/screenshots/)
- **Troubleshooting & Common Errors**  
  - [`troubleshooting/errors.md`](troubleshooting/errors.md) – Documentation of errors encountered during lab setup and practical solutions
---

## Skills Demonstrated

- Active Directory and Group Policy configuration  
- Windows Server and Windows 11 administration  
- Ubuntu server installation and Linux administration  
- Network setup, IP addressing, and connectivity testing  
- Documentation and portfolio organization

---

## Virtual Home Lab Folder Structure

```text
it-support-home-lab/
 ├─ README.md
 ├─ documentation/
 │    ├─ lab-setup.md
 │    ├─ network-architecture.md
 │    └─ Active-Directory-users-workstations.md
 └─ group-policy/
      ├─ Company-Security-Policy.md
      └─ screenshots

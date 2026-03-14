
# Shared Folder Lab – IT Home Lab Project

## Overview

This lab demonstrates the setup and configuration of a **network shared folder** in a Windows Server 2022 environment, integrated with Active Directory. The shared folder provides a centralized location for lab files, scripts, and reports, simulating a corporate file server environment.

The lab is designed for hands-on practice in **IT support, network file sharing, and permission management**.

---

## Lab Environment

| Component          | Configuration           |
| ------------------ | ----------------------- |
| Virtualization     | VMware Workstation      |
| Server             | Windows Server 2022     |
| Client             | Windows 11 VM           |
| Domain             | corp.local              |
| Shared Folder Name | Shared_IT        |
| User Account       | it.support (domain user) |

---

## Problem Simulation

A user requires access to a shared folder located on the server. Permissions must be configured so that the user can **read, write, and modify files** without granting unnecessary access to other users. Misconfigured permissions may result in **access denied errors** or network drive mapping failures.

---

## Folder Contents

```
Shared_IT/
├─ Lab-Instructions.docx
├─ Scripts/
│   ├─ Add-User.ps1
│   └─ Reset-Password.bat
├─ Reports/
│   └─ Sample-Incident-Report.docx
└─ ISO/
    └─ Windows_Server_2022.iso
```

---

## Access and Permissions

* **NTFS Permissions:** Control file/folder access at the server level.
* **Share Permissions:** Control network access from client machines.
* **Mapped Drive:** Users typically map the shared folder to the `Z:` drive on Windows 11 clients.
* **Domain Integration:** Only authorized domain users can access the shared folder.

---

## Evidence (Screenshots)

All screenshots are stored in the **[`screenshots folder`](Shared-Folder/screenshots)** inside this project. 

---

## Skills Demonstrated

* Setting up a network shared folder in a Windows Server environment
* Configuring NTFS and share permissions for domain users
* Mapping network drives on Windows 11 clients
* Troubleshooting access issues for IT support scenarios
* Simulating real-world corporate file server setup

---



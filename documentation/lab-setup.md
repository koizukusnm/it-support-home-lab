Lab Setup

1. Overview
   This document explains about the setup of IT Support Home lab used to practice system administration, troubleshooting, and enterprise IT Tasks.
   The Lab environment is built using virtualization and includes Windows Server, Windows 11 clients, and Ubuntu Linux

2. Host System Specification
   - Operating System: Windows 11
   - CPU: AMD Ryzen 7 7735HS
   - RAM: 32GB
   - Storage: 1 TB
   - Virtualization Software: VMware Workstation

3. Virtual Machines
   | Vm Name | Operating System | Role | RAM | Disk | Network Adapter |
   |---------|----------------- |------|-----|------|-----------------|
   | Windows Server | Windows Server 2022 | Domain Controller, DNS | 8GB | 100GB | NAT |
   | Windows Client | Windows 11 | Client Machine | 8GB | 100GB | NAT |
   | Ubuntu Server | Ubuntu 24.04 LTS | Linux Server | 8GB | 100GB | NAT |

4. Network Configuration
   All Virtual Machine are connected usign VMware virtual networking.
   
   Network Setup:
   -Virtual Network: VMnet
   -Subnet: 192.168.10.0/24

   Ip configuration:
   | Device | IP Address |
   |--------|------------|
   | Windows Server | IP Address |
   | Windows Client | IP Address |
   | Ubuntu Server | IP Address |

 
5. Windows Server Installation:
     - Create a new virtual machine in VMware
     - Select Windows Sever 2022 ISO   
     - Allocated resources
       - 2 CPU
       - 8 GB RAM
       - 100 GB Disk
     - Install Windows Server with Desktop Experience (Windows Server 2022 Standard)
     - Set Administrator password
6. Active Directory Setup
      Active Directory Domain Services was installed to create a domain environment
    Steps:
     - Open Server Manager
     - Add Role and Features
     - Install Active Directory Domain Services
     - Promote the server to Domain Controller
     - Create a new domain named corp.local
7. Domain Join Process
   The Windows 11 Client machine was joined to the Domain.
   Steps:
     -Open System Settings
     -Change Computer name and join domain
     -Enter Domain name: corp.local
     - Authenticate using domain administrator details
     - Restart the client Machine
8. Ubuntu Server Setup:
     Ubuntu 24.04 LTs was installed for Linux administrator practice
   Steps:
     - Create new VM in VMware
     - Install Ubuntu using the ISO file
     - Configure static IP Address
     - Enable SSH for remote access
9. Testing Connectivity
    Connectivity between systems was tested using:
       -ping
       -ipconfig
       -ifconfig
       -Remote Desktop
     Successful responses confirm netowkr communication between lab machines
10. Lab Purpose
    This Lab environment is used to practice:
      - Active Directory administration
      - User and Group Management
      - Domain join configuration
      - Network troubleshooting
      - Basic Linux administration
      - IT Support Scenarios
    


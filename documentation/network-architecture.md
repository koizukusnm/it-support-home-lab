Network Architecture
1. Overview
  This document describes the network architecture of the IT Support Home Lab. The environment simulates a small enterprise network using virtual machines hosted on VMware Workstation.

The lab includes a domain controller, client machine, and Linux server connected through a virtual network.

2. Network Topology
  The following diagram represents the logical structure of the lab network.

| Machine | Operating System | Role | IP Address | Services |
|--------|-----------------|------|-----------|----------|
| Host Machine | Windows 11 | Virtualization Host | - | VMware Workstation |
| Windows Server | Windows Server 2022 | Domain Controller | 192.168.10.10 | Active Directory, DNS |
| Windows 11 Client | Windows 11 | Domain User Workstation | 192.168.10.20 | Domain Login Testing |
| Ubuntu Server | Ubuntu 24.04 LTS | Linux Administration Practice | 192.168.10.30 | SSH, Linux Management |

```
Host Machine (Windows 11)
│
├── Windows Server 2022 (Domain Controller)
│   └── IP: 192.168.10.10
│
├── Windows 11 Client
│   └── IP: 192.168.10.20
│
└── Ubuntu 24.04 Server
    └── IP: 192.168.10.30
```

Host Machine (Windows 11)
│
├── Windows Server 2022 (Domain Controller)
│ IP: 192.168.10.10
│ Services: Active Directory, DNS
│
├── Windows 11 Client
│ IP: 192.168.10.20
│ Role: Domain User Workstation
│
└── Ubuntu 24.04 Server
IP: 192.168.10.30
Role: Linux Administration Practice

All virtual machines communicate within the same VMware virtual network.

3. Network Configuration

| Component | Configuration |
|-----------|---------------|
|Network Type| VMware NAT / Host-Only |
| Subnet | 192.168.10.0/24 |
| Gateway | 192.168.10.1 |
| DNS Server | 192.168.10.10 (Windows Server) |

4. IP Address Allocation

| Device | IP Address | Function |
|--------|------------|----------|
| Windows Server | 192.168.10.10| Domain Controller & DNS |
| Windows Client | 192.168.10.20| Domain-joined workstation |
| Ubuntu Server | 192.168.10.30	| Linux server |

Static IP addressing is used to ensure consistent communication between servers and clients.

5. Domain Infrastructure
  The Windows Server is configured as the Domain Controller for the lab environment.

Domain Name:
corp.local
  
  Services configured on the domain controller include:
    -Active Directory Domain Services (AD DS)
    -DNS Server
    
The Windows 11 client machine is joined to the domain for centralized authentication and management.

6. Connectivity Testing
    Connectivity between systems was tested using standard network troubleshooting tools.

Examples:
  Ping test from Windows client to server:
  ping 192.168.10.10

  Ping test from Ubuntu to Windows client:
  ping 192.168.10.20
  
Successful responses confirm that all machines can communicate within the virtual network.

7. Security Considerations
    Basic security practices applied in this lab include:
      -Domain-based authentication
      -Controlled network access within the virtual network
      -Administrator privileges restricted to server management tasks
Future improvements may include firewall configuration and network monitoring tools.

8. Future Enhancements
    Possible improvements for the lab network include:
      -Adding a pfSense firewall
      -Network segmentation using multiple subnets
      -Implementing SIEM monitoring
      -Simulating attack scenarios for security testing
      
Virtual Home Lab Network Image:
<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/5c530f3b-f7b9-40d6-b406-65bc925f4339" />

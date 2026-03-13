Overview
  This document explains how users and workstations were added to the Active Directory environment in the IT Support Home Lab.

Domain name:
  corp.local

Organizational Unit Structure
  To simulate a real enterprise environment, departmental Organizational Units(OUs) were created in Active Directory.

  The following departments were configured:
    - IT  
    - Finance
    - HR

OU Structure:

```mermaid
flowchart TD
    A[corp.local]

    A --> B[IT OU]
    B --> B1[it_admin]
    B --> B2[it_support]

    A --> C[Finance OU]
    C --> C1[finance_user1]

    A --> D[HR OU]
    D --> D1[hr_user1]

    A --> E[Workstations OU]
    E --> E1[WIN11-CLIENT01]

    A --> F[Servers OU]
    F --> F1[DC01]
```

 Each Department can cotain its own users, groups, and computers. This allows administrators to apply different Group Policies and permissions to each department.

  Using Organizational Units allows centralized management of users and simplifies administrative tasks in enterprise environments.

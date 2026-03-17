# Incident Report: Remote Client Support – Windows Update Troubleshooting

## Incident Summary

I assisted a user from the IT department who needed help with Windows Updates on their workstation. I remotely accessed the system using Remote Desktop Protocol (RDP) to verify the update status and ensure all pending updates were installed.

---

## Environment

| Component         | Configuration        |
|------------------|---------------------|
| Domain           | corp.local          |
| Server           | Windows Server 2022 |
| Client System    | Windows 11          |
| Admin System     | Windows 11          |
| Protocol         | RDP                 |
| Admin Account    | corp\Administrator       |

---

## Problem Description

The user could not confirm if their system had installed all Windows Updates. I needed to remotely check the workstation and ensure updates were applied properly.

---

## Investigation

I connected to the user’s machine via RDP and performed the following:

- Checked Windows Update status  
- Reviewed pending or failed updates  
- Verified system update settings  
- Confirmed network connectivity for updates  

---

## Root Cause

The system had pending updates that were not yet installed.

---

## Resolution

I performed the following steps remotely:

- Opened Windows Update settings  
- Checked for available updates  
- Installed pending updates  
- Ensured updates completed successfully  

---

## Verification

After applying updates, I confirmed that the system was fully up to date. The user verified that their workstation was functioning normally and no further issues occurred.

---

## Evidence

All screenshots are stored in:

**Screenshots folder:**[`screenshots/`](IT-Support-Troubleshooting/Scenario-2-Remote-Support/screenshots/)

---

## Skills Demonstrated

- Configuring and using Remote Desktop (RDP)  
- Remote system administration  
- Troubleshooting and managing Windows Updates  
- IT support incident handling  
- Documentation of troubleshooting steps  

---

## Security Considerations

- Restricted RDP access to authorized domain users  
- Used domain credentials for secure authentication  
- Ensured controlled and safe remote administration  

---

## Real-World Relevance

Using RDP, I was able to remotely manage updates and troubleshoot a client workstation efficiently. This reflects common IT support practices in enterprise environments where remote administration reduces downtime and improves response times.

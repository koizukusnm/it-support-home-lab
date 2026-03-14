
# Troubleshooting & Common Errors

This document contains errors encountered during the setup and configuration of the IT Support Home Lab and the steps taken to resolve them. It demonstrates problem-solving skills, practical troubleshooting, and documentation ability.

---

## 1. Windows Server Installation Errors

### Error: “Windows cannot find the Microsoft license terms”
**Cause:** Corrupted or incomplete installation media.  
**Solution:**  
- Verified the ISO file integrity  
- Re-mounted ISO in VMware  
- Restarted installation  

### Error: “Windows setup cannot find the disk”  
**Cause:** Virtual disk not configured properly in VMware.  
**Solution:**  
- Added a virtual SATA/SCSI controller  
- Created a new virtual disk  
- Retried installation

---

## 2. Windows 11 Client Issues

### Error: Domain join failed  
**Cause:** DNS misconfiguration or network issue.  
**Solution:**  
- Verified server IP and DNS settings  
- Ensured Windows client network was set to the same NAT/Host-only network  
- Retried domain join with correct credentials  

---

## 3. Ubuntu Server Installation Errors

### Error: “Unable to find a medium containing a live file system”  
**Cause:** ISO not recognized by VM or corrupted media.  
**Solution:**  
- Re-attached ISO file to VM  
- Verified ISO integrity  
- Rebooted VM

### Error: “Disk full / dpkg sub-process returned an error code”  
**Cause:** VM disk too small or partitions not set correctly.  
**Solution:**  
- Increased virtual disk size  
- Reinstalled Ubuntu  
- Used proper partitioning

---

## 4. Group Policy / Active Directory Issues

### Error: GPO not applying to clients  
**Cause:** Policy not linked to correct OU or replication delay.  
**Solution:**  
- Linked GPO to the correct OU  
- Ran `gpupdate /force` on the client machine  
- Verified with `gpresult /r`  

### Error: Control Panel restriction not enforced  
**Cause:** User permissions override or local policy conflict.  
**Solution:**  
- Checked GPO scope and permissions  
- Ensured client was domain-joined and logged off/logged on

---

## 5. Networking / Connectivity Issues

### Error: Cannot ping server from client  
**Cause:** Network adapter misconfiguration.  
**Solution:**  
- Verified VMware NAT/Host-only network settings  
- Checked IP addresses and subnet masks  
- Confirmed firewall rules

---

## 6. Domain Login Failure – Client Access Issues

### Problem: Login still allowed after disabling account
**Cause:** The Windows 11 client initially allowed login because the local account was used instead of the domain account, or cached credentials were active.  
**Solution:**  
- Ensure the user attempts login with the domain account.  
- Sign out and clear cached credentials if necessary.

### Problem: Event Viewer access denied
**Cause:** Standard users do not have permission to read the Security log; administrative rights were required to view authentication failures.  
**Solution:**  
- Log in with an account that has administrative privileges.  
- Open Event Viewer to check authentication logs.

### Problem: Event log did not appear on Domain Controller
**Cause:** Failed login attempts from a disabled account may not always be logged on the DC immediately; sometimes only the client logs the failure.  
**Solution:**  
- Check both client and DC logs.  
- Ensure DC replication and log settings are correct.


## Notes

This troubleshooting documentation will be updated over time as more errors are encountered and resolved. It demonstrates the ability to **identify, analyze, and fix system issues** in a professional IT lab environment.

# Company Security Policy Lab

**Domain:** corp.local  
**Server:** Windows Server 2022  
**Client:** Windows 11

## Steps

1. Created new GPO: `Company-Security-Policy`
2. Edited GPO to:
   - Disable Control Panel
   - Account Lockout Policy
   - Set Password Complexity
   - Account Lockout Policy
3. Linked GPO to **IT OU**
4. Tested on client machine with `gpupdate /force`
5. Verified policies with `rsop.msc` and `gpresult /r`

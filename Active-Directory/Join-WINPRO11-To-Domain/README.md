# Joining A WindowsPro11 to the Domain Lab

## Objective 
Deploy a Windows 11 Pro Workstation, configure a static IP address, point it to the Domain Controller to the DNS, join it to the "corp.contoso.local" domain, and verify the domian authentication is working.

## Why This Matters
Domain joining workstation is a routine responsibility for Help Desk and System Administration teams. It enables centralized authentication, policy enforcement, and enterprise management of endpoints.

## Steps Performed
- Created a Windows 11 Pro virutual machine named PC-001
- Renamed the computer and configured a static IPv4 address
- Configured DNS to point the Domain COntroller (192.168.50.10)
- Verified network and DNS connectivity
- Joined the workstation to "corp.contoso.locl" domain
- Logged in using domain credentails
- Confirmed the computer object appeared in Active Directory
- Verified domain memebership using command line tools

## Skills Learned
- Install Windows 11 Pro
- Configure a static IPv4 address
- Understand why DNS is critical for domain joins
- Join a computer to a Active Dierctory domain
- Authenticate using domain credentials
- Verify the computer object in Active Directory Troubleshoot common fomain join issues

## Screenshots
Windows Pro 11 Installation
<img width="1024" height="768" alt="2 1InstallingWINPro" src="https://github.com/user-attachments/assets/16325768-51bf-4a83-a9c4-aacae6ffd66b" />

Remnaming PC
<img width="1024" height="768" alt="2 2RenamingWINSPro" src="https://github.com/user-attachments/assets/a5f49464-71f9-492d-bcc9-a991c3510018" />

Making A Static IP
<img width="1024" height="768" alt="2 3StaticIP" src="https://github.com/user-attachments/assets/2f2b45de-2dbf-4e49-9a95-a3b151ace345" />

Pinging Server from Workstation
<img width="1024" height="768" alt="2 4PingServer" src="https://github.com/user-attachments/assets/d38e3e77-5786-4701-93f5-f7ac5e0831d4" />

nslookup Domain Controller
<img width="1024" height="768" alt="2 5nslookupDC" src="https://github.com/user-attachments/assets/668c3c32-018b-4e33-a47c-1e4b6af108c0" />

Joining Workstation to Domain
<img width="1024" height="768" alt="2 6JoiningDomain" src="https://github.com/user-attachments/assets/a2ea7765-0652-4ac2-984b-186fd6233d94" />
<img width="1024" height="768" alt="2 7DomainSuccessful" src="https://github.com/user-attachments/assets/6dfc376f-0003-4bd3-a2a6-5de8b9783b01" />

Logged into Domain with Administrator Credentials
<img width="1024" height="768" alt="2 8AdminDomainLogin" src="https://github.com/user-attachments/assets/6f1080b6-d273-4d7d-942e-7c896359d9d0" />

ID Verification
<img width="1024" height="768" alt="2 9IdentityVerfication" src="https://github.com/user-attachments/assets/14388e9f-036f-45fe-a757-54bf6afe9b3b" />

Verify PC from ADUC
<img width="1024" height="768" alt="2 10VerifyPC-001" src="https://github.com/user-attachments/assets/e56e4812-512e-4af0-a822-f29e3ffb774b" />

## Conclusion

This lab added the first managed workstation to the COntoso Technologies Active Directory enviornment. The client can now authenticate against the Domain Controller and is ready for future management through Organizational Units, Group Policym software deployment, and enterprise security policies.


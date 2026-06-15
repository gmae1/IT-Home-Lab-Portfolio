# AD Intergrated DNs Configuration

## Objective
Configure Windows Server 2022 to function as the AD intergrated DNS for lab environment

## Tools Used

- Windows Sever 2022
- AD DS
- DNS Server
- Windows 11
- Command Prompt
- DNS Manager

## Task Performed

- Verififed that DNS Server is running for Windows Server 2022
- Verified the IPv4 DNS Records in DNS Manager
- Verified the IP Address of the Windows Server 2022 Machine
- From the Windows 11 Client machines I checked the Perfered DNS Server
- Statically Configured the Windows 11 client machine to 192.168.50.10 (Server's DNS)
- Flushed the Windows 11 DNS so that it will be able to accept its new perfered DNS server
- Verified that Windows 11 has connectivity with the server by pinging throgh the hostname (dc1.lab.local)

## Screenshots

DNS Server Running
<img width="1024" height="768" alt="3 1DNS-Service-Running" src="https://github.com/user-attachments/assets/b3a8ce02-1153-4ba2-ae36-0761c46ce0c0" />

DNS Manager DNS Records
<img width="1024" height="768" alt="3 2DNS-Manager-Lab-Local-Zone" src="https://github.com/user-attachments/assets/15a4c083-46e5-41e5-ae5a-fa56e5a9ffc4" />

DNS IPconfig
<img width="1024" height="768" alt="3 3DC1-DNS-Ipconfig" src="https://github.com/user-attachments/assets/0184d336-6b07-4873-b380-3dca6afaf7b3" />

Windows 11 IPconfig
<img width="1024" height="768" alt="3 4win11-DNS-Before" src="https://github.com/user-attachments/assets/81e95820-dbac-467d-ba87-5f78a88b0fc4" />

Windows 11 Perfered DNS Server (Static)
<img width="1024" height="768" alt="3 5win11-ethernet2-dns-config" src="https://github.com/user-attachments/assets/e3d28ae1-215b-4274-b3de-1ada31fe4f6c" />

Flush DNS
<img width="1024" height="768" alt="3 6Flush_DNS" src="https://github.com/user-attachments/assets/40fcf6e7-3cd9-401b-948d-2b24dc5adff6" />

New DNS Perfered DNS Server
<img width="1024" height="768" alt="3 7New-DNS" src="https://github.com/user-attachments/assets/23bff6e3-3de7-418f-9eb8-db4e99c32b2b" />

Ping Connectivity
<img width="1024" height="768" alt="3 8Ping_DC1" src="https://github.com/user-attachments/assets/e112bfe2-b3b1-4a8b-95dc-d3611ec779d0" />

## What I Learned

- Active Directory dpends heavily on DNS
- Prompting a server to a Domain Controller automatically installs and integratess DNS
- Clients in the domain should use the Domain Controller as their DNS Server
- Incorrect DNS serrings can prevent domain resources from being located
- Hostname communication is perfered over using IP address

# Active Directory High Availabilty And Replication

## Objective
Built a redundant Active Directory environment by deployingg a second Windows Server 2022 Domain Controller, configuring Active Directory and DNS replication, exploring FSMO roles, and implementing high availabilty concepts. Verified domain functionality across mulpitle domain conteollers while trouble shooting real-world infrastructe issues releated to DNS, DHCP, and replications

## Skills Demonstrated
- Active Directory Domain Services (AD DS)
- Multi-Domain Controllere Deployments
- Active Directory Replication
- DNS Replication
- Active Directory-Integrated DNS
- FSMO Roles
- FSMO Role Transfer
- High Availability
- Fault Tolerance
- Windows Server Administration
- Powershell
- Active Directory Troubleshooting
- DNS Troubleshooting
- DHCP
- DHCP Dependency Analysis

## Task Performed
- Created a New Virtual Machine (New Microsoft Server 2022)
- Changed new Server name to DC2
- Statically changed DC2 IPv4 Address
- Assigned DC2 to LAB.LOCAL forest
- nslookup DC1 from DC2
- Verified connection between the two servers (DC1 & DC2)
- Assigned DC2 assigne as a AD DS (Active Directory Domain Services)
- Created a new user in DC1 and Verified the Users creation from DC2
- Added New User to Memebrs Of for specific department (IT Admins) from DC1 & Verified Users Memeber Of Status from DC2
- Verified DNS recrods (A Records) from Both Servers (DC1 & DC2)
- Verified DNS Servers are Running for Both Servers
- Verified FSMO Roles
- Checked Operations Masters,
- Powered off DC1 to simulate server being offline
- Changed the Prefered DNS server from DC1 to DC2
- Ping verification from Client Machine and DC2 for network verification
- nslookup from Client Machine to DC2
- Viewed FSMO (Flexible Single Master Operations)
- Assigned different FSMO Roles between the two Servers
- Verified New FSMO Roles

## What I Learned
- How enterprise Active Directory enviroments achieve high availability
- Why organizations deploy multiple Domain Controllers
- Hows Active Domain and DNS replication function together
- The purpose and responsibilities of the five FSMO roles
- The difference between transfering FSMO roles
- Why DNS and DHCP are critical dependencies fro Active Directory
- How to troubleshoot replication, DNS, authentication, and networking issues in a multi-server environment

## Screenshots
New Server (DC2)
<img width="864" height="436" alt="1 1New_Server" src="https://github.com/user-attachments/assets/725a7fd5-4a87-4ad1-afa8-9d8d834525ae" />

Renamed New Server To DC2
<img width="1024" height="768" alt="1 2DC2" src="https://github.com/user-attachments/assets/92d6d342-80e4-48f3-8c65-fffe45e8f7b9" />

Changed IP Address of DC2
<img width="1024" height="768" alt="1 3Static_IP_Address" src="https://github.com/user-attachments/assets/66c3d5e2-706f-4034-99e2-7579fc18c322" />

Assigned DC2 to LAB.LOCAL Forest
<img width="1024" height="768" alt="1 4Member_Of" src="https://github.com/user-attachments/assets/002647fd-0c85-42c4-b998-134bf88c4f04" />

Connection Verification
<img width="1024" height="768" alt="1 6Connection" src="https://github.com/user-attachments/assets/1d5b5017-e5f2-4e22-a804-b223af541be6" />

nslookup DC1 from DC2
<img width="1024" height="768" alt="1 5nslookup_DC1" src="https://github.com/user-attachments/assets/9d78284d-eb9d-45ce-8586-7a232b0bef93" />

Assigned DC2 Roles (Domain Controller, DNS Server and DHCP Server)
<img width="1024" height="768" alt="1 7DC2_Roles" src="https://github.com/user-attachments/assets/aee5139e-f770-4203-bbb4-9fb6838a79bf" />

Domain Controller Verification
<img width="1024" height="768" alt="1 9Domain_Controllers_Verification" src="https://github.com/user-attachments/assets/2aa35d17-445d-4c55-b88c-2cb7c7b1f150" />

Creating A New User With DC1
<img width="1024" height="768" alt="1 10Creating_New_User_DC1" src="https://github.com/user-attachments/assets/d6b771ab-6040-4667-99e0-53f6c00da080" />
<img width="1024" height="768" alt="1 11Creating_New_User_DC1" src="https://github.com/user-attachments/assets/49e5ec3f-6a6c-4e0a-a39b-ae0c067596a2" />

Verified the Users Account On DC2
<img width="1024" height="768" alt="1 12User_On_DC2" src="https://github.com/user-attachments/assets/cf84b27b-7c6d-4171-88f2-37cb0689c7b8" />

Verified the User on Powershell
<img width="1024" height="768" alt="1 13Verified_From_PWS" src="https://github.com/user-attachments/assets/1bc0918c-b129-45c0-9db6-97a3e78a91db" />

Adding New User to Member Of (IT Department)
<img width="1024" height="768" alt="1 14Adding_Mike_IT" src="https://github.com/user-attachments/assets/e4a826be-4293-4df9-b022-64bddb230b62" />

Verified New User is apart of Member Of (IT Department) in DC2
<img width="1024" height="768" alt="1 15Mike_MemberOf_DC2" src="https://github.com/user-attachments/assets/07070761-c663-4a87-8714-5cd2517ff2b2" />

Viewed DNS A Records
<img width="1024" height="768" alt="1 16Verfy_DNS_Host_DC1" src="https://github.com/user-attachments/assets/1360d3c0-7032-4210-825b-a3d05ba1dc95" />
<img width="1024" height="768" alt="1 17Verify_DNS_Host_DC2" src="https://github.com/user-attachments/assets/d8fef91d-1205-403c-8d76-bab04c0bbc7e" />

Verified DNS is running for both Servers
<img width="1024" height="768" alt="1 18DNS_Running_DC1" src="https://github.com/user-attachments/assets/42dc3408-22d9-4bfc-9534-4b21ccaaacd8" />
<img width="1024" height="768" alt="1 19DNS_Running_DC2" src="https://github.com/user-attachments/assets/cac69fdd-d6ac-49c3-ba08-6799d147db01" />

Creating a Test Server on DC1
<img width="1024" height="768" alt="1 20Creating_Test_Server_DC1" src="https://github.com/user-attachments/assets/a1552851-6e97-4f44-abc0-c2de24ecde3e" />

Verified Test Server was Successful from DC2
<img width="1024" height="768" alt="1 21Verify_Test_Server_On_DC2" src="https://github.com/user-attachments/assets/38f2e849-6c0d-4227-b79b-2ec993a43bfa" />

nslookup Test Server 
<img width="1024" height="768" alt="1 22nslookup_TestServer" src="https://github.com/user-attachments/assets/80401012-3df9-4c54-9a3b-68a9585af7fe" />

Viewed FSMO Roles (Flexible Single Master Operation) from Powershell
<img width="1024" height="768" alt="1 23FSMO_Roles" src="https://github.com/user-attachments/assets/a1de3a75-f393-4608-a50f-b1eedbd91b91" />

Vewing Operation Masters
<img width="1024" height="768" alt="1 24Operations_Masters" src="https://github.com/user-attachments/assets/4a10b5c6-0751-45fc-afc6-f357db522ec8" />
<img width="1024" height="768" alt="1 25OM_Domain_Naming" src="https://github.com/user-attachments/assets/23253521-d523-4ec2-9290-e0f5d6c75108" />
<img width="1024" height="768" alt="1 27Console_Root" src="https://github.com/user-attachments/assets/ab192b64-0d95-414f-abda-3d33bdaed76c" />

Assigned FSMO Roles Between The Two Servers
<img width="1024" height="768" alt="1 35Assigning_FSMO_Roles" src="https://github.com/user-attachments/assets/c7b56551-886b-40de-b49e-041a96df7a0b" />

Verified New FSMO Roles
<img width="1024" height="768" alt="1 36FSMO_Roles_Verified" src="https://github.com/user-attachments/assets/9d878deb-510a-485e-b258-9c5db14a4a33" />

Simulated DC1 being off the Network
<img width="1024" height="768" alt="1 29Hostname_DC2" src="https://github.com/user-attachments/assets/6005eaf3-69f5-4f07-9b96-c65f7eb28c7b" />
<img width="833" height="482" alt="1 28PowerOff_Dc1" src="https://github.com/user-attachments/assets/ad87846a-d67d-4cf9-a159-759aa7d797f9" />

Changed Client DNS Server from DC1 to DC2
<img width="1024" height="768" alt="1 31Change_DNS_Server" src="https://github.com/user-attachments/assets/2b67035d-6fe0-434d-91e0-79bf3ea40513" />

 CLient Machine Verifies Connection of DC2
 <img width="1024" height="768" alt="1 32Ping_Verification" src="https://github.com/user-attachments/assets/7b5a59c9-6645-4076-a9e0-168557d73802" />

nslookup DNS Server (DC2) from client machine
<img width="1024" height="768" alt="1 33nslookup_dc2" src="https://github.com/user-attachments/assets/4100813e-4723-4234-94ec-85d7c5813df8" />

## Conclusion
Built a redundant Active Directory environment using two Windows SErver 2022 Domain Controllers, configured Active Directory, DHCP server and DNS replication, validated high availability through failover testing, managed FSMO toles and resolved real-world DNS, DHCP, and replication issues using PowerShell and Windows admin tools.


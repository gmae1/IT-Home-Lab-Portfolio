# Windows Server 2022 Initial Configuration

## Objective
Prepare a newly installed Windows Server 2022 machine for Active Directory deployment by renaming the server, assigning a static IP address, and verifying communication with exsiting lab systems

## Tools Used

- Windows Server 2022
- VirtualBox
- Server Manager
- Command Prompt

# Task Performed

- Installed Windows Server 2022 Desktop Experience
- Renamed the server to DC1
- Assigned the static IPv4 address
- Configured DNS setting
- Verified network connectivity with Windows 11 and Ubuntu
- Confirmed the hostname change after reboot

## Screenshots

Windows Server 2022 Desktop Experience Instalation
<img width="1024" height="768" alt="1 1Window_Server_StaticIP" src="https://github.com/user-attachments/assets/c4eeb6a7-6d5c-49be-a6b3-b8e5b088a4d0" />

Static IP Address
<img width="1024" height="768" alt="1 1Window_Server_StaticIP" src="https://github.com/user-attachments/assets/2d1fdb8e-d445-45f7-846f-b21ffdddb784" />

Verification of IP Address
<img width="1024" height="768" alt="1 3WindowsClient_IP" src="https://github.com/user-attachments/assets/4f303478-a81d-40d7-b6b1-e5c89b96b41d" />

Windows (Client) IP Address
<img width="1024" height="768" alt="1 3WindowsClient_IP" src="https://github.com/user-attachments/assets/aff5f9d4-eb32-43b5-83ea-07e39b554ad1" />

Ubuntu IP Address
<img width="1280" height="800" alt="1 4Ubuntu_IP" src="https://github.com/user-attachments/assets/c7b90a0a-3fb8-445c-bbec-8e24fc0e62be" />

Successful Ping from Windows Server
<img width="1024" height="768" alt="1 5Ping_Successful" src="https://github.com/user-attachments/assets/ee76a576-b459-4525-b1b2-9663770fbc6b" />

Change Server Name
<img width="1024" height="768" alt="1 6Change_CPU_Name" src="https://github.com/user-attachments/assets/bcb5d8d5-f0d8-42bf-abdd-0532716e85ce" />

Hostname Verification
<img width="1024" height="768" alt="1 7Hostname_Change" src="https://github.com/user-attachments/assets/237006ca-f1e6-4a43-afd6-8f6fd1c11bc9" />

## What I Learned 

- Windows Servers typically use static IP addresses
- Server Manager provides centralized administration tool
- Hostnames should folllow meaningful naming
- Domain Controllers require reliacble IP addressing
- Connectivity should be verified before installing Active Directory
- ICMP ping can be used to validate communication between host

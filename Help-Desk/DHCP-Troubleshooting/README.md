# DHCP Troubleshooting

## Objective
Practice Troubleshooting DHCP-related connectivity issues using Windows Command Prompt tools.

## Tools Used
- Windows 11
- VirtualBox
- Command Prompt

## Task Performed
- Review current IP configuration
- Verified DHCP was enabled
- Released DHCP lease
- Observed loss of network connectivity
- Renewed DCHP lease
- Restored network connectivity
- Reviewed DHCP lease information

## Commands Used

###cmd
- ipconfig
- ipconfig /all
- ipconfig /release
- ipconfig /renew
- ping 8.8.8.8

## Screenshots

Current IP Configuration
<img width="1024" height="768" alt="11 1Current_IP" src="https://github.com/user-attachments/assets/b649744c-41cf-4fc0-a88c-8a8b3c9fafb4" />

DHCP Enabled Verification
<img width="1024" height="768" alt="11 2DHCP_Enabled" src="https://github.com/user-attachments/assets/f6a9c8ec-80b5-4780-b068-2fde8b92fd59" />

DHCP Lease Release
<img width="1024" height="768" alt="11 3Release_Address" src="https://github.com/user-attachments/assets/1fb08f94-8f20-415f-bee6-e975b7d67d01" />

IPv4 APIPA Address
<img width="1024" height="768" alt="11 4APIPA" src="https://github.com/user-attachments/assets/9383cc98-a25b-4bc5-9b63-e4113c8fe0df" />

Connectivity Loss Verification
<img width="1024" height="768" alt="11 5Connectivity_Lost" src="https://github.com/user-attachments/assets/58be350f-6605-4f90-bb0f-489182270c54" />

DHCP Lease Renewal
<img width="1024" height="768" alt="11 6Renew_Address" src="https://github.com/user-attachments/assets/c0f7d87b-f33c-4abd-8e4f-5fa762ad9336" />

Connectivity Restored
<img width="1024" height="768" alt="11 7Connectivity_Restored" src="https://github.com/user-attachments/assets/a89103b9-4089-450c-8fdf-b3e898211f06" />

DHCP Lease Information
<img width="1024" height="768" alt="11 8Lease_Information" src="https://github.com/user-attachments/assets/be810676-2717-4231-b8e4-61488f931155" />

## What I Learned
- How DHCP automatically assign IP addressing information
- How to verify wether DHCP is enabled on a Windows syste,
- How to release and renew DHCP leases using Command Prompt
- How DHCP issues can impact internet connectivity
- How to use ping to verify network connectivity
- How to identify DHCP server and lease information
- Basic DHCP troubleshooting techniques used by Help Desk technicians.

# Wireshark DHCP DORA Packet Analysis

## Objective
Capture and analyze DHCP traddic using Wireshark to observe how a client obtains a IP address throgh the DORA process

## Tools Used

- Windows 11
- VirtualBox
- Wireshark
- Command Prompt

## Task Performed

- Capture DHCP trafic using Wireshark
- Applied DHCP packets filters
- Release the current IP address
- Renewed the IP address
- Observed the complete DORA sequence
- Analyzed DHCP communication betwwen the client and DHCP server
- Verified successful IP address assignment

## Screenshots

Wireshark Interface
<img width="1024" height="768" alt="7 1 WireShark_Interface" src="https://github.com/user-attachments/assets/26233d4b-7fef-47f6-a948-f5c8d2114eab" />

BootIP Filter
<img width="1024" height="768" alt="7 2Bootp_Filter" src="https://github.com/user-attachments/assets/c79108e7-32c7-48ce-b13e-1f36b9b134e5" />

Current IP Address
<img width="1024" height="768" alt="7 3Current_IP" src="https://github.com/user-attachments/assets/8a08bf60-ad02-4b48-8b3c-c33ff86f395b" />

Release IP 
<img width="1024" height="768" alt="7 4Release_IP" src="https://github.com/user-attachments/assets/998a3543-00c8-4af7-8a36-dd47958ab88d" />

Renew IP
<img width="1024" height="768" alt="7 5Renew_IP" src="https://github.com/user-attachments/assets/ec2da22b-4532-457e-8596-cd1280c4d0db" />

DHCP DORA
<img width="1024" height="768" alt="7 6DORA" src="https://github.com/user-attachments/assets/b863a413-482c-4e08-b830-5f4d5c7dfaf9" />

## What I Learned

- DHCP dynamically assigns IP addresses to clients
- DHCP traffic appers as BOOTP packets in Wireshark
- The DORA proccess consists of Discover, Offer, Request, ACK
- DHCP uses UDP port 67 & 68
- Clients intially broadcast without knowing their IP address
- DHCP servers offer available IP addresses
- Clients request the offered address
- DHCP servers acknowledge and finalize the lease
- Successful DHCP communication is required for network commectivity


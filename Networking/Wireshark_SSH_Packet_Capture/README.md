# Wireshark SSH Packet Capture

## Objective
Capture and anaalizye SSH traffic between a Windows workstation and an Ubuntu Linux server using Wireshark

## Tools Used
- Windows 11
- Ubuntu Linux
- VirtualBox
- WireShark
- OpenSSH Server
- Command Prompt
- Linux Terminal

## Task Performed

- Established an SSH connection from Windows to Ubuntu
- Capture network traffic is using Wireshark
- Applied packet filterrs to isolate SSH traffic
- Identified communication over TCP port 22
- Examinied TCP packet details
- Followed the TCP stream between client and server
- Observed encrypted SSH traffic
- Verified that commmand data and credntials were protected

## Commands Used

### Windows

#### cmd
- ssh vboxuser@192.168.1.78

### ubuntu

#### bash
- whoami
- hostname
- pwd
- exit

#### Wireshaek
- tcp.port == 22

## Screenshots

Wireshark Interface
<img width="1024" height="768" alt="3 1WireShark_Interface_Selected" src="https://github.com/user-attachments/assets/a966a55e-76f2-43c5-a043-78e02ff0df1d" />

SSH Filter
<img width="1024" height="768" alt="3 2SSH-Filter" src="https://github.com/user-attachments/assets/2b3fbbae-bcb7-4116-95e0-a696ffed8e41" />

SSH Commands
<img width="1024" height="768" alt="3 3SSH_Commands" src="https://github.com/user-attachments/assets/83b590fa-7c64-4e4c-b673-cdcb118eaddf" />

SSH Packets in Wireshark
<img width="1024" height="768" alt="3 4SSH_Packets" src="https://github.com/user-attachments/assets/4b5ecf3f-5767-48e4-929b-554a132fc496" />

TCP Details
<img width="1024" height="768" alt="3 5TCP_Details" src="https://github.com/user-attachments/assets/d0ecb928-43be-4029-b98a-69c0ea972b00" />

TCP Stream
<img width="1024" height="768" alt="3 6Follow_TCP" src="https://github.com/user-attachments/assets/b2211c18-ddb6-496b-b692-fc2b4d595559" />

## What I Learned 

- How Wireshark capture network traffic
- How SSH communication uses TCP port 22
- How to filter traffic using packet filtering
- How to identify source and destination IP addresses
- How TCP packets form conversation between client and source
- How to follow a TCP stream in Wireshark
- How SSH encrypts traffic and protects commands and credentials
- Why SSH is perferred over insecure prtocols such as Telnet

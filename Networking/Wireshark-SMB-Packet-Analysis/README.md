# Wireshark SMB Paacket Analysis

## Objective
Capture and analyze SMB traffic between Ubuntu and Windows while accessing a shared folder and transferring files.

## Tools Used

- Windows 11
- Ubuntu Linux
- VirtualBox
- Wireshark
- SMB Client (smbclient)
- Linux Terminal

## Task Performed
- Verified SMB connectivity betwwen Ubuntu and Windows
- Connected to the CompanyShare folder
- Navigated directories within the share
- Listed files and folders remotly
- Downloaded a text file from the Windows share
- Captured SMB traffic using Wireshark
- Analyze SMB2 packets and protocol operations
- Observed authentication and file access processes

## Commands Used

### Ubuntu
- smbclient //192.168.1.153/CompanyShare -U "LAB-NET/vboxuser"

## Screenshots

Wireshark Interface
<img width="1024" height="768" alt="5 1Wireshrl_Interface_Selected" src="https://github.com/user-attachments/assets/12e0d9c8-c65d-4e77-a365-2cc38d5037e4" />

SMB Filter
<img width="1024" height="768" alt="5 2SMB_Filter" src="https://github.com/user-attachments/assets/bef99d9e-90f2-4ec4-9da3-3d05a8ae3c0e" />

CompanyShare Connected
<img width="1280" height="800" alt="5 4SMB_Windows_Folder" src="https://github.com/user-attachments/assets/561916cd-7365-4b5a-a359-729ee7c62052" />

Downloading Secret Message Text
<img width="1280" height="800" alt="5 8Downloading_Windows_Txt" src="https://github.com/user-attachments/assets/19fdb323-d722-45f7-ae45-2687edf4ce6d" />

Successful Text
<img width="1280" height="800" alt="5 9Successfully_Accesssed_Txt" src="https://github.com/user-attachments/assets/fa1ad745-1006-44c2-a0b2-73380cc1e4f4" />

SMB Packets
<img width="1024" height="768" alt="5 6SMB_Packets" src="https://github.com/user-attachments/assets/ca508246-c98e-4984-ae91-7c0af8374197" />

SMB Details
<img width="1024" height="768" alt="5 7SMB_Details" src="https://github.com/user-attachments/assets/a26e213c-5b75-4420-8e04-5f0a09835577" />

## What I Learned
- How SMB uses TCP port 445 for file sharing
- How to remotly access Windows shared folders
- How to navigate directories using smbclient
- How to transfer files across the network
- How Wireshark captures traffic
- How SMB authentication works
- How SMB2 negotiation and session setup occur
- How Tree Connect request establish access to shared folders
- How file operations generate network traffic

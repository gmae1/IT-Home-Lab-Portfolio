# Nmap Network Discovery

## Objective
Use Nmap to discover hosts, identify open ports, and enumerate network services running on a Windows system from an Ubuntu machine.

## Tools Used 

- Ubuntu Linux
- Windows 11
- VirtualBox
- Nmap
- Terminal

## Task Performed

- Verified connectivity between Ubuntu and Windows machine
- Installed and verified Nmap
- Performed basic host discovery
- Scanned the Windows machine for open ports
- Enumerated services running on open ports
- Investigated firewall effects on Nmap scans
- Observed filtered ports caused by Windows Firewall

## Screeenshots
Windows Firewll Turned On
<img width="1024" height="768" alt="8 4Turned_Firewall_Back_On" src="https://github.com/user-attachments/assets/d010dd33-47fd-4540-a6c6-8b7cde4a536a" />

Nmap Scan is Unsuccessful
<img width="1280" height="800" alt="8 5Nmap_Unsuccessful" src="https://github.com/user-attachments/assets/9ab712b8-b438-4bcc-95de-85dae53bb436" />

Windows Firewalls Turned Off
<img width="1024" height="768" alt="8 1Windows_Firewalls_Off" src="https://github.com/user-attachments/assets/b14dd365-fccc-467c-a96b-9ed5476a5585" />

Ubuntu Nmap Scan
<img width="1280" height="800" alt="8 2Nmap_Scan" src="https://github.com/user-attachments/assets/387dcf98-2ffc-41cd-8754-ee737f3e658c" />

Ubuntu Service Enumeration
<img width="1280" height="800" alt="8 3Service_Version_Scan" src="https://github.com/user-attachments/assets/d31f84ac-d092-4855-b24b-78b988da92fc" />

Windows Firewall Turned Back On
<img width="1024" height="768" alt="8 4Turned_Firewall_Back_On" src="https://github.com/user-attachments/assets/ad22f155-3365-472c-8dd8-c8591ac477cc" />

## Why Windows Firewall was Disabled

- Firewalls can hide services from scanners
- ICMP filtering may cause host to appear offline
- Filtered ports do not necessarily mean the host is down
- Security controls directly affect network visibility

## What I Learned

- Nmap can discover host and open ports on a network
- Windows Firewall affects scan results
- Filtered ports are different from closed ports
- Port 135 is used by Microsof RPC
- Port 445 is used by SMB file sharing
- Enumeration is the process of gathering information
- Open ports reveal services available on a system

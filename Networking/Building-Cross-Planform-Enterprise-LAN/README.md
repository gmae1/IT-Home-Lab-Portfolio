# Building A Cross Platform Enterprise LAN Lab

## Objective
Building a functional; enterprise lab network by integrating Windows Server 2022, Windows 11 Pro, Ubuntu Server, and Ubuntu Desktop into the same VirtualBox internal network

Configure static IPv4 addressing for each system and verify end to end communication to establish the networking foundation for future enterprise labs.

## Why This Lab Matters
Enterprise environments rarely consist of only Windows Computers.

System Administrators routinely manage environments containing:
- Windows Servers
- Windows Workstations
- Linux Servers
- Virtual Machines
- Other Operating Systems

Before deploying enterprise technologies like Active Directory, pfSense, VLANs, Azure, or Microsoft 365, administrators must first ensure every system can communicate across the network.

Hiring managers value candidates who understand how to integrate multiple operating systems into a single network rather than working with only Windows.

## Task Performed

### Windows Machine
- Verified communication between Windows Server 2022 and Windows Pro 11
- Confirmed both systems were configured on the 192.168.50.0/24 internal network.
- Verified DNS services were provided by the Domain Controller (192.168.50.10)

### Ubuntu Server 
- Connected Ubuntu Server to the LabNet Internal Network
- Configured a static IPv4 address: 192.168.50.30/24
- Configured DNS: 192.168.50.10
- Verified the static IP using: ip addr
- Confirmed connectivity with Windows systems.

### Ubuntu Desktop
- Connected Ubuntu Desktop to the LabNet internal network
- Configured a static IPv4 address through NetworkManager: 192.168.50.31
- Configured DNS: 192.168.50.10
-Verified successful communication with all Windows and Linux System.

## Network Verification 
Verified communication using:
  - ping
  - ip addr
  - ipconfig

## Skills Learned
- Virtualbox networking
- NAT vs Internal Networking
- Static IPv4 configuration
- Enterprise IP addressing
- DNS configuration
- Ubuntu Netplan
- Ubuntu NetworkManager 
- Crossplatform networking
- Linux networking fundamentals
- Windows netowrking fundamnetals
- Windows networking fundamnetals
- Basic enterprise network verifcation

## Screenshots 
Domain Controller IP Address
<img width="1024" height="768" alt="1 1" src="https://github.com/user-attachments/assets/fd908a0b-0bce-4f62-ae3f-81d2fb36abca" />

Windows Pro IP Address
<img width="1024" height="768" alt="1 2Win11IP" src="https://github.com/user-attachments/assets/42b7af7e-1670-4fcb-827e-bef9b5fe19de" />

Ubuntu Server IP Address
<img width="1280" height="800" alt="1 3UbuntuServerIP" src="https://github.com/user-attachments/assets/5f9b5449-da3d-4541-9106-0f6e14a00f23" />

Ubuntu Desktop IP Address
<img width="1280" height="800" alt="1 4UbuntuDeskIP" src="https://github.com/user-attachments/assets/75027d74-02c2-4d50-93c6-203b3fb63462" />

Windows Server Pinging All Devices
<img width="1024" height="768" alt="1 5WServerPing" src="https://github.com/user-attachments/assets/65b0c5ba-2ca4-40d1-b45f-d0149133e611" />

Windows Desktop Pinging All Devices
<img width="1024" height="768" alt="1 6WDeskPing" src="https://github.com/user-attachments/assets/8da192b5-261c-4b97-9e1d-778c981f9591" />

Ubuntu Server Pinging All Devices
<img width="1280" height="800" alt="1 7UServerPing" src="https://github.com/user-attachments/assets/4b309de5-7e0f-46c9-8bcc-35b021a17fc0" />

Ubuntu Desktop Pinging All Devices
<img width="1280" height="800" alt="1 8UDesktopPing" src="https://github.com/user-attachments/assets/df0fa2c4-8eac-4da8-89ac-7174c5dae1d9" />

netplan Ubuntu Server Configurations
<img width="1280" height="800" alt="1 9netplan" src="https://github.com/user-attachments/assets/65cdf6f0-55dc-4702-96ee-0e9d5e019704" />

Ubuntu Desktop IP Configuration
<img width="1280" height="800" alt="1 10UDesktopConfi" src="https://github.com/user-attachments/assets/9d0740c2-ef07-44d5-b931-1326f5e35902" />

## Conclusion
A functional cross platform enterprise LAN was successfully built using Windows Server 2022, Windows 11 Pro, Ubuntu Server, and Ubuntu Desktop.

Each virtual machine was assigned a static IPv4 address on the 192.168.50.0/24 subnet and configured to use the Domain Controller as its DNS server. Communication was verified across all four systems, providing a stable networking foundation for future labs.

This environment will serve as the baseline infrastructure for upcoming projects involving asset inventory, network diagrams, pfSense deployment, VLAN implementation, firewall configuration, Azure integration, Microsoft 365 connectivity, and enterprise network security.

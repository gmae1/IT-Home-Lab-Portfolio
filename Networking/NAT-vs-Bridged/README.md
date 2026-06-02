# NAT vs Bridged Lab

## Objectives
Compare NAT and Bridge netorking modes in VirtualBoc and observe how each configuration afffects IP addressing and networking connectivity.

## Tools Used
- Windows 11
- VirtualBoc
- Command Prompt

## Task Performed
- Reviewed VirtualBoc netwok adapter settings
- Configured a virtual machine to use NAT networking
- Identified NAT  IP addressing information
- Tested internet connectivity using ping
- Configured a virtual machine to use Bridge networking
- Identified Bridge IP addressing information
- Compared network behavior between NAT nd Bridge modes
- Reviewed DHCP, DNS and gateway information.

## Commands Used

### cmd
- ipconfig
- ipconfig /all
- ping 8.8.8.8
- ping google.com

## Screenshots 

VirtualBox Network Adapter Settings
<img width="1919" height="1079" alt="10 1Network_Adapter_Settings" src="https://github.com/user-attachments/assets/4da943c9-f5d5-4d8b-a8f2-0dcc549054c1" />

NAT IP Configuration
<img width="1024" height="768" alt="10 2NAT_IPconfig" src="https://github.com/user-attachments/assets/a1349c14-7cca-4cc0-99e7-854c1f9de586" />

NAT Connectivity Test
<img width="1024" height="768" alt="10 3NAT_Ping_Test" src="https://github.com/user-attachments/assets/45772a53-a426-4921-8187-ec8015b83911" />

Bridge Adapter
<img width="1911" height="1079" alt="10 4Bridge_Adapter" src="https://github.com/user-attachments/assets/55cf4aa8-a4cb-409f-a8a7-7033e4466533" />

Bridge IP Configurations
<img width="1024" height="768" alt="10 5Bridge_Ipconfig" src="https://github.com/user-attachments/assets/b4ac0ffc-5b0d-4e83-9015-5033b8bddaf9" />

Bridge vs NAT Comparison
<img width="1024" height="768" alt="10 6Bridge_Ipconfig_All" src="https://github.com/user-attachments/assets/dfe2518c-028e-4723-be90-3c0ecdbde044" />
<img width="1024" height="768" alt="NAT_IPconfig_All" src="https://github.com/user-attachments/assets/515a9521-5552-4c0e-8a7d-7a52589c403a" />

## What I learned
- How NAT networking allows a virtual machine to access the internet through the host system
- How Bridge networking places a virtual machine directly on the physical network
- How IP addressing differes between NAT and Bridge mode
- How DHCP assigns network configuration information
- How to verify internet and DNS connectivity using ping
- How network adapter configuration affects communication betwwen devices






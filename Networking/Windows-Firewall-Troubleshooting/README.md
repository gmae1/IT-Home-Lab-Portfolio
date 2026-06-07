# Windows Firewall Troubleshooting

## Objective

Troubleshoot network connectivity issues by identifying and modifying

## Tools Used

- Windows 11
- Ubuntu Linux
- VirtualBox
- Windows Defender Firewall with Advanced Security
- Command Prompt
- Linux Terminal

## Task Performed

- Verified network connectivity between Windows and Linux
- Test ICMP communication using ping
- Examined Windows Defender Firewall inbound rules
- Disabled ICMP Echo Request firewall rules
- Verified ping traffic was blocked in Linux
- Re-enabled firewall rules
- Confirmed network connectivity was restored

## Commands Used

### Windows

'''cmd
ping 192.168.1.73
'''

### Ubuntu
'''bash
ping 192.168.1.153
'''

## Screenshots

Successful Windows Ping
<img width="1024" height="768" alt="2 1Ping_Works" src="https://github.com/user-attachments/assets/4fa42426-65f6-4236-8d52-10a94f63afdf" />

Successful Ubuntu Ping
<img width="1280" height="800" alt="2 2Ubuntu_Ping_Works" src="https://github.com/user-attachments/assets/2618c695-4e27-46fb-b711-8b8e5cbdc216" />

Inbound ICMP Rules Disabled
<img width="1024" height="768" alt="2 4ICMP_Rule_Disabled" src="https://github.com/user-attachments/assets/1b0079b3-d100-4284-aefa-81adfecd4efc" />

Linux Ping Unsuccessful
<img width="1280" height="800" alt="2 5Ping_Failure" src="https://github.com/user-attachments/assets/c51f19e1-9c46-4f2e-9274-1e8d0c1b7bf5" />

Inbound ICMP Rules Enabled
<img width="1024" height="768" alt="2 6ICMP_Rules_Enabled" src="https://github.com/user-attachments/assets/7f7cb3e8-a747-4c6a-8947-801cabb436ce" />

Linux Ping Successful
<img width="1280" height="800" alt="2 7Ping_Restored" src="https://github.com/user-attachments/assets/9e9fbec1-2763-4d5a-85ae-4d40f5d79287" />

## What I Learned
- How WIndows Defender Firewall controls inbound network traffic
- How ICMP is used to test connectivity betwwen systems
- How firewall rules can impact network traffic
- How to identify the difference between a network issue and a firewall issue
- How to investigate unexpected troubleshooting results
- How to verify that a configuration change resolves an issue
- The importance of validating connectivity before and after changes

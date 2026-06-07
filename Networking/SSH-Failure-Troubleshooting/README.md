# SSH Failure Troubleshooting

## Objective
Troubleshoo and restore SSH connectivity

## Tools Used

- Windows 11
- Ubuntu Linux
- VirtualBox
- OpenSSH Server
- Command Prompt
- Linux Terminal
- systemctl

## Task Performed

- Verified SSH connectivity failures from Windows
- Configured network connectivity using ping command
- Investigated SSH service status on Ubuntu
- Discovered SSH socket activation
- Analyzed services dependencies and triggers
- Restarted SSH services
- Verified port 22 availabilty
- Restored remote SSH access
- Validated successful remote administration

## Commands Used

### Windows

'''cmd
ping 192.168.1.78
ssh vboxuser@192.168.1.78

### Ubuntu

'''bash
sudo systemctl start ssh.socket
sudo systemctl start ssh
sudo ss -tupln | grep :22

## Screenshots

SSH Unsuccessful
<img width="1024" height="768" alt="1 1SSH_Ubsuccessful" src="https://github.com/user-attachments/assets/61fba5a0-850f-461f-a365-43e821eb037e" />

Successful Ping
<img width="1024" height="768" alt="1 2Successful_Ping" src="https://github.com/user-attachments/assets/baf34e26-73b4-474b-98a7-85f29b519b10" />

SSH Inactive
<img width="1280" height="800" alt="1 3SSH_Inactive" src="https://github.com/user-attachments/assets/0ba6e93d-3ad7-4702-9166-3ed502269e50" />

Port 22 Not Listening
<img width="1280" height="800" alt="1 4Port22_NotListening" src="https://github.com/user-attachments/assets/36f3fefd-5abe-462e-8c6e-587b74881bcb" />

Starting up SSH Services
<img width="1280" height="800" alt="1 5Startin_SSH_Services" src="https://github.com/user-attachments/assets/067781d4-218d-453a-871c-2ea799ad0161" />

Service Active Again
<img width="1280" height="800" alt="1 6Services_Starting_Again" src="https://github.com/user-attachments/assets/350830cf-0eec-4f53-9189-d9c64eeb3e14" />

Port 22 is Listening
<img width="1280" height="800" alt="1 7Port22_Listening" src="https://github.com/user-attachments/assets/adc60582-b4c3-45b9-81f6-074b36a56810" />

SSH working from Windows
<img width="1024" height="768" alt="1 8SSH_Working_Again" src="https://github.com/user-attachments/assets/2b85baf9-155b-4118-a3dc-0534f148f7f2" />

## What I learned

- How to troubleshoot SSH connectivity issues
- How to verify service health using systemctl
- How SSH depends on TCP port 22 for remote access
- How to distinguish between network issues and service failure
- How Linux socket activation can automatically start services
- How to identify root cause during remote access outages
- How to restore SSH functionality and verify resoultion
- The importance of validating fixes after troubleshoooting




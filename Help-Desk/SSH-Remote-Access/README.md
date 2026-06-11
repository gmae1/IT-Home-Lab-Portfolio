# SSH Remote Access Lab 

## Objective
Configure OpenSSH Server on Ubuntu and establish a secure remote connection from a Windows workstation using SSH

## Tools Used
- Windows 11
- Ubuntu Linux
- Open SSH Server
- Command Prompt
- Linux Terminal

## Task Performed
- Verified network connectivity between Windows and Ubuntu virtual machine
- Installed OpenSSH Server on Ubuntu
- Started and enabled the SSH server
- Verified SSH service status
- Confirimed SSH was listening on TCP port 22
- Identified Ubuntu IP address
- Established an SSH connection from Windows to Ubuntu
- Executed Linux commands remotely
- Successfuly closed the remote session

## Commands Used

### Ubuntu (bash)
- sudo apt update
- sudo apt install openssh-server -y
- sudo systemctl start ssh
- sudo systemctl enable ssh
- sudo systemctl status ssh
- sudo ss -tupln | grep ssh

### Windows (cmd)
- ipconfig
- ping 192.168.1.78
- ssh virtualbox@192.168.1.78

## Screenshots

Virtualbox Network Settings
<img width="1636" height="804" alt="15 1Windows_Settings" src="https://github.com/user-attachments/assets/b3b72374-b909-4c49-8e56-080d40fffc67" />
<img width="1876" height="658" alt="15 2Ubuntu_Settings" src="https://github.com/user-attachments/assets/d67efca1-a99b-425d-b4aa-41fcca9956a1" />

Ubuntu Internal IP
<img width="1280" height="800" alt="15 4UbuntuIpA_PingWindows" src="https://github.com/user-attachments/assets/505196f8-7c42-451d-bc56-67b85aab9711" />

SSH Services Active
<img width="1280" height="800" alt="15 10SSH_Verification" src="https://github.com/user-attachments/assets/9518bc79-12a2-4724-9f4e-5599576b18ef" />

Windows Ping Ubuntu
<img width="1024" height="768" alt="15 3WindowsIPconfig_PingUbuntu" src="https://github.com/user-attachments/assets/60f6ffec-7377-4a94-bd91-e92b248fcdf9" />

SSH Port 22 Listening
<img width="1280" height="800" alt="15 6Verify_22_Listening" src="https://github.com/user-attachments/assets/5c654c8e-d967-4f0c-9bfd-155f00019a4f" />

SSH Login Success
<img width="1024" height="768" alt="15 7Windows_SSH_Ubuntu" src="https://github.com/user-attachments/assets/30e0f130-ccc2-4c43-b3f8-3479692dec3c" />

Remote Commands
<img width="1024" height="768" alt="15 8Ubuntu_Commands_Windows" src="https://github.com/user-attachments/assets/0bdfb5f1-e35a-476d-9cdc-af2c36f8d841" />

SSH Session Closed
<img width="1024" height="768" alt="15 9SSH_Session_Closed" src="https://github.com/user-attachments/assets/c5b22f7e-8380-41f1-93a4-50ce28003ee5" />

## What I Learned
- How SSH provide secure remote access to Linux systems
- How to instakk and configure OpenSSH Server on Ubuntu
- How to verify that a service is running using systemctk
- How to verify a service listening on a network port
- How TCP port 22 is used for SSH communications
- How to establish a remote connection from Windows to Linux
- How to execute Linux commands remotely through an SSH session
- The importance of network connectivity when troubleshooting remote access issues





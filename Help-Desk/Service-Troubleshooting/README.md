# Service Troubleshooting

## Objective
Practice and investigating and troubleshooting Windows services using both GUI and command line.

## Tools Used
- Windows 11
- Virtual Box
- Services.msc
- Command Prompt

## Tasks Performed
- Opened Services console
- Investigated common Windows services
- Stopped and restarted Print Spooler
- Verified service status using the Command Prompt
- Started sercives usinf command line (administrative)
- Verified the service was running using service.msc

## Commands Used
### cmd
sc query spooler
net start spooler

## Screenshots

Service Controls
<img width="1024" height="768" alt="5 1Services_Homw" src="https://github.com/user-attachments/assets/6ee75011-cddf-4574-aadb-e7bd82f61856" />

Print Spooler Services
<img width="1024" height="768" alt="5 2Print_Spooler_Services" src="https://github.com/user-attachments/assets/5d97614b-8a72-4f0e-bc07-7abb2092b939" />

 Print Spooler Stopped
 <img width="1024" height="768" alt="5 3Print_Spooler_Stopped" src="https://github.com/user-attachments/assets/36a10691-c80a-4e6e-8b99-0e86642bec03" />

 Command Line Verification
 <img width="1024" height="768" alt="5 4Verification_Spooler_Stopped" src="https://github.com/user-attachments/assets/b29fd480-574a-4f4c-aad4-35426b3245ed" />

Print Spooler Started in Command Prompt (administrative)
<img width="1024" height="768" alt="5 5Print_Spooler_Started_CMd" src="https://github.com/user-attachments/assets/5ba2bac9-c089-4ada-821e-0027a3889ca9" />

Verification Spooler Started in services.msc
<img width="1024" height="768" alt="5 6Verification_Spooler_Started" src="https://github.com/user-attachments/assets/eb6136f8-66f5-4d72-8b9b-471406c80f70" />

Service Dependencies
<img width="1024" height="768" alt="5 7Dependencies" src="https://github.com/user-attachments/assets/a08e4cd7-8e3a-46ad-b791-2a4bebff579c" />


## What did I learn
- How Windows services suppoert system functionality
- Difference between Automatic, Manual and Disable startu types
- How to stop and restart services
- How to verify service status using Command Prompt
- How service failures can impact applications and devices
- Importance of the Print Spooler service in printer functionality



 

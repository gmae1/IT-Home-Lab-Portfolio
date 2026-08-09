# Corporate Logon Banner Deployment with Group Policy Lab

## Objective
Create and deploy an enterprise Group Policy Object that displays a standardized corporate security notice before users sign in to domain managed Windows workstations.

The policy was linked specifically wo the Workstation Organizational Unit, allowing centralized configuration of all managed Windows 11 computers without manually configuring each device.

## Why This Lab Maaters
Group Policy is one of the primary tools Windows administrators use to centrally configure and secure computers in an Active Directory environ.

Instead of manually configuring individual workstations, administrators can create a policy once and automatically deploy it to hundreds or thousands of computers.

A corporate logon banner can be used to:
- Notify users that systems are company property
- Warn against unauthorized access
- Inform users that activity may be monitored
- Standardize security messaging across managed endpoint
- Demonstrate centralized workstation management

This lab demonstrates the fundamental relationship between Active Directory OUs and Group Policy Object

## Skills Demonstrated 
- Group Policy Management Console (GPMC)
- Group Policy Object creation
- GPO linking
- Organizational Unit targeting
- Computer Configuration policies
- Windows Security Options
- Centralized endpoint administration
- gpudate
- Group Policy troublshooting
- Policy Validation

 ## Task Performed
 1. Identified Target Organizational Unit
 2. Using Group Policy Management to create a "Corporate Logon Banner" and this GPO was directly linked to the "Workstation" OU
 3. Configured the Security Notice
 4. Forced Group Policy Refresh
 5. Validated the Security Banner

## Screenshots

GPO Management
<img width="1024" height="768" alt="12 1GPOManagement" src="https://github.com/user-attachments/assets/f4938baa-b1de-4f24-9ad1-ab57e68b086c" />

Creating New GPO
<img width="1024" height="768" alt="12 2NewGPO" src="https://github.com/user-attachments/assets/c801889f-5eaf-4cf7-b988-6fe672b2d51c" />

GPO Editor
<img width="1024" height="768" alt="12 3GPOEditor" src="https://github.com/user-attachments/assets/7d1c81ea-6310-4229-8cbc-d7fde34e456c" />

Select Specific GPO
<img width="1024" height="768" alt="12 4SelectedGPO" src="https://github.com/user-attachments/assets/9cbb4c0d-ae28-41fc-82b4-f5854ead7dd3" />

Creating Company Message
<img width="1024" height="768" alt="12 5Message" src="https://github.com/user-attachments/assets/8203eb58-6ff8-4482-8e46-9b83af4a974a" />

Selecting Second GPO
<img width="1024" height="768" alt="12 5SecondGPO" src="https://github.com/user-attachments/assets/3f11ae7c-058e-4222-bb14-767d5b421b9b" />

Creating Second Company Message
<img width="1024" height="768" alt="12 6Message" src="https://github.com/user-attachments/assets/5a5c2964-6af7-4429-b630-504ff3f2cb70" />

Force Update
<img width="1024" height="768" alt="12 7ForceUpdate" src="https://github.com/user-attachments/assets/f8dda9a9-f059-4c9e-83c4-f217ac267da5" />

Verifying Update on Windows Workstation
<img width="1024" height="768" alt="12 8VerifyUpdate" src="https://github.com/user-attachments/assets/556248cc-7375-4a41-a55c-cb98c4619e75" />

## Conclusion 
This lab demonstrated the deployment of a centralized Windows workstation configuration using Active Directory Group Policy

A Corporate Logon Banner GPO was created, configured and linked specifically to the Workstation OU, Client site validation confirmed that domain joined Windows 11 systems successful received and enforced the security policy

The lab established the foundation for more advanced enterprise Group Policy administration, including security restrictions, password policies, Windows configuration management, policy filtering, and GPO troubleshooting.

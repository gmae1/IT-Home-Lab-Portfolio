# Windows Serrver Backup Disaster Recovery Lab

## Objective
Deploy and configure Windows Server Backup on a Windows Server 2022 Domain Controller, create a dedicated backup storage volume, perform a manual backup of company data, simulate accidental data loss, and successfully restore deleted files using the Windows Server Backup recovery wizard.

## Why This Lab Matters
Data loss can occurr due to accidental deletion, hardware failure, ransomware, or system corruption. Winddows Server Backup provides administrators with a built-in disaster recovery solution that protects critcal business data and enables rapid recovery with minimal downtime. 
This lab demonstrates practical Windows Server administration by configuring backup storage, creating backups, and restoring deleted data, which are common responsibilities for System Administrators and Windows Server Administrators.

## Task Performed 
- Installed the Windows Server Backup feature through Server Manager
- Created a folder (C: \CompanyData) with department folders
- Added a second 20 GB virutal hard disk to the Windwos Server virutal Machine
- Initialized a new disk using GPT in Disk Management
- Created and formated a new NTFS volumed labeled Backups (E:)
- Performed a manual Windows Server Backup of CompanyData folder to the dedicated backup volume
- Verified that Windows Server Backup Successfully created the backup repo
- Simulated data loss by purpossly deleting HR
- Verified that the recovered Folderand Contents inside were successfully Restored

## Screenshots

Windows Bakup Selected/Installed
<img width="1024" height="768" alt="3 1Windows_Backups" src="https://github.com/user-attachments/assets/ec51a153-7a8b-48dc-a096-3292e3ebc114" />
<img width="1024" height="768" alt="3 2WBU_Installed" src="https://github.com/user-attachments/assets/6ccb3ff2-104c-4f44-9612-f20a84cabe73" />

Created Company Folder
<img width="1024" height="768" alt="3 3ComapnyData_Folder" src="https://github.com/user-attachments/assets/24780d2d-75d2-4484-9c6d-8f8753cb4a97" />
<img width="1024" height="768" alt="3 4HR_emplyoees" src="https://github.com/user-attachments/assets/6bda1d0e-fd39-49ac-8592-f264812b03a4" />
<img width="1024" height="768" alt="3 5Sales_Goal" src="https://github.com/user-attachments/assets/9ab97f19-95ca-4ecc-a63c-89ae7e5e505b" />
<img width="1024" height="768" alt="3 6Engineering_Projects" src="https://github.com/user-attachments/assets/2a5f872e-1cf8-4854-8719-e8c119653a47" />

Adding a New Hard Disk To Virtual Machine
<img width="772" height="521" alt="3 9Add_HardDisk" src="https://github.com/user-attachments/assets/15d78670-520f-41c3-a002-8800ccf4a4b6" />
<img width="767" height="513" alt="3 10New_HardDisk" src="https://github.com/user-attachments/assets/1c73fd57-ab42-40f1-a540-496c50cf9380" />

Allocating New Disk/Disk Configuration
<img width="1024" height="768" alt="3 11Allocating_Disk" src="https://github.com/user-attachments/assets/bff45c67-b555-49fc-8065-ee90853bbc65" />
<img width="1024" height="768" alt="3 12Disk_Config" src="https://github.com/user-attachments/assets/de7ad4c0-0f94-410e-9f7c-ca1ab3354857" />

Adding Items To Be Bsckedup 
<img width="1024" height="768" alt="3 13Adding_Items" src="https://github.com/user-attachments/assets/0baacd9c-7bf2-4700-855a-cb7f345eda6e" />

Selecting Backup Destination
<img width="1024" height="768" alt="3 14Backup_Destination" src="https://github.com/user-attachments/assets/32f99f1a-e258-4921-9338-cdd23fa93a6c" />

Delting HR
<img width="1024" height="768" alt="3 15HR_Deleted" src="https://github.com/user-attachments/assets/c6984cd6-d61d-476f-b9b5-99e534ee1a04" />

Recovering Lost Data In Wizard
<img width="1024" height="768" alt="3 16Recover_Lost_Data" src="https://github.com/user-attachments/assets/439f7034-fbb1-4848-aea2-8d1f5e43a194" />

HR Recovered
<img width="1024" height="768" alt="3 17HR__Recovered" src="https://github.com/user-attachments/assets/37dd8ee3-68bd-45c1-b38c-df2b77e37443" />

## Conclusion 
This lab demonstrated how Windows Server Backup can be used to protect and recover business-critical data. A dedicated backup volume was configured using a seperate virtual disk, allowing backups to remain isolated from the operating system drive. Afrer simulating accidental deletion of a department folder, the recovery process successfully restored the lost data. This exercise reinforced enterprise backup beest practices, storage management, and disaster recovery procedures commonly performed by Windows SErver administrators.

# Resource and User Data Managemnet Lab

## Objective
Implemented centralized user resource management using Folder Redirection to store user documents on the server instead of locally on workstations.

## Why This Lab Matters
Folder Redirection allows organizations to centeralize user data, simplify backups, and provide seamless access to file across multiple computers

## Task Performed
- Created UserDocs Folder
- Shared Folder
- Configured Permissions (Share Permissions & NTFS Permissions)
- Created New GPO (Folder Redirection)
- Configured Folder Redirection
- Updated/Applied Group Policy
- Verified Redirection

## Screenshots

Created Folder
<img width="1024" height="768" alt="13 1Created_New_Folder" src="https://github.com/user-attachments/assets/85529fb6-5ff2-4640-815b-147b547044c4" />

Assigned Permissions (NTFS)
<img width="1024" height="768" alt="13 2Assign_Permissions" src="https://github.com/user-attachments/assets/a5977aac-d4af-45cd-ac78-ce4bce4cd7c1" />

Assigned Permissions (Shared)
<img width="1024" height="768" alt="13 3Sharing_Permissions" src="https://github.com/user-attachments/assets/bf8f52a5-88a1-483e-a9ba-c6b998b6b476" />

Created New GPO
<img width="1024" height="768" alt="13 4New_GPO" src="https://github.com/user-attachments/assets/30cb8f79-7b3b-4023-b432-6bf7bfd91e39" />

Redirection Folder Setting
<img width="1024" height="768" alt="13 5Target_Folder" src="https://github.com/user-attachments/assets/a1a301e7-909a-4872-b499-be355e63323b" />

Update/Applied Group Policy
<img width="1024" height="768" alt="13 6Update" src="https://github.com/user-attachments/assets/843a293f-6cd7-4403-8dfb-30b92d19376c" />

Folder Access (From John Adams)
<img width="1024" height="768" alt="13 7Folder_Accessible" src="https://github.com/user-attachments/assets/57d52904-63e2-44e6-aeb8-aae1a9c96a2a" />

Create Doccument from Client Machine
<img width="1024" height="768" alt="13 8Creating_Doc_From_JA" src="https://github.com/user-attachments/assets/dd23b13a-ca6c-41e7-bfb2-aa5da690bf4a" />

Verified Doccument from Server
<img width="1024" height="768" alt="13 9Verified_Of_Text_Doc" src="https://github.com/user-attachments/assets/342cd803-14b4-42ed-be73-5f2ddf42465d" />

## Conclusioin
Implemented Folder Redirection using Active Directory Group Policy and SMB shares to centralize user document storage, enabling seamless access to files across multiple workstations and improving data resiliency.

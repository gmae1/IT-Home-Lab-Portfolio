# File Shares and NTFS Permissions

## Objective
Implement departmentr file shares and configure NTFS permissions using Active Directory security groups top provide secure access to shared resources.

## Why This Lab Matters
Organizations rely on file servers to store depatmental data securely. Access should be granted based on group membership rather than assiging permissions directly to individual users.
This lab demonstrates the principlle of least privlege and centralized access management

## Task Performed
- Created Department Folders
- Configured SMB Shared Permissions
- Configured NTFS PermissionsVerified Group Membership
- Tested Access

## Screenshots

Creat Folders
<img width="1024" height="768" alt="6 1Create_Folder" src="https://github.com/user-attachments/assets/ea3d9531-2cc3-46ca-b5ee-51c95266937f" />

Department Folders
<img width="1024" height="768" alt="6 2Folders_Inside_Shares" src="https://github.com/user-attachments/assets/49b7e26d-62a1-4261-a805-c8a7655c974b" />

Assigning Sharing Permissions
<img width="1024" height="768" alt="6 3Sharing_Permissions" src="https://github.com/user-attachments/assets/71c390f5-c7bb-4e97-a8ff-4a16f8855039" />

Shares Verification
<img width="1024" height="768" alt="6 4Shares_Verification" src="https://github.com/user-attachments/assets/3fc4dc6c-4890-4aa1-a7ec-91a2d717088f" />

Group Verification
<img width="1024" height="768" alt="6 5Group_Verification" src="https://github.com/user-attachments/assets/4655ece3-c9a6-4c74-b5a2-cee029275ed3" />

Advanced Security Sharing
<img width="1024" height="768" alt="7 1Disable_Inheritance" src="https://github.com/user-attachments/assets/b8ab0d7e-9a19-4f10-8576-71d0e9ac09fa" />

Disabling Inheritance
<img width="1024" height="768" alt="7 1Disable_Inheritance" src="https://github.com/user-attachments/assets/ba8df869-5f16-4d36-9978-c4d109f9ac69" />

Removing Unassociated Users
<img width="1024" height="768" alt="7 2Removing_Users" src="https://github.com/user-attachments/assets/ca1c3bf4-7e5b-4133-9578-29b7e2d26081" />

Adding Group Users
<img width="1024" height="768" alt="7 3Adding_Users" src="https://github.com/user-attachments/assets/6b5aa668-dbdb-44e2-a1b3-6e0185513df8" />

User Unable To Access Folder Outside Of Their Group
<img width="1024" height="768" alt="7 4Unable_Access_Folder" src="https://github.com/user-attachments/assets/a60a658b-d07a-418e-a519-2a4bb2852c92" />

User Able TO Access Folder In Their Group
<img width="1024" height="768" alt="7 5Able_To_Access_Folder" src="https://github.com/user-attachments/assets/48b305cf-ec36-4304-92df-c3fd4a582d5c" />

## Conclusion
Implemented centralized file sharing using SMB and NTFS permissions in a Windows Server enviornment, leveraging Active Directory security groups to enforce least privilege access and departmental resource separation.

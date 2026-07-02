# DFS NameSpace Enterptise File Sharing Lab

## Objective
Deploy and configure a Distributed File System (DFS) Namespace in a Windows Server 2022 Active Directory enviornment. Create a centralized namespace that provides users with a single network path to departmental shared folders while abstracting the physical file server location.

## Why This Lab Matters
Enterprise enviornments often contain multiple file servers that host departmental data. Without DFS users must remember the server hosting each shared folder, making server migration and infrastructure upgrades disruptive.
DFS Namespace provides a single consistent network path for users while allowing administrators move data between servers without changing users access paths. This helps simplifies file management, improves scalability, and preparest the enviornment for high availability through DFS Replication.

## Steps Performed

- Installed DFS Namespaces and DFS Replication role services.
- Created a centeralized departmental folder structure
- Shared the Company Data folder over the network
- Verified network accessibility using the UNC path
- Created a Domin-Based DFS Namespace
- Configured the namespace root
- Added departments to DFS folder
    - HR
    - Sale
    - Engineering
- Configured folder targets to point to the appropriate shared folders
- Verified successful access throguh the DFS Namespcace
- Validated the user can access departmental resources using a single namespace path rather then individual server shares

## Screenshots

Selected/Installed DFS Features
<img width="1024" height="768" alt="4 1Selected_DFS" src="https://github.com/user-attachments/assets/74ebedfe-a21d-48fc-8ae2-7f7f1881d129" />
<img width="1024" height="768" alt="4 2NFS_Installed" src="https://github.com/user-attachments/assets/d4d6d7db-7909-4332-8c6d-a1daf37adfa6" />

DFS Wizard
<img width="1024" height="768" alt="4 3DFS_Management" src="https://github.com/user-attachments/assets/39e4604c-cb53-433c-9ab0-e51d72d65dac" />

Company Data/Departments
<img width="1024" height="768" alt="4 4CompanyData(1)" src="https://github.com/user-attachments/assets/41d87ce7-5681-4b95-9e75-f41f0bbeaa33" />
<img width="1024" height="768" alt="4 4CompanyData" src="https://github.com/user-attachments/assets/8d205824-7ab1-4b95-946e-342c7989bbc5" />

Shared Company Folder
<img width="1024" height="768" alt="4 5Sharing_Folder" src="https://github.com/user-attachments/assets/3dd9f9b0-4c89-4134-b8c0-db3c7d67f228" />

NameSpace Server 
<img width="1024" height="768" alt="4 6NameSpace_Server" src="https://github.com/user-attachments/assets/e649800c-42a2-4563-97d2-8af71df6f847" />

NameSpace Name
<img width="1024" height="768" alt="4 7NameSpace_Name" src="https://github.com/user-attachments/assets/9ff88087-4e3a-489a-ba03-ed51d3926dc4" />

NameSpace Type
<img width="1024" height="768" alt="4 8NameSpace_Type" src="https://github.com/user-attachments/assets/53c1fdcd-a54b-4f1a-8cb7-07f938876ebf" />

NameSpace Confirmation
<img width="1024" height="768" alt="4 9Confirmation" src="https://github.com/user-attachments/assets/419dca79-9cd1-4024-a9ae-5542bf52c2c0" />

Creating Folder in New NameSpace
<img width="1024" height="768" alt="4 10Creating_NewFolder" src="https://github.com/user-attachments/assets/e733fa04-e53d-4a10-8d94-f8754fe86f40" />

All Folders Created
<img width="1024" height="768" alt="4 11Created_All_Folders" src="https://github.com/user-attachments/assets/65cef563-ff86-4b34-9083-db58237cc8b1" />

Access From Windows Pro Machine
<img width="1024" height="768" alt="4 12Access_From_WindowsPro" src="https://github.com/user-attachments/assets/3fb5817e-5758-43a7-b686-30f81136a6ee" />

## Conclusion
This lab demonstrated how DFS Namespace centralizes enterprise file sharing by providing users with a consistent network path independent of the physical server.

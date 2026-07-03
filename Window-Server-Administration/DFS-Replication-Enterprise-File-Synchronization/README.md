# DFS Replication Enterprise File Synchronization Lab

## Objective 
Configured DFS Replication between two Windows Server 2022 domain controllers (DC1 & DC2) to automatically synchronize company shared folders across multiple severs, providing redundency and improving enterprise file availability

## Why This Lab Matters
Enterprise organizations rely on DFS Replication to ensure important departmental files remain synchronized across multiple servers. If one file server becomes unavailable, another server maintains an up-to-date copy of the data, reducing downtime and improving busineess continuity
This lab demonstrates how Windows Server replicates shared data automatically between domain controllers while working alongside DFS Namespace to provide users with seamless access to company resources.

## Task Performed
- Installed DFS Replication role services on both domain controllers
- Verified communication between DC1 and DC2 using ping and nslookup
- Created a Multipurpose Replication Gruop
- Added DC1 and DC2 as replication members
- Selcted a Fulll Mesh Topology
- Configured DC1 as the Primary Member
- Selected C:\CompanyData as the replicated folder
- Configured C:\CompanyData on DC2 as the replication destiniation
- Completed the replication wizard
- Created a test file within the HR folder
- Verified automatic replication from DC1 and DC2

## Screenshots

Adding DFS Replication to DC2
<img width="1024" height="768" alt="5 1Adding_DFS_Rep" src="https://github.com/user-attachments/assets/872c1f9c-85d4-4859-a2ed-97fed486837d" />

Replicaiton Wizard
<img width="1024" height="768" alt="5 2Replication_Wizard" src="https://github.com/user-attachments/assets/412cb4b3-a1df-4fac-8624-011b282fb812" />

Name and Domain
<img width="1024" height="768" alt="5 3Name_Domain" src="https://github.com/user-attachments/assets/659021cf-486b-455b-b2a0-174b9a9f4ab0" />

Adding Replication Group Members
<img width="1024" height="768" alt="5 4Adding_Replication_Hroups" src="https://github.com/user-attachments/assets/75dad80a-88ef-45d4-808a-56c13694e53d" />

Selecting Topolgies
<img width="1024" height="768" alt="5 5Topology" src="https://github.com/user-attachments/assets/be60efe3-8e68-448d-999d-47bbea0d47de" />

Selecting Primary Member
<img width="1024" height="768" alt="5 6Primary_member" src="https://github.com/user-attachments/assets/b5cbac7d-3a5b-4fcb-abfc-758015fb5222" />

Adding Folder To Replicate
<img width="1024" height="768" alt="5 7Adding_Folder_To_Replicate" src="https://github.com/user-attachments/assets/05052577-9d7c-47ab-b469-2c788193d391" />

Verified Replication Role On DC1 And DC2
<img width="1024" height="768" alt="5 8Replication_On_DC2" src="https://github.com/user-attachments/assets/9d074b70-9cd9-4dcc-aa00-d6fc00385a12" />
<img width="1024" height="768" alt="5 9Replication_On_DC1" src="https://github.com/user-attachments/assets/e31d9a8f-ca76-487b-b3be-b51f89463141" />

Creating a test txt in HR Folder on DC1
<img width="1024" height="768" alt="5 10Create_Text_On_DC1" src="https://github.com/user-attachments/assets/1d23cef6-d641-487c-be80-1718d9bdc72b" />

Verified Text on DC2
<img width="1024" height="768" alt="5 11Text_Created_On_DC2" src="https://github.com/user-attachments/assets/1ee59424-806e-4eae-82f7-be2ba93fe343" />


## Conclusion
The Lab Successfully implemented DFS Replication between two Windows Server 2022 Domain Controllers. Department Data stored within CompanyData Directory is automatically synchronized between DC1 and DC2, providing redundency and ensuring file conssistency across the enterprise enviornment. Combined with the previous lab DFS Namespace, users can access shared folders and resourcfes throuhg a single network path while administrators benifit from improved resiliency and simplified file management.

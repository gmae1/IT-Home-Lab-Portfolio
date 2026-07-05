# File Server Resource Manager FSRM Storage Management Lab

## Objective
Deploy and configure File Server Resource Manager (FSRM) on Windows SErver 2022 to manage enterprise file storage by implementing storage quotes, file screening policies, and storage utilization reports.

## Why This Lab Matters
Organizations rely on File Server Resource Manager (FSRM) to enforce storage polocies, prevent unauthorized file types from being stored on file servers, and monitor storage consumption across departments. Proper storage management helps maintain file server performance, supports capacitty planning, and prevents users from consuming excessive storage resources.

## Task Performed
- Installed File Server Resource Manager (FSRM)
- Created a Hard Quota on HR Department Folder
- Configured a 100 MB storage limit for the HR folder
- Created a 150 MB test file using fsutil
- Verified  the FSRM prevented files exceeding the quota from being stored
- Confirmed that folders without quotas were unaffected
- Configured File Screen to block selected audio and cideo file types within the CompanyData folder
- Created a Storage Report Task for the CompanyData File
- Generated storage reports to analyze file usage, duplicate files, file groups, and storage utilizaion

## Scrrenshots

File Server Resource Manager Role Added
<img width="1024" height="768" alt="6 1FileServerResource_Add" src="https://github.com/user-attachments/assets/59ae0bd9-0bad-4198-b8b9-b939d55f4f31" />
<img width="1024" height="768" alt="6 2File_Server_Resources" src="https://github.com/user-attachments/assets/49c38681-d3bb-4623-9eb5-cf14e864cef5" />

Creating Quota
<img width="1024" height="768" alt="6 3Creating_Quota" src="https://github.com/user-attachments/assets/7c938d72-4440-4db6-8793-bb15834e3080" />

Test File 
<img width="1024" height="768" alt="6 4 Create_A_Test_Filer" src="https://github.com/user-attachments/assets/3024e227-46c1-41e9-9482-13ad5f71fc02" />
<img width="1024" height="768" alt="6 5Test_File" src="https://github.com/user-attachments/assets/35f44e84-38c0-4696-bc6d-5499cbf4c677" />

Test File Too Large For HR Folder
<img width="1024" height="768" alt="6 6Item_Too_Large" src="https://github.com/user-attachments/assets/c2570c35-ad77-4e3c-b2b3-5f0ba6aaa235" />

Creating File Screening
<img width="1024" height="768" alt="6 7Creating_File_Screening" src="https://github.com/user-attachments/assets/3f821e76-67a2-4074-a972-7c75235b437b" />
<img width="1024" height="768" alt="6 8Path_For_FileScreening" src="https://github.com/user-attachments/assets/9ef89fef-31f8-4c75-910b-c2b212222dbf" />

Downlodaded MP3 File
<img width="1024" height="768" alt="6 9MP3_Sound" src="https://github.com/user-attachments/assets/f4c26baa-57a7-417c-a311-e30fb3941c97" />

MP3 Denied
<img width="1024" height="768" alt="6 10MP3_Denied" src="https://github.com/user-attachments/assets/bd45782b-2bdf-45e5-8ddb-cb3c44c91459" />

Created Storage Report Task
<img width="1024" height="768" alt="6 11Storage_Reports" src="https://github.com/user-attachments/assets/a0f2a065-7d92-4725-b4b1-58d30155854b" />
<img width="1024" height="768" alt="6 12Storage_Reports_Scope" src="https://github.com/user-attachments/assets/01ddc24e-87a6-46c5-b0b4-bdf14da1cdc0" />

## Conclusion
This lab demonstrated how Windows Server File Server Reource Manager (FSRM) can be used to enforce enterprise storage policies. Storage quotas were implemented to prevent departments from exceeding allocated disk space, file screening policies were configured to block unauthorized file types, and storage reports were generated to provide administrators with insight into storage utilization and file management. These capabilities help organizations maintain efficent, secure, and well-managed file server environments.

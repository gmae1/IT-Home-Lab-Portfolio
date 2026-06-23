# Powershell Active Directory Administration

## Objective
Use Powershell to query, create, abd bulk create Active Directory users, including importing users from a CSV file and placing them into department-specific OUs

## Why This Lab Matters
PowerShell allows administrators to mange Active Directory at scale, Instead of manually creating users through ADUC, administrators can automate repetitve account-management tasks and reduce manual errors

## Task Performed
- Filtered Users in Current Server
- Research Information of a Specific User
- Researched more Information of that Same User
- Used different commands to check Names, Active Users, Disabled Accounts, Locked Out Accounts, and Expired Accounts
- Created A Varriable so that all New users will obtain the same Password from first Logon
- Created One New User
- Verified The New User
- Added the User to the It Department
- Disabled New User (Then Re-enabled User)
- Reset New Users Password
- Created Bulk Users in Notepad using CSV
- Verified all Imported Users through the Powershell
- Created all New Users Bulked together with One command String
- Verified New Users

## Screenshots

GetADUser -Filter *
<img width="1024" height="768" alt="15 1PWS_command" src="https://github.com/user-attachments/assets/fe4c2950-5685-43c0-b3b1-837bd1972c9a" />

John Adms Information
<img width="1024" height="768" alt="15 2JA_Information" src="https://github.com/user-attachments/assets/a63a9a07-ce1e-4d19-9acc-56649208ae5d" />

More of John Adams Information
<img width="1024" height="768" alt="15 3JA_More_Info" src="https://github.com/user-attachments/assets/f8009986-52fd-4ebb-9d67-977074afb7c2" />

Select Name
<img width="1024" height="768" alt="15 4Select_Name" src="https://github.com/user-attachments/assets/198cce2a-dcdb-419f-864c-5945adf56f6d" />

Active Users
<img width="1024" height="768" alt="15 5Active_Users" src="https://github.com/user-attachments/assets/dda5961c-2080-4067-99f1-3b184d5fb2db" />

Accounts Disabled
<img width="1024" height="768" alt="15 6Account_Disabled" src="https://github.com/user-attachments/assets/ebd245ef-2e03-408c-8c1d-99f062551cc7" />

Locked Out Users (None)
<img width="1024" height="768" alt="15 7LockedOut_User" src="https://github.com/user-attachments/assets/9b6b9d43-bb34-45fc-bd87-b119a926ada8" />

Accounts Expired (None)
<img width="1024" height="768" alt="15 8Account_Expired" src="https://github.com/user-attachments/assets/c3f9b855-c20c-45af-a564-9bb5826cd383" />

Password Varriable
<img width="1024" height="768" alt="15 9Create_Varriable" src="https://github.com/user-attachments/assets/7f94e264-4807-4c9e-a7ec-388974339f1d" />

Creating New User
<img width="1024" height="768" alt="15 10Creating_new_User" src="https://github.com/user-attachments/assets/a61e92b1-03cc-40e8-b053-3ab156dc491c" />

Verify New User
<img width="1024" height="768" alt="15 11Verify_New_User" src="https://github.com/user-attachments/assets/602fc345-b92f-4423-aa98-2fd1fadc3f3e" />

Add New User To IT Department
<img width="1024" height="768" alt="15 12Add_User_To_IT_Admin" src="https://github.com/user-attachments/assets/37dd1668-48f2-45a4-9e3f-ecc6cf1b01ee" />

Verified User in Department
<img width="1024" height="768" alt="15 13Verify_Add_User" src="https://github.com/user-attachments/assets/04b085cf-5200-4fe6-9de6-5e498b79f356" />

Disable New User
<img width="1024" height="768" alt="15 14Disable_User" src="https://github.com/user-attachments/assets/9a665c06-b245-4ac9-851a-502f39e95303" />

Verified Disabled Accounts
<img width="1024" height="768" alt="15 15Verify_Disabled_Account" src="https://github.com/user-attachments/assets/3db2fcf7-3a85-4c06-952a-901e299a61aa" />

Reset New Users Password
<img width="1024" height="768" alt="15 16Reset_Password" src="https://github.com/user-attachments/assets/f4451b29-913a-4b52-8e0b-bd5882d3e7b1" />

Creating Bulk Users in Notepad with CSV
<img width="1024" height="768" alt="15 7Bulk_Users" src="https://github.com/user-attachments/assets/81864fd7-0605-4a04-8fef-0551187dfe1a" />

Importing New Users on Powershell
<img width="1024" height="768" alt="15 17Importing_New_Users" src="https://github.com/user-attachments/assets/b971db2e-7310-4f8b-9769-dc7784829651" />

Bulk String To Create all New Users
<img width="1024" height="768" alt="15 18Creating_New_Users" src="https://github.com/user-attachments/assets/be5fedcd-961f-42e0-97a0-0da51dabccf9" />

Verified New Users
<img width="1024" height="768" alt="15 19Verified_New_Users" src="https://github.com/user-attachments/assets/c5616523-8e81-4f30-9763-e78c4739d29a" />

## Conclusion
Automated Active Directory user management with Powershell by querying directory objects, creatinf individual users, and bulk-importing accounts from CSV files into departmet specific OUs

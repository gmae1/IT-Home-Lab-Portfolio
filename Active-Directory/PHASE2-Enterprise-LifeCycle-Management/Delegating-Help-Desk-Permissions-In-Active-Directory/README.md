# Delegating Help Desk Permissions in Active Directory Lab

## Objective
Implement delegated administration in Active Directory by creating a Help Desk role with limited administrative privileges. Configure delegated permissions that allow Help Desk technicians to reset passowrds and unlock user accounts wwhile preventing access to higher privleged administrative task.

## Why This Matters
In enterprise environments, Help Desk technicians should not be members of Domain Admins group. Instead, organizations use delegated administration to grant only the permissions required to perform daily support task. This approach reduces security risks, limits the impact of compromised accounts, and folllows the Principle of Least Privilege.

This lab demonstrates how to securly delegate administrative reponsibilities while validating that unauthorized actions remain restriceted.

## Steps Performed
- Create a Help Desk OU and security Groups
- Created Help Desk technician account (Alex Morgan)
- Added the technician account to the GG-HelpDesk security Groups
- Delegateed password reset and account unlock permissions.
- Added RSAT(Remote Server Administration Tools) to PC-002 from Administrative Account
- Logged into Help Desk account (Alex Morgan)
- Verified delegated task using Active Directory Users and Computers
- Confirmed restricted administrative access
- Documented the change through a servuce desk ticket

## Screenshots
New OU (Organizational Unit)
<img width="1024" height="768" alt="11 1NewOU" src="https://github.com/user-attachments/assets/08743b37-5719-4c8a-900f-6cab0f1d7f10" />

New GG (Global Group)
<img width="1024" height="768" alt="11 2NewGG" src="https://github.com/user-attachments/assets/a80b703a-8f53-40ac-8236-8e803ee2ef9d" />

Created New User 
<img width="1024" height="768" alt="11 3CreatingNewUser" src="https://github.com/user-attachments/assets/779ec5ee-de18-469d-b479-dffacac0a837" />

Adding New User To GG
<img width="1024" height="768" alt="11 4AddingUserToGG" src="https://github.com/user-attachments/assets/ecfe8e64-ed25-4e39-a0e5-d5a7deec6901" />

Added GG-HelpDesk To Delegated Controls
<img width="1024" height="768" alt="11 5DelegatedControls" src="https://github.com/user-attachments/assets/aadb612c-ba83-4fce-9e9d-9d91400c2f5b" />

Selected Delegation Task for Help Desk
<img width="1024" height="768" alt="11 6DelegationTask" src="https://github.com/user-attachments/assets/7ab8f857-811f-4619-9442-2924ff1dc035" />

Added RSAT From Admin Account
<img width="1024" height="768" alt="11 7AddingRSATFromAdmin" src="https://github.com/user-attachments/assets/a1606d59-bde8-4881-917d-5168604f0146" />

Logged into Help Desk Account (Alex Morgan)
<img width="1024" height="768" alt="11 8LoginAMorgan" src="https://github.com/user-attachments/assets/0042a160-d4be-45c9-b871-cca600ccb8c0" />

Opened ADUC from Help Desk Account
<img width="1024" height="768" alt="11 9ADUC" src="https://github.com/user-attachments/assets/cbd8572c-1f02-430f-91e1-38e1004bbcfe" />

Reset Users Password from Help Desk Account
<img width="1024" height="768" alt="11 10ResetUserPass" src="https://github.com/user-attachments/assets/38fb70a8-d02c-43de-a5f7-f3137728ee00" />
<img width="1024" height="768" alt="11 11UserPasswordChanged" src="https://github.com/user-attachments/assets/522ac1ec-a027-4265-8147-974ee32c3e68" />

Denied permissions to Delete Account
<img width="1024" height="768" alt="11 12DeniedToDelete" src="https://github.com/user-attachments/assets/90c9c2d1-bd37-4b9e-a04a-e9d198812109" />

## Conclusion
This lab deomonstrated how enterprise enviironments implement delegated adminisration within Active directory, Rather than gathering excessive privileges, Help Desk technicians received only the permissions required to perform their daily responsibilities. Validation testing confirmed that approved administratice actions succeeded while unauthorized actions were appropriately denied, reinforcing secure identity and access management practices.

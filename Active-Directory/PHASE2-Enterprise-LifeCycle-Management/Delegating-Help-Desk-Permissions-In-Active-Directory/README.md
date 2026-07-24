# Delegating Help Desk Permissions in Active Directory Lab

## Objective
Implement delegated administration in Active Directory by creating a Help Desk role with limited permissions for password restes and account unlcoks.

## Why This Matters
Enterprise IT teams rarely grant full administrative rights to Help Desk staff. delegated administration improves security by allowing technicians to perform routine support tasks without exposing the entire Active Directory environment

## Steps Performed
- Create a Help Desk OU and security Groups
- Created Help Desk technician account
- Delegateed password reset and account unlock permissions.
- Added RSAT(Remote Server Administration Tools) to PC-002
- Verified delegated task
- Confirmed restricted administrative access
- Documented the change thriugh a servuce desk ticket

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


## Conclusion
This lab demonstrarted a core enterprise security practice, delegated admiistration. By granting only the permissions required for Help Desk responsibilities, the environment now better reflects a production Active Directory deployment while reinforcing the Principle of Least Privilege

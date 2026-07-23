# Create Administrative Accounts Lab

## Objective
Implement the Principle of Least Privilege by creating a dedicated administrative account, organizing privleged indentity, and assigning administrative access through security groups

## Why this lab matters
Enterprise organizations reduce security risk by separating standard user identites from privileged administrator accounts. This practice limits the exposure of elevated credentials and supports stronger access control.

## Steps Performed 
- Created a global Security Group "GG-IT-Admins" for privlaged IT staff.
- Created a dedicated adminstrative account (adm-mdavis) in the Admin Accounts OU
- Populated business properties and labeled the account as a privileged identity.

- Added the account to GG-IT-Admins
- Added the account to Domain Admins for lab purposes
- Verified group memberships and aadministrative logon funstionality.

## Screenshots

Creating New Group
<img width="1024" height="768" alt="5 1CreatingNewGroup" src="https://github.com/user-attachments/assets/e7fd03ab-2bd0-4005-a042-a2bab488e79a" />

Creating New Admin user
<img width="1024" height="768" alt="5 2CreatingNEwAdminUser" src="https://github.com/user-attachments/assets/e34e516c-6d3d-4870-b15b-13c2b6a59af3" />

Admin Properties
<img width="1024" height="768" alt="5 3AdminProps" src="https://github.com/user-attachments/assets/e6292063-ef7d-4c26-b377-9223458c7335" />

Admin Organization Properties
<img width="1024" height="768" alt="5 4AdminOrgProp" src="https://github.com/user-attachments/assets/a4de7557-399a-4f8d-a867-0659f50c8e28" />

Adding User To Global Group
<img width="1024" height="768" alt="5 5AddingUserToGG" src="https://github.com/user-attachments/assets/8f2ff01d-f26b-4095-8826-5da626cafb5d" />

Addming Mdavis to Domain Admins (Lab Purposes)
<img width="1024" height="768" alt="5 6AddMdavisToDomainAdmin" src="https://github.com/user-attachments/assets/2cab2305-06da-4388-9096-6bbba6f18c82" />

Verifying all of Mdavis Groups
<img width="1024" height="768" alt="5 7VerifyMdavisGroups" src="https://github.com/user-attachments/assets/2c26f559-17a3-4bd3-8ce5-7d4b9818f2bf" />

Logging into Admins Account From PC-001
<img width="1024" height="768" alt="5 8LoggingIntoAdmin" src="https://github.com/user-attachments/assets/6926ec8d-56dd-4ab1-bd24-bf95a1e5af03" />

Loggin Successful0
<img width="1024" height="768" alt="5 9LoggedIntoAdmin" src="https://github.com/user-attachments/assets/698c5014-bac2-4d36-a168-465c53098f95" />

## Conclusion
This lab introduced enterprise privileged access management by seperating administrative identities from standard user accounts. The enviornment now follows the Principle of Least Privilege, laying the groubdwork for delegated administration, security hardening, and advanced access control in future labs.

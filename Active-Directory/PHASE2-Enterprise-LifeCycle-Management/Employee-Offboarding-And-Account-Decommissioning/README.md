# Employee Offboarding & Account Decommissioning Lab

## Objective 
Simulate a secure employee offboarding process by disabling an Active Directory account, removing Security Group memberships, relocating the account to a dedicated Disabled Users Organizational Unit, and verify access revocation

## Why This Lab Matters
Employee terminations require immediate action to protect organizational resources. This lab demonstrates enterprise offboarding procedures that help maintain security, compliance, and accurate identity management.

## Steps Performed
- Create a Disabled Users Organizational Unit
- Disabled the employee's Active Directory account
- Removed deprtment specific Security Groups memberships
- Moved the account to the Disabled Usrs OU
- Verified authentication was blocked
- Completed a service desk ticket documenting the termination

## Screenshots

Creating Disabled User OU
<img width="1024" height="768" alt="10 1CreatingNewOU" src="https://github.com/user-attachments/assets/b6fa7af2-b1fb-45df-be36-5878e7d8ef4e" />

Targeted User
<img width="1024" height="768" alt="10 2DisabledUser" src="https://github.com/user-attachments/assets/be727d49-69b9-4d02-b464-f8d372b20747" />

User Moved to Disabled OU
<img width="1024" height="768" alt="10 3Transfered" src="https://github.com/user-attachments/assets/1b43f727-5add-4aba-aaf6-04bfd8e8051d" />

Current GG-Sales
<img width="1024" height="768" alt="10 4CurrentSalesGG" src="https://github.com/user-attachments/assets/f42a55d8-dd96-4549-a336-f17f62b8f051" />

User Removed from GG-Sales
<img width="1024" height="768" alt="10 5Removed" src="https://github.com/user-attachments/assets/68b033f8-1d49-4fb0-a6a6-570972fd3659" />

Disabled Account
<img width="1024" height="768" alt="10 6DisableAccount" src="https://github.com/user-attachments/assets/5360d98d-16d3-4f54-8d47-bd5e7699f741" />

Confirmed Disabled Account
<img width="1024" height="768" alt="10 7ConfirmDisableAccount" src="https://github.com/user-attachments/assets/540c240d-fcc5-4c24-99e6-0acc0ddd7e31" />

## Conclusion
This lab siulated a complete employee offboardding workflow commonly performed by Help Desk and System Administrators. It reinforced secure account deactivation, least privlege principles, Active Directory organization, and the importance of maintaining a documented audit trail for terminated users.

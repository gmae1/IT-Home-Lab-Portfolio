# Employee Department Transfer And Permission Management

## Objective 
Simulate an employee department transfer by updating Active Directory Organizational Unit placement, user attributes, and Security Group memberships while enforcing the Principle of Least Privilege.

## Why This Lab Matters
Employee transfers are a routine part of enterprise identity management. Administrators must ensure users receive appropriate access for their new roles while removing permissions that are no longer required.

## Steps Performed
- Moved Emily Carter from the Finance OU to the IT OU
- Update her department and job title
- Removed her from the Finance Security Group
- Addrd her to thhe IT Security Group
- Verified Organizational Unit placement
- Verified Security Group memberships
- Doccumented the administrative changes

## Screenshots

Emily Carter User
<img width="1024" height="768" alt="7 1EmilyC" src="https://github.com/user-attachments/assets/21578a20-3ece-4110-aaf8-a321758de76b" />

Moved User Department
<img width="1024" height="768" alt="7 2MoveUserDepartment" src="https://github.com/user-attachments/assets/8f518938-e1e0-4841-9feb-e8d94147075c" />

Emilys Old Properties
<img width="1024" height="768" alt="7 3OldProperties" src="https://github.com/user-attachments/assets/aecc46a6-697e-4403-9154-9397b6e8d0cf" />

Emilys New Properties
<img width="1024" height="768" alt="7 4NewProperties" src="https://github.com/user-attachments/assets/973a5b6d-a6b5-4014-8f7c-c0da3da9d55c" />

Old Global Group
<img width="1024" height="768" alt="7 5OldGG" src="https://github.com/user-attachments/assets/cc033d35-4c71-4cf7-bac5-c82397347b85" />

New Global Group
<img width="1024" height="768" alt="7 6NewGG" src="https://github.com/user-attachments/assets/7191e18c-71c6-4e03-908a-61ae4633ab14" />

Global Group Verification
<img width="1024" height="768" alt="7 7GGVerify" src="https://github.com/user-attachments/assets/ac1131f6-9bdc-4067-9459-0194dde8e374" />

## Conclusion
This lab demonstrated a realistic employee transfer within a enterprise Active Directory environment. The users account was updated to reflect their new department and responsibilities while outdated permissions were removed to maintain the Principle of Least Privilege. The exercise reinforced the importance of acurate identity management, proper doccumentation, and secure access control during employee lifecycle events.

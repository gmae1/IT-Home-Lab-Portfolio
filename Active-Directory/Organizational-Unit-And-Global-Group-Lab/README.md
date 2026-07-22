# Organizzational Unit (OU) and Global Group Lab

## Objective
Designed and implemented a scalable Organizational Unit structure for Contoso Technologies and create department-based Global Security Groups that will be used for permissions, Global Policy, and access management throughout the remainder of the lab series.

## Why this Matters
One of the first things a Windows Administrator does after deploying Active Directory is organize it. 
A poorly organized Active Directory quickly becomes difficult to manage. We want to be able to seperate users, computers, servers and departments into OUs. This will allow us to Apply Group Policies to specific departments, Delegate administrative controls, Organize users logically, Simplify Troubleshooting, and Improvve Security.

Security Groups are equally important because they allow administrators to assign permissions to group instead of individual users.

## Skills Learned
- Created Organizational Units
- Understad the purpose of OUs
- Create Global Security Groups
- Understand Security Group scopes
- Follow enterprise Active Directory organization standards
- Prepare Active Directory for future Grouup Policy deployment

## Steps Performed
- Created a top-level "Contoso" Organizational Unit
- Built child OUs (Users, Computers, Servers, Groups, Service Accounts, and Admin Accounts)
- Created department specific OUs under the Users container
- Created Workstation and Laptops OUs under Computer OUs
- Createed Gobal Security Groups for each department using a standard name
- Verified OUs hieractchy and group configuration

## Screenshots

Created OU
<img width="1024" height="768" alt="3 1CreatingNewOU" src="https://github.com/user-attachments/assets/6c721f19-c9df-4a24-b0dd-076a17fb05e4" />

Created Child OUs for each Department
<img width="1024" height="768" alt="3 2CreatedOUsInsideContoso" src="https://github.com/user-attachments/assets/6b3faf1d-4dce-453d-842c-669549405f3b" />

Global Groups
<img width="1024" height="768" alt="3 4GlobalGroups" src="https://github.com/user-attachments/assets/2c7bd213-40ac-4ed0-b98b-b840af80728e" />

Hierarchy Verification
<img width="1024" height="768" alt="3 3CreatedNewOUs" src="https://github.com/user-attachments/assets/5d9826ce-ef91-477e-b4ec-c9f69f67158d" />

## Conclusion
This lab transformed the default Active Directory layout into a enterprise ready structure that supports future user management, Group Policy deployment, dekegated administration and secure permission assignment. The enviornment is now organized according to reak world Active Directory administration practices.

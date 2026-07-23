# Deploy Additional Workstations and Organize Computer Objects Lab

## Objective
Deploy additional Windows 11 Pro workstations, join them to the Active Directory domain, and organize computer objects into dedicated Organizational Unit for enterprise management.

## Why This Lab Matters
Enterprise environments require consistent deployment and organization of workstations. Properly managing computer accounts enables targeted Group Policy, simplifies administration, and improve scalability.

## Steps Performed
- Created two additional Windows Pro 11 Virtual Machines
- Configured static IPv4 settings and DNS
- Verified connectivity to the Domain Controller
- Joined both systems to the "corp.contoso.local" domain
- Moved all workstation computer objects into Workstations Organizational Unit
- Verified domain membership and Active Directory organization.

## Screenshots

New PC002/PC003 Workstation
<img width="831" height="337" alt="6 2NewWorkstation" src="https://github.com/user-attachments/assets/7a7527c9-cf6d-47af-bd06-ecbffec90908" />
<img width="779" height="293" alt="6 5CreatedPC003" src="https://github.com/user-attachments/assets/a77d8d46-d882-455d-83e4-861eba0f903c" />


Configured PC002/PC003 IP Adress
<img width="1024" height="768" alt="6 1ConfiguringPC002" src="https://github.com/user-attachments/assets/bf457ef2-94d5-406c-b888-5b4af39607c0" />
<img width="1024" height="768" alt="6 6ConfiguringPC003" src="https://github.com/user-attachments/assets/8f91fbb6-4a99-48aa-8c63-dc962c401f1a" />

Adding PC's to Corp.Contoso.Local Domain
<img width="1024" height="768" alt="6 7AddingPC003ToDomain" src="https://github.com/user-attachments/assets/775edf95-74ce-4622-92f0-cf4fd75e1924" />
<img width="1024" height="768" alt="6 3AddingPC002ToDomain" src="https://github.com/user-attachments/assets/5c3af7a1-cba2-41b0-89dc-e5b65313a9cb" />

Adding DOmain Success
<img width="1024" height="768" alt="6 4PC002Success" src="https://github.com/user-attachments/assets/f9509320-5f59-4db3-80f1-ff61f8c7144d" />
<img width="1024" height="768" alt="6 8PC003Success" src="https://github.com/user-attachments/assets/74f374b2-0c8e-414d-88e7-1a3a18d43bbd" />

Verifying Hosname And Domain Memebership
<img width="1024" height="768" alt="6 11Hostname" src="https://github.com/user-attachments/assets/130f6f83-d473-4f02-bcae-822afd668ee2" />
<img width="1024" height="768" alt="6 9Hostname" src="https://github.com/user-attachments/assets/6a8b0c9e-e6f3-441e-a7fc-f2aca534cce5" />
<img width="1024" height="768" alt="6 10DomainVerify" src="https://github.com/user-attachments/assets/dc0f5e25-c698-4884-bc54-4f70e1959b67" />
<img width="1024" height="768" alt="6 12DomainVerifyPC002" src="https://github.com/user-attachments/assets/7a6df9d7-4db1-4bdd-aac9-62f65f559455" />

Organizing Workstations to the Workstation OU Container
<img width="1024" height="768" alt="6 13ADUCVerification" src="https://github.com/user-attachments/assets/d82edcf7-06e8-4ffe-ae18-370d8042fefb" />

## Conclusion
This lab simulated the deployment if additional enterprise workstations and demonstrated proper Active Directory computer account management. By organizing computer objects into a dedicated Ogranizational Unit, the enviornment is now prepared for centralized Group Policy management and continued enterprise growth.

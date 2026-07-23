# Deploy First Domain Controller 

## Objective
Deploy the first Windows Server 2022 Domain Controller by installing Active Directory Domain Services and DNS, creating a new Active Directory forest, and preparing the environment for enterprise identity managemnet.

## Why This Lab Matters 
Organizations rely on Domain Controllers to centraliza authentication, authorization, DNS, and policy management. This lab establishes the core infrastructure required for all future Windows administration tasks.

## Step Performed
- Installed Windows Server 2022 (Desktop Experience)
- Renamed the server DC01
- Configured a static IPv4 address (192.168.50.10)
- Installed AD DS and DNS Server roles.
- Promoted the server to the first Domain Controller in the corp.contoso.local forest
- Verified Active Directory and DNS functionality using administrative toiks abd command linw utilites

## Screenshots

Created a Active Directory Virtual Machine
<img width="796" height="652" alt="1 1CreatedADVM" src="https://github.com/user-attachments/assets/70c4263e-9b03-434a-8003-3431ebaac1b8" />

Renaming Server to DC01
<img width="1024" height="768" alt="1 2RenamingServer" src="https://github.com/user-attachments/assets/4ae18e35-b75b-4253-8ce2-cb8eb380b2e3" />

Statically Changing IPv4
<img width="1024" height="768" alt="1 3ChangeStaticIP" src="https://github.com/user-attachments/assets/64ea180b-4106-4651-801d-2d0b8a016bc3" />

Adding ADDS/DNS Roles
<img width="1024" height="768" alt="1 4AddingADDS" src="https://github.com/user-attachments/assets/a521d16a-0204-4773-80e8-b9d99a1b35cf" />

Installation Completed
<img width="1024" height="768" alt="1 5InstiallationCompleted" src="https://github.com/user-attachments/assets/a24a12f2-c4dd-460a-8726-d0b021ed08cc" />

Creating New Forest
<img width="1024" height="768" alt="1 6CreatingNewForest" src="https://github.com/user-attachments/assets/6882f18f-0c7e-4896-b606-3670ff42ae02" />

Verifying ADUC Roles
<img width="1024" height="768" alt="1 7VerifyingADUS" src="https://github.com/user-attachments/assets/56e413a9-515a-4fb2-9888-3a080f636ff7" />

Verifying DNS Roles
<img width="1024" height="768" alt="1 8VerifyingDNS" src="https://github.com/user-attachments/assets/6bc73097-9b3b-487e-8a34-d9f84136de43" />

Verifying IPv4
<img width="1024" height="768" alt="1 9VerifyIPAddress" src="https://github.com/user-attachments/assets/27b7c2ec-037c-4605-b4b4-08c196aaecb1" />

nslookup Verification
<img width="1024" height="768" alt="1 10nslookupVerify" src="https://github.com/user-attachments/assets/00718417-df16-4204-8e86-50933a063cb4" />

## Conclusion
This Lab establishesed the foundational Active Directory infrastucture for the enviornment. With a functioning Domain COntroller and intergrated DNS, the domain is now ready for orginazational units, users, grouos, Group Policym and the day to day administration task performed in enterprise Window enviornments.


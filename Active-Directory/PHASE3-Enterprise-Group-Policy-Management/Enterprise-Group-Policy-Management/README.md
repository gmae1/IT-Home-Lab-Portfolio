# Lab 14 — Restrict Control Panel & Windows Settings Using Group Policy

## Overview

In this lab, I configured and deployed a user-based Group Policy Object (GPO) in a Windows Server 2022 Active Directory environment to restrict standard domain users from accessing the Windows Control Panel and PC Settings.

The policy was scoped to the organization's employee Users OU and tested using a standard domain user account. Group Policy processing was then verified from the Windows 11 workstation using `gpresult`.

---

## Objective

The objective of this lab was to:

- Create a user-targeted Group Policy Object
- Restrict access to Control Panel and Windows Settings
- Apply the policy to standard employee accounts
- Understand the difference between User Configuration and Computer Configuration
- Validate that the GPO was successfully applied to a domain user
- Practice troubleshooting and verifying Group Policy deployment

---

## Environment

| Component | Configuration |
|---|---|
| Domain | corp.contoso.local |
| Domain Controller | DC01 |
| Server OS | Windows Server 2022 |
| Domain Controller IP | 192.168.50.10 |
| Client OS | Windows 11 Pro |
| Virtualization | VirtualBox |
| GPO | Standard User - Control Panel Restriction |
| Test User | Sarah Johnson (sjohnson) |

---

## Active Directory Scope

The environment uses a structured OU hierarchy for managing users and computers.

The restriction was linked to the employee Users OU so that standard employee accounts within its child OUs could inherit the policy.

Example structure:

Contoso
├── Users
│   ├── HR
│   │   └── Sarah Johnson
│   ├── IT
│   ├── Finance
│   ├── Sales
│   └── Engineering
│
├── Admin Accounts
├── Help Desk
├── Computers
├── Groups
└── Servers

This design allows policies intended for standard employees to be separated from administrative accounts.

---

## Group Policy Configuration

A Group Policy Object named:

`Standard User - Control Panel Restriction`

was linked to the Contoso employee Users OU.

The following policy was configured:

User Configuration  
→ Policies  
→ Administrative Templates  
→ Control Panel  
→ Prohibit access to Control Panel and PC settings

Configuration:

`Enabled`

Security Filtering:

`Authenticated Users`

---

## User Configuration vs. Computer Configuration

One of the primary concepts demonstrated in this lab was understanding how Group Policy scope changes depending on the configuration type.

### User Configuration

User Configuration policies apply based on the location of the **user object** in Active Directory.

For this lab, Sarah Johnson's user account was located within the employee Users OU hierarchy.

Therefore, the Control Panel restriction followed Sarah's user account when she logged into the domain workstation.

### Computer Configuration

Computer Configuration policies instead apply based on the location of the **computer object** in Active Directory.

This distinction is important when designing and troubleshooting Group Policy in enterprise environments.

---

## Policy Deployment

After configuring the GPO, I logged into a Windows 11 domain workstation using:

`CORP\sjohnson`

Group Policy was refreshed using:

`gpupdate /force`

After policy processing, the Control Panel restriction was tested using Sarah's domain account.

---

## Validation

The following tests were successfully completed:

| Validation Test | Result |
|---|---|
| GPO created and configured | PASS |
| GPO linked to employee Users OU | PASS |
| User Configuration policy enabled | PASS |
| Standard domain user received policy | PASS |
| Sarah Johnson blocked from Control Panel | PASS |
| Applied GPO verified from Command Prompt | PASS |

The restriction successfully prevented the standard employee account from accessing Control Panel.

---

## Group Policy Verification

To verify that the restriction was being delivered through Group Policy, I used:

`gpresult /r`

The results confirmed that:

`Standard User - Control Panel Restriction`

was included in the user's applied Group Policy Objects.

This provided evidence that the restriction was being enforced by the intended domain GPO rather than by a local workstation configuration.

---

## Troubleshooting Experience

During configuration, I initially navigated to:

Computer Configuration  
→ Policies  
→ Administrative Templates  
→ Control Panel

The required setting was not available in the expected location.

I identified that the restriction was intended to target **users rather than computers** and corrected the configuration path to:

User Configuration  
→ Policies  
→ Administrative Templates  
→ Control Panel

This reinforced the importance of understanding whether a Group Policy setting belongs to User Configuration or Computer Configuration when deploying and troubleshooting GPOs.

---

## Skills Demonstrated

- Windows Server 2022 Administration
- Active Directory Domain Services
- Group Policy Management
- Group Policy Objects (GPO)
- Organizational Unit Design
- User-Based Policy Deployment
- Group Policy Inheritance
- Security Filtering
- Windows 11 Domain Administration
- `gpupdate`
- `gpresult`
- Group Policy Troubleshooting
- Policy Validation

---

## Screenshots

GPOME
<img width="1024" height="768" alt="15 2GPME" src="https://github.com/user-attachments/assets/53b20803-ec6b-41dc-b7ca-f9c5f7cc2eda" />

Prohibit Control Pannel 
<img width="1024" height="768" alt="15 3ProhibitCP" src="https://github.com/user-attachments/assets/f59d68a8-3987-4f0c-a5a0-ba09a5899889" />

Enable Control Panel
<img width="1024" height="768" alt="15 3ProhibitCP" src="https://github.com/user-attachments/assets/2c95c2c6-04f1-4a18-bd0a-1f02933af56a" />

Logging in as Sarah Johnson
<img width="1024" height="768" alt="15 6LoggingSJ" src="https://github.com/user-attachments/assets/f5f9abc0-ca43-4a36-9047-25f0eaf2c92f" />

Control Pannel Restriction
<img width="1024" height="768" alt="15 7Restriction" src="https://github.com/user-attachments/assets/bb3f9b51-b887-4055-96c0-3e873f11d54d" />

Group Policy Results
<img width="1024" height="768" alt="15 8GPResult" src="https://github.com/user-attachments/assets/97ef2e70-68f7-48b8-a950-a32bf554402b" />


---

## Key Takeaways

This lab demonstrated that Group Policy deployment depends on both the configured policy and the location of Active Directory objects.

A user-based policy linked to an employee OU can follow the user regardless of which domain workstation they use, provided the user falls within the GPO's applicable scope.

I also gained hands-on experience using `gpresult` to verify Group Policy processing rather than assuming that a policy applied simply because the expected behavior occurred.

---

## Resume Bullet

- Configured and deployed a user-targeted Active Directory Group Policy restricting Control Panel and Windows Settings access for standard employees, validating successful policy application using `gpupdate` and `gpresult` in a Windows Server 2022 domain environment.

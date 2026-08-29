# Deploy a Mapped Network Drive Using Group Policy Lab

## Overview

In this lab, I configured a centralized Windows network share and used
Active Directory Group Policy Preferences to automatically map the shared
resource as a network drive for domain users.

The network share was hosted on a Windows Server 2022 domain controller and
deployed to users within the Contoso employee Users OU.

The deployment was tested from a Windows 11 domain workstation using a
standard employee account.

---

## Objective

The objectives of this lab were to:

- Create a centralized Windows network share
- Configure basic SMB share permissions
- Test access using a UNC path
- Create a Group Policy Object for drive mapping
- Deploy a mapped network drive using Group Policy Preferences
- Automatically assign the S: drive to domain users
- Validate Group Policy processing using gpresult
- Verify access to the mapped resource from a domain workstation

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
| Network Share | \\DC01\Shared |
| Mapped Drive | S: |
| GPO | Map Corporate Shared Drive |
| Test User | Sarah Johnson (sjohnson) |

---

## Network Share Configuration

A centralized folder structure was created on DC01:

C:\CompanyShares\Shared

The folder was shared across the network using the share name:

Shared

This created the UNC path:

\\DC01\Shared

A test file was placed inside the directory:

Welcome-to-Contoso.txt

The file was used to verify that domain users could successfully access
content hosted on the network share.

---

## UNC Path Testing

Before deploying the drive through Group Policy, the network share was
tested manually from a Windows 11 domain workstation.

While logged in as:

CORP\sjohnson

the following UNC path was accessed:

\\DC01\Shared

The share successfully opened and the test file was accessible.

This verified that network connectivity, DNS name resolution, SMB sharing,
and basic permissions were functioning before Group Policy was introduced.

---

## Group Policy Configuration

A new Group Policy Object was created:

Map Corporate Shared Drive

The GPO was linked to the Contoso employee Users OU.

The drive mapping was configured using:

User Configuration
→ Preferences
→ Windows Settings
→ Drive Maps

The following settings were configured:

| Setting | Value |
|---|---|
| Action | Create |
| Location | \\DC01\Shared |
| Label | Contoso Shared |
| Drive Letter | S: |

Security Filtering remained configured for:

Authenticated Users

---

## Group Policy Preferences

This lab introduced Group Policy Preferences.

Unlike many administrative policy settings, Group Policy Preferences can
be used to deploy and configure resources such as:

- Network drive mappings
- Printers
- Shortcuts
- Registry settings
- Files and folders

For this deployment, a Drive Maps preference automatically created the
S: drive for users receiving the GPO.

---

## Deployment

After configuring the GPO, I logged into the Windows 11 workstation using
the standard domain employee account:

CORP\sjohnson

Group Policy was refreshed using:

gpupdate /force

After policy processing and user sign-in, the mapped drive appeared
automatically in File Explorer as:

Contoso Shared (S:)

The mapped drive pointed to:

\\DC01\Shared

---

## Validation

The following validation tests were successfully completed:

| Validation Test | Result |
|---|---|
| Shared folder created on DC01 | PASS |
| Folder shared through SMB | PASS |
| UNC path accessible from workstation | PASS |
| Test file accessible through UNC path | PASS |
| Drive mapping GPO created | PASS |
| GPO linked to employee Users OU | PASS |
| Drive Maps preference configured | PASS |
| Group Policy update completed | PASS |
| S: drive automatically mapped | PASS |
| Test file accessible through S: | PASS |
| GPO verified using gpresult | PASS |

---

## Group Policy Verification

The following command was used to verify Group Policy processing:

gpresult /r

Under the user policy results, the following GPO was confirmed as applied:

Map Corporate Shared Drive

This verified that the mapped drive deployment originated from the
intended domain Group Policy Object.

---

## Architecture

DC01
│
├── C:\CompanyShares\Shared
│
└── SMB Share
    │
    └── \\DC01\Shared
            │
            ▼
     Map Corporate Shared Drive GPO
            │
            ▼
       Contoso Users OU
            │
            ▼
       Domain Employee
            │
            ▼
       Windows 11 Client
            │
            ▼
     Contoso Shared (S:)

---

## Troubleshooting Methodology

The network share was tested independently before Group Policy deployment.

This helped separate potential file-sharing problems from Group Policy
problems.

The troubleshooting process used in this lab was:

1. Verify network connectivity
2. Verify DNS/name resolution
3. Test the UNC path directly
4. Verify share access
5. Verify GPO scope and link
6. Force Group Policy processing
7. Verify applied GPOs with gpresult
8. Verify the mapped drive

This approach prevents unnecessary changes to Group Policy when the actual
problem may be related to networking, DNS, SMB, or permissions.

---

## Key Concepts Learned

### UNC Path

A Universal Naming Convention path identifies a shared network resource.

Example:

\\DC01\Shared

Format:

\\ServerName\ShareName

---

### Mapped Network Drive

A mapped drive assigns a drive letter to a network resource.

In this environment:

S:
→ \\DC01\Shared

This provides users with a familiar way to access centralized network files.

---

### Group Policy Preferences

Group Policy Preferences allow administrators to deploy configurable
resources and settings to domain users and computers.

In this lab, Group Policy Preferences automatically created a mapped
network drive for employees.

---

## Skills Demonstrated

- Windows Server 2022 Administration
- Active Directory Domain Services
- Group Policy Management
- Group Policy Preferences
- Drive Maps
- Windows File Sharing
- SMB
- UNC Paths
- Windows 11 Domain Administration
- Organizational Unit Management
- GPO Linking and Scope
- gpupdate
- gpresult
- Network Resource Deployment
- Group Policy Troubleshooting

---

## Screenshots

C Drive
<img width="1024" height="768" alt="16 1CDrive" src="https://github.com/user-attachments/assets/da31f1ec-7d90-4283-b967-233c049f03f5" />

Company Share
<img width="1024" height="768" alt="16 2CompanyShare" src="https://github.com/user-attachments/assets/531861b8-9188-45b8-8906-d62c12cab753" />

Text Document
<img width="1024" height="768" alt="16 3WordTxt" src="https://github.com/user-attachments/assets/fd2b2866-326d-4b6e-bd6a-7ea5cc46191e" />

Share Properties
<img width="1024" height="768" alt="16 4ShareProperties" src="https://github.com/user-attachments/assets/0e067361-5c7f-4150-b7e8-5acd6b3166e7" />

Shared Permissions
<img width="1024" height="768" alt="16 6SarahJohnson" src="https://github.com/user-attachments/assets/71d52983-2a48-4161-9419-3a3cf0a29b55" />

Sarahs Access To Shared Doccument
<img width="1024" height="768" alt="16 7Access2Doc" src="https://github.com/user-attachments/assets/8ee45e18-e7e9-47aa-bcf5-11d974394340" />

Group Policy Management
<img width="1024" height="768" alt="16 8GPM" src="https://github.com/user-attachments/assets/8af5b26e-eab0-4c65-b005-da2d5283fe84" />

New GPO
<img width="1024" height="768" alt="16 9NewGPO" src="https://github.com/user-attachments/assets/7ddebb8f-7895-4278-be56-9eb20b7c2a0c" />

GPM Editor
<img width="1024" height="768" alt="16 10GPManagementEditor" src="https://github.com/user-attachments/assets/fbdebda3-e62d-4f4e-820e-5bf4444cea1f" />

Drive Map
<img width="1024" height="768" alt="16 11DriveMap" src="https://github.com/user-attachments/assets/6c12c3db-362b-464c-8f38-ee546ccd212e" />

Drive Map Properties
<img width="1024" height="768" alt="16 12DriveMapProps" src="https://github.com/user-attachments/assets/aa9068f0-8034-4594-a640-a1e36e4a3759" />

GP Update (Server)
<img width="1024" height="768" alt="16 13GPUpdate" src="https://github.com/user-attachments/assets/d59d1f3e-d7ef-4de2-8b1a-d40e67a23d44" />

GP Update (User Workstation)
<img width="1024" height="768" alt="16 14GPUpdateUser" src="https://github.com/user-attachments/assets/0893b410-f15e-4ca2-a439-9209d5a6af9f" />

Verify New S: Drive
<img width="1024" height="768" alt="16 15VerifyDrive" src="https://github.com/user-attachments/assets/73831365-cc3d-4893-a7f4-2b91dfc6de87" />

Verify Group New Group Policy
<img width="1024" height="768" alt="16 16VerifyGP" src="https://github.com/user-attachments/assets/036b2374-5f18-4eda-bcf3-862a530e0ac6" />

Sarah Can Edit New Text
<img width="1024" height="768" alt="16 17SarahEdit" src="https://github.com/user-attachments/assets/12aad9d4-9452-452a-ba05-b8430d3b34d0" />

---

## Key Takeaways

This lab demonstrated how Active Directory Group Policy Preferences can
automate the deployment of network resources to domain users.

Instead of manually mapping network drives on individual workstations,
the mapped drive can be centrally configured and automatically delivered
to users through Group Policy.

The lab also demonstrated the importance of testing the underlying network
resource before troubleshooting Group Policy.

---

## Resume Bullet

- Configured a centralized Windows SMB network share and automated network
  drive deployment using Active Directory Group Policy Preferences,
  providing domain users with mapped access to shared organizational
  resources and validating policy application using gpresult.

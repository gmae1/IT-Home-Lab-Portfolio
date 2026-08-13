# Domain Password Policy & Account Security

## Objective
Configure and validate a centralized Active Directory domain password policy for Contoso Technologies using Group Policy.

The policy establishes standardized password requirements for domain users, including password length, complexity, history, and aging requirements.

The lab also validates the policy by testing both compliant and non compliant password against an Active Directory user accounts.

## Why This Lab Matters
Password security is a fundamental component of enterprise identity and access management.

In an Active Directory environment, administrators can centrally enforce passwords requirements for domain accounts rather than relying on individual workstation configurations.

Centralized password policies help organizations:
  - Establish consistent credential requirements
  - Reduce the use of weak passwords
  - Prevent immediate password reuse
  - Standardize account security across departments
  - Maintain centrally managed identity security controls

This lab also demonstrates the difference between a workstation targeted GPO and a domain account.

## Skills Demonstrated
- Active Directory administration
- Group Policy Management
- Domain password policy configuration
- Password complexity enforcement
- Password history configuration
- Password aging
- Credential security
- Group Policy refresh
- Command line verification
- Security control validation
- Enterprise change documentation

## Steps Performed

1. Access the Domain Account Policy
2. Configure Password History
3. Configure Password Aging
4. Configure Minimum Password Length
5. Enable Password Complexity
6. Disable Reversible Encryption
     - Reversible password storage was disabled to reduce unnecessary credential; exposure
7. Refreshed Group Policy
8. Verified the Domain Account Policy
9. Test Password Enforcement

## Lesson Learned
- Active Directory domain password policies are centrally managed through Group Policy
- Domain account policies differ from GPOs targeted specifically at workstation OUs
- Password history helps prevent immediate credential reuse
- Minimum password age can prevent users from rapidly cycling through their password history
- Password complexity and password length provide separate security controls
- Reversible password encryption should normally remain disabled
- gpupdate /force can be used during policy deployment and testing
- net accounts /domain provide quick method for verifying domain account policy values
- A security control should be tested after configuration rather than assumed to be working

## Screenshots

GPO
<img width="1024" height="768" alt="13 1GPOMan" src="https://github.com/user-attachments/assets/f56a85e2-bdbc-4b03-8f30-aa647131db84" />

GPO Editor
<img width="1024" height="768" alt="13 2Editor" src="https://github.com/user-attachments/assets/181b27a6-fa6b-4122-a213-3bcad7115e75" />

Password Policy
<img width="1024" height="768" alt="13 3PasswordPolicy" src="https://github.com/user-attachments/assets/6a0997af-785a-4cb9-b88f-1afe99b5dd8a" />

Change Password Age
<img width="1024" height="768" alt="13 5PasswordAge" src="https://github.com/user-attachments/assets/5ed75dc8-1214-4fb3-9a16-64a68da143e5" />

Minimum Password Age
<img width="1024" height="768" alt="13 6MinPassAge" src="https://github.com/user-attachments/assets/57b3956f-3d54-422b-93e2-e1c7d33f7d63" />

Minimum Password Length
<img width="1024" height="768" alt="13 7MinPassLength" src="https://github.com/user-attachments/assets/15831c8f-f287-457a-a848-584962f0d3fa" />

Max Password Age
<img width="1024" height="768" alt="13 8MaxPassAge" src="https://github.com/user-attachments/assets/a57a1ee8-3f82-4aa8-88c0-9c2a0675dd89" />

Password Complexity
<img width="1024" height="768" alt="13 9PasswordComplex" src="https://github.com/user-attachments/assets/56cb164e-3bbb-459a-9970-051448454a51" />

Reversible Encryption
<img width="1024" height="768" alt="13 10Encrypt" src="https://github.com/user-attachments/assets/d428f0f3-dae8-443c-bf02-0715d6ea2b01" />

Force Update
<img width="1024" height="768" alt="13 11ForceUpdate" src="https://github.com/user-attachments/assets/8c901b40-cbb9-4f93-81ed-6defc34617c5" />

Force Update Verification
<img width="1024" height="768" alt="13 12ForceUpdate" src="https://github.com/user-attachments/assets/39dc9ac3-6af1-42be-b628-63b179bd3815" />

Inform User of Password 
<img width="1024" height="768" alt="13 13" src="https://github.com/user-attachments/assets/a73e258a-aac2-4dc7-b8c9-656ea95816a7" />


## Conclusion 
This lab demonstrated the implementation and validation of centralized password security within an Active Directory domain

Password history, age, minimum length, complexity, and encryption requirements were configured through Group Policy and verified using administrative command line tools

Testing against Active Directory user accounts confirmed that noncompliant password was rejected while compliant passwords were accepted.

The lab reinforced an important systems administration practice. Security configurations should be validated from the perspective of the systems and users they are intended to protect rather than consider complete simply became the configuration exists.

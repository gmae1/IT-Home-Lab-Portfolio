# Group Policy Security Poicies

## Objective
Implement domain wide security policies using Group Polict to enforce password requirements and account lockout protections across Active Directory.

## Why This Lav Matters
Group Policy allws administrators to centrally manage security settings for all domain users and computers. By enforcing password complexity and account lockout polocies, organizations reduce the risk of weak passwords

## Task Performed
- Opened Group Policy Management
- Configured Password Policy
- Forced Group Policy "gpupdate /force"
- Verified Password Policy "net accounts"
- Modified Account Lockout Settings
- Forced Policy "gpupdate /force"
- Verified Lockout Policy "net accounts"
- Tested Authentication Failures
- Unlocked Account from Users Account in Active Directory Users and Computers

## Screenshots

Group Policy Management
<img width="1024" height="768" alt="8 1Group_Policy" src="https://github.com/user-attachments/assets/896c2f19-2030-45a9-9d92-733d5a629e45" />

Password Policy Management
<img width="1024" height="768" alt="8 3Password_Policy_Management" src="https://github.com/user-attachments/assets/f1eeabef-d008-4260-92d7-0aca0325b57e" />

Password Length Change/ History/ Age
<img width="1024" height="768" alt="8 4Password_Length_Change" src="https://github.com/user-attachments/assets/3a48e095-4c04-4347-a481-238f9e73ed99" />
<img width="1024" height="768" alt="8 5Password_History" src="https://github.com/user-attachments/assets/92b954ad-cdc0-430f-a360-668928a38de8" />
<img width="1024" height="768" alt="8 6Maximum_Password_Age" src="https://github.com/user-attachments/assets/5a2caadd-4f76-46ef-b4f1-7d47a31bd8bb" />

Password Force Update
<img width="1024" height="768" alt="8 7Update" src="https://github.com/user-attachments/assets/b9307d17-e3e0-4c1d-9f5e-5e34c06dffeb" />

Verify Updates
<img width="1024" height="768" alt="8 8Verify_Updates" src="https://github.com/user-attachments/assets/1bd0a2e5-2f6e-4a93-aa45-8e1194b56504" />

Account Lockout Policy
<img width="1024" height="768" alt="8 9Account_Lockout_Policy" src="https://github.com/user-attachments/assets/c07a48b1-1a00-45a8-a3b9-831e3d4df976" />

Account Lockout Threshold/ Lockout Duration/Reset Account Counter
<img width="1024" height="768" alt="8 10Account_Lockout_thresh" src="https://github.com/user-attachments/assets/4162b5e1-9ee7-4f43-89d9-919cd1d79276" />
<img width="1024" height="768" alt="8 11Account_Lockout_Duration" src="https://github.com/user-attachments/assets/282fefb3-ee0d-475e-9fca-443dd2fd4cd3" />
<img width="1024" height="768" alt="8 12Reset+Account_Counter" src="https://github.com/user-attachments/assets/cb7b5f73-4ccf-4326-af34-43a5f8c2fe0b" />

Acount Lockout Force Update
<img width="1024" height="768" alt="8 13Update" src="https://github.com/user-attachments/assets/fca3f266-8cbe-4b15-8751-
b50890205fcd" />

Verify Account Lockout Update
<img width="1024" height="768" alt="8 14Verify_Accounts" src="https://github.com/user-attachments/assets/f563aff2-8e7f-45e8-bd07-f26ef5910915" />

Account Locked Out
<img width="1024" height="768" alt="8 15Account_LcokedOut" src="https://github.com/user-attachments/assets/ce5e250a-3fe7-4a82-8065-88c608df2d77" />

Unlock Account From AD UC
<img width="1024" height="768" alt="8 16Unlock_Account" src="https://github.com/user-attachments/assets/652fd9d2-271f-496e-953c-241c401c474c" />

Successful Login After Unlocked Account
<img width="1024" height="768" alt="8 17Successful_Login" src="https://github.com/user-attachments/assets/07d867d5-708d-4e50-8909-f1338cbd8e0d" />

## Conclusion
Implemented domain-wide password and account lockout policies and Group Policy Management to enforce security standards and protect Active Directory accounts against brute-force attacks.


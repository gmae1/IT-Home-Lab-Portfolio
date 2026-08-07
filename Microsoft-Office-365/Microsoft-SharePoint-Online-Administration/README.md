# Microsoft SharePoint Online Administration Lab

## Objective 
The objective of this section was to gain hands on experience administering Microsoft SharePoint Online within an enterprise Microsoft 365 enviornment.

Using the fictional company "Contoso Manufacturing", I configured departmental document storage, managed access, performed file recovery, worked with version history, configured file secure sharing, managed site ownership, and created an HR communication portal.

This lab demonstrates common SharePoint Online responsibilities performed by Microsoft 365 Administrators and Windows System Administrators.

## Why This Lab Matters 
SharePoint Online provides the document storage and collaboration infrastructure behind many Microsoft 365 service.

Administrators are commonly responsible for managing:
  - Department SharePoint sites
  - Document libraries
  - Permissions
  - Microsoft 365 Group integration
  - File recovery
  - Version history
  - Secure Sharing
  - Site ownership
  - Internal communication sites

Understanding SharePoint is especially important when administering Microsoft Teams because files uploaded to Teams channels are stored with SharePoint

## Lab 16 - Creating Engineering Document Library

## Objective 
Create a dedicated SharePoint document library for Engineering technical documentation.

### Steps Performed 
  - Accessed the Engineering SharePoint Team Site
  - Navigate to Site Contents
  - Created a new document library
  - Named the library Engineering Documentation
  - Added a description explaining its business purpose
  - Added the library to site navigation

### Results
Engineering received a dedicated document repository for technical and departmental documentation

### Screenshots 

Empty
<img width="1902" height="899" alt="Screenshot 2026-08-07 110631" src="https://github.com/user-attachments/assets/bd05e9c4-1fc2-4a43-b3bd-ba5c6625540d" />

Site Contents Before 
<img width="1915" height="903" alt="Screenshot 2026-08-07 110707" src="https://github.com/user-attachments/assets/3640d21b-a4ed-4eb0-85fa-a4a0729add4c" />

Creating New Document Library
<img width="797" height="464" alt="Screenshot 2026-08-07 110828" src="https://github.com/user-attachments/assets/92baf6a1-8493-46de-9639-adfe2d6fedf2" />

Verifying New Library 
<img width="812" height="342" alt="Screenshot 2026-08-07 110913" src="https://github.com/user-attachments/assets/b62922d9-02b9-4c9d-8096-ea2983177868" />

## Lab 17 - Organize Engineering Documentation

## Objective
Create a logical folder structure for Engineering documents.

## Steps Performed
  - Created the 3 folders: Active Projects, Standard Operating Procedures, and Archive
  - Created a test document called "Engineering Change Procedure" inside of the Standard Operating Procedures folder.

### Results 
Engineering documentation was organized into logical business categories

### Screenshots 

Folder Creation
<img width="574" height="451" alt="Screenshot 2026-08-07 111042" src="https://github.com/user-attachments/assets/afd6cfbf-a5f9-459d-8a71-5b3cc2c1bcda" />
<img width="602" height="373" alt="Screenshot 2026-08-07 111104" src="https://github.com/user-attachments/assets/6c4ce505-2c0a-446d-a38a-cad3f138ef55" />
<img width="623" height="473" alt="Screenshot 2026-08-07 111119" src="https://github.com/user-attachments/assets/7467e8b4-334c-4801-a4c1-ef057961ad46" />

Tex Document inside of the Standard Operating Procedures Folder
<img width="1809" height="418" alt="Screenshot 2026-08-07 111254" src="https://github.com/user-attachments/assets/4f772d0d-6c04-4c3b-938e-891b1c362e93" />

Verify Documents Creation
<img width="1296" height="300" alt="Screenshot 2026-08-07 111350" src="https://github.com/user-attachments/assets/c6dd6fed-ba1a-4c8d-8d27-87dff6068479" />

## Lab 18 - Manage SharePoint Permissions 

## Objective
Verify access to the Engineering SharePoint site through Microsoft 365 Group membership

## Steps Performed
  - Opened Engineering Site Permissions.
  - Reviewed Site Owners and Site Members
  - Verified Engineering Microsoft 365 Group membership
  - Confirmed Engineering employees received access through group membership
  - Verified administrator ownership

### Result
SharePoint access was managed through centralized Microsoft 365 Group membership instead of individual user permissions.

### Screenshots

Permission Taskbar
<img width="388" height="937" alt="Screenshot 2026-08-07 111828" src="https://github.com/user-attachments/assets/ac727f2e-0121-4d03-9c54-a87ff053bab5" />

Current Permissions for Users
<img width="379" height="307" alt="Screenshot 2026-08-07 111915" src="https://github.com/user-attachments/assets/81949735-af3c-4eb9-b10a-20155e08c9d4" />

Permission Access
<img width="292" height="724" alt="Screenshot 2026-08-07 121702" src="https://github.com/user-attachments/assets/bb460e52-72a4-4433-9ce1-c7c26c8f62e8" />
<img width="314" height="433" alt="Screenshot 2026-08-07 112037" src="https://github.com/user-attachments/assets/52dfb286-eb74-41bd-9f88-1256bbed0e91" />

## Lab 19 - Recover a Deleted SharePoint Document 

## Objective 
Recover an accidentally deleted Engineering document

## Scenario 
An Engineering employee accidentally deleted the Engineering Change Procedure text document.

## Steps Performed 
- Deleted the test document to simulate accidental deletion
- Opened the SharePoint Recycle Bin
- Located the deleted document
- Restored the document
- Verified the document returned to its original location

### Result
Successfully recovered deleted organizational data using SharePoint recovery capabilities 

### Screenshots 

Current Document
<img width="955" height="280" alt="Screenshot 2026-08-07 112258" src="https://github.com/user-attachments/assets/5070eca4-6331-4caf-b480-29c8ee52ab65" />

Deleted Document
<img width="1572" height="442" alt="Screenshot 2026-08-07 112332" src="https://github.com/user-attachments/assets/9e8affa2-0edf-4875-a6bd-f45764beb6d3" />

Document in Recycle Bin
<img width="1449" height="296" alt="Screenshot 2026-08-07 112352" src="https://github.com/user-attachments/assets/924fc135-336c-4c74-aaca-bed08d66748b" />

Restored Document 
<img width="1177" height="255" alt="Screenshot 2026-08-07 112412" src="https://github.com/user-attachments/assets/e91b2fc5-0ae3-4c42-a46f-63dae9d93cfb" />

## Lab 20 - Restore a Previous Document Version

## Objective
Recover a document after incorrect information was saved over the original content. 

## Steps Performed
  - Modified the Engineering Change Procedure Text Document
  - Opened SharePoint Version History
  - Reviewed pervious document versions
  - Identified the version created before the incorrect modification
  - Restored the previous version
  - Verified the original content was recovered

### Result
Successfully used SharePoint Version History to recover from an unwanted document modification.

### Screenshot

Incorrect Information
<img width="1487" height="543" alt="Screenshot 2026-08-07 112517" src="https://github.com/user-attachments/assets/dddb7c5c-cf7d-421a-9878-0fa9539979a4" />

SharePoint Version History
<img width="994" height="434" alt="Screenshot 2026-08-07 112540" src="https://github.com/user-attachments/assets/28d82a41-0f9f-4608-b767-2b74f5e05d2d" />

Restoring Version
<img width="1147" height="666" alt="Screenshot 2026-08-07 112622" src="https://github.com/user-attachments/assets/02beea1f-8344-462d-a2a0-df8022d0c056" />

## Lab 21 - Secure SharePoint File Sharing 

## Objective 
Provide another department with access to a specific Engineering document without granting unnecessary access to Engineering resources.

## Steps Performed
  - Selected the Engineering Change Procedure Text Document
  - Opened SharePoint sharing settings
  - Configured access for a specific organizational user
  - Assigned view only permissions with HR department
  - Verified access using Manage Access

### Result
Implemented least privilege access by granting access to the required document without adding the user to the Engineering Microsoft 365 Group.

### Screenshots

Sharing Document
<img width="909" height="294" alt="Screenshot 2026-08-07 113114" src="https://github.com/user-attachments/assets/08b33db8-47ad-4f98-b2df-6e127c15cb3b" />

Adding Permissions
<img width="301" height="249" alt="Screenshot 2026-08-07 113222" src="https://github.com/user-attachments/assets/f46407ac-f21d-4c49-819c-de19dc639f4f" />

Who Can View Shared Documents
<img width="575" height="409" alt="Screenshot 2026-08-07 113322" src="https://github.com/user-attachments/assets/0108af15-eb70-41e0-affe-e79fb3a198ae" />

Verifying Shared Document
<img width="445" height="510" alt="Screenshot 2026-08-07 113357" src="https://github.com/user-attachments/assets/027ac2c2-4de9-475f-97ca-515217ce234e" />

## Lab 22 - Manage SharePoint Site Ownership

## Objective
Provide the Engineering SharePoint environment with an additional owner

## Steps Performed
- Reviewed Engineering site membership
- Identified an existing Engineering member
- Promoted David Martinez from Member to Owner
- Verified multiple owners existed for the Engineering environment.

### Result
Reduced dependency on a single site owner and improved administrative continuity.

### Screenshots

Original Membership
<img width="379" height="752" alt="Screenshot 2026-08-07 113952" src="https://github.com/user-attachments/assets/69755969-455f-47fc-994a-826c1c99fe65" />

New Membership
<img width="385" height="370" alt="Screenshot 2026-08-07 114008" src="https://github.com/user-attachments/assets/da6d62fb-b406-4bd1-bd44-ac4196837b23" />

## Lab 23 - Create an HR Communication Site

## Objective
Create an employee-facing SharePoint portal for HR information

## Steps Performed
  - Opened the SharePoint Admin Center.
  - Created a new Communication Site
  - Selected the Department template
  - Created the Contoso HR Portal
  - Establish areas for: Company Announcements

 ### Result
 Created a centralized employee information portal designed for organizational communication rather than team collaboration.

 ### Screenshots

 SharePoint Admin Center
 <img width="1912" height="944" alt="Screenshot 2026-08-07 114231" src="https://github.com/user-attachments/assets/bc82970b-734f-4c53-b55c-1aadfe2ef0fd" />

Selecting Site Type
<img width="1241" height="746" alt="Screenshot 2026-08-07 114302" src="https://github.com/user-attachments/assets/4d0089bd-8ad4-4ab1-b60c-cca774c6afaa" />

Template Selection
<img width="1239" height="792" alt="Screenshot 2026-08-07 114409" src="https://github.com/user-attachments/assets/dc246b2b-8385-4234-af49-8f4cc62a4a96" />

Configuring Site
<img width="1240" height="794" alt="Screenshot 2026-08-07 114538" src="https://github.com/user-attachments/assets/40fd30a6-d5b7-48a3-a182-7b970fa5e336" />

Verify Site
<img width="1869" height="914" alt="Screenshot 2026-08-07 114714" src="https://github.com/user-attachments/assets/956dca73-0234-49bd-ae1c-b4f63f56c0cc" />

Creating Area for Company Announcements
<img width="1450" height="768" alt="Screenshot 2026-08-07 131440" src="https://github.com/user-attachments/assets/ceaab288-137e-45fb-a4c1-1420d2d39dad" />

Verifying Company Announcements
<img width="1665" height="813" alt="Screenshot 2026-08-07 131515" src="https://github.com/user-attachments/assets/76acad97-2b97-42f7-b149-2e6a7d3e2ea2" />


## Skills Learned
  - SharePoint Online Administration
  - SharePoint Team Sites
  - Communication Sites
  - Document Libraries
  - Document Management
  - SharePoint Permissions
  - Microsoft 365 Group Integration File Recovery
  - File Recovery
  - Version History
  - Secure File Sharing
  - Least-Privilege Access
  - Site Ownership Management
  - Microsoft Teams and SharePoint Integration

## Conclusion
These labs provided hands on experience administering SharePoint Online in a simulated enterprise Microsoft 365 environment.

The project covered the lifecycle of departmental content from creating document storage and configuring access to recovering deleted information, restoring precious version, securely sharing files, managing ownership, and provisioning an employee facing communication site

The environment also demonstrated the relationship between Microsoft 365, Groups, Microsoft Teams, and SharePoint Online, reinforcing how Microsoft 365 collaboration services operate together in an enterprise environment.

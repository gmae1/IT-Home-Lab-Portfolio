# Shadow Copies Previous Versions File Recovery

## Objectives
Configure Shadow Copies (Previous Versions) on Windows Server 2022 file server to provide rapid recovery of acciedentally deleted or overwritten files wiothout restoring an entire system backup.

## Why This Lab Matters
Accidental file deletion and file overwrites are common in enterprise environments. Shadow Copies allow administrators and users to quickly restore previous versions of files and folders from scheduled snapshots, signifcantly reducing recovery time and minimizing help desk workload.
Unlike traditional backups, Shadow Copies provide near-instant recovery for day to day file mistakes while complementing enterprise backup and disaster recovery strategies.

## Task Performed 
- Open Shadow Copies properties for the C: file
- Enabled Shadow Copies on the C: drive
- Reviewed storage allocation and snapshot scheduling settings
- configured the default storage location for snapchots
- created a initial manual snapshot
- Created a test file (Policies.txt) in the HR Department folder
- Generated a second manual snapshot after the file was created
- Modified the contents of the file tp simulate accidental overwritting
- Accessed the Previous Version tab
- Verified the availability previous snapshots
- Restored the Original Version of the file using Shadow Copies
- Confirmed successfl recovery of the orginal file contents.
- Made Schedule Shadow Coppies for M, T, W, Th, F at 9AM, 12PM & 5PM

## Screenshots 

C Drive Properties/ Shadow Copies
<img width="1024" height="768" alt="7 1CDrive_Prop" src="https://github.com/user-attachments/assets/e505d5d9-581f-42f2-b282-61c76dab3854" />
<img width="1024" height="768" alt="7 2Shadow_Coppies" src="https://github.com/user-attachments/assets/59a5d9d3-6847-461f-a37d-8973c29f7e51" />

Enable CDrive Shadow Copies
<img width="1024" height="768" alt="7 3Enable_CDrive" src="https://github.com/user-attachments/assets/0cf63fd1-becf-4453-91a0-1a59020f44f9" />

Created Snapshots
<img width="1024" height="768" alt="7 4Created_Snapshot" src="https://github.com/user-attachments/assets/3e672f28-cce7-4992-8735-932d0f5d3d75" />

Created Polocies.txt for HR Department
<img width="1024" height="768" alt="7 5HR_Polocies" src="https://github.com/user-attachments/assets/602c558f-3570-469b-9f03-7024710d44e7" />

Created another Snapshot
<img width="1024" height="768" alt="7 6Created_New_SC" src="https://github.com/user-attachments/assets/85d68327-0ead-403b-91d3-243eca95227c" />

Polocies.txt got Overwritten
<img width="1024" height="768" alt="7 7Redid_Text" src="https://github.com/user-attachments/assets/24297f19-5fd9-4439-9f37-4605dd6bbb81" />

Previous Polocies
<img width="1024" height="768" alt="7 8Previous_Version" src="https://github.com/user-attachments/assets/0bc77751-197b-4b00-a680-b149b67c73ae" />

Verify the Previous Text before Restoring
<img width="1024" height="768" alt="7 9Verify_Previous_Version" src="https://github.com/user-attachments/assets/690f4fcb-d11b-4b4c-bf6f-fb603fabab1b" />

Verify PRoper Restoration in Notepad
<img width="1024" height="768" alt="7 10Verfy_Restore_Proper" src="https://github.com/user-attachments/assets/b73c6136-11f0-4ece-9c84-5556c9f91948" />

Scheduled Shaddow Coppies
<img width="1024" height="768" alt="7 11Scheduled_ShadowCoppies" src="https://github.com/user-attachments/assets/500e3d5b-0962-4222-8669-5d190ff801c1" />

## Conclusion 
This lab demonstrated how Windows Server Shadow Copies provid rapid recovery of previous file versions through scheduled volume snapshots. Unlike traditional backups, Shadow Copies enable administrators and users to restore accidentally modified or deleted fiiles within seconds, improving operational effciency and reducing recovery time. This feature complements Windows Server Backup and DFS Replication by providing an additional layer of enterpruse file protection.

# Wireshark DNS Packet Analysis

## Objective
Capture and analyze DNS traffic to observe how domain names are translated into IP addresses

## Tools Used
- Windows 11
- VirtualBox
- Wireshark
- Command Prompt

## Task Performed

- Capture DNS traffic using Wireshark
- Applied DNS packet filters
- Generated DNS queries using nslookup
- Examined DNS query packets
- Identified DNS server communication
- Observed domain name resolution
- Analyzed query and response behavior

## Comands Used

### Windows

- nslookup google.com
- nslookup microsoft.com

### Wireshark Filter

- dns

## Screenshots

Wireshark Interface
<img width="1024" height="768" alt="4 1Wireshark_Interface_Selected" src="https://github.com/user-attachments/assets/6888524a-3073-4613-90ea-985ebfce74f9" />

DNS Filter
<img width="1024" height="768" alt="4 2DNS_Filter" src="https://github.com/user-attachments/assets/91e7b150-8a87-4b36-9257-8a09a222ed65" />

Nslookup Results
<img width="1024" height="768" alt="4 3nslookup_results" src="https://github.com/user-attachments/assets/e5358480-b7dc-42df-b1cf-7b31bbb45ceb" />

DNS Query Response
<img width="1024" height="768" alt="4 4dns_Query_Response" src="https://github.com/user-attachments/assets/220d19d6-d23e-49b9-9a89-37b74d3870a5" />

DNS Query Details
<img width="1024" height="768" alt="4 5DNS_Query_Details" src="https://github.com/user-attachments/assets/27aa4cbb-6cb9-4de0-8093-70080e73e138" />

DNS Response Details
<img width="1024" height="768" alt="4 6DNS_Response_Details" src="https://github.com/user-attachments/assets/68b55936-2c89-4759-9f82-6298b71cca8c" />

## What I Learned
- How DNS translates domain names into IP addresses
- How DNS queries and responses apper in packet caprutes
- How to identify DNS traffic using Wireshark
- How to analyze DNS request and response packets
- How DNS servers respond to client requests
- How UPD port 53 is commonly used for DNS communication
- How name resolution works before connecting to a website
- The role DNS plays in network troubleshooting

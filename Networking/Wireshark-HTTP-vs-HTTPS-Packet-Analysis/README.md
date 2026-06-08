# Wireshark HTTP vs HTTPS Packet Analysis

## Objective
Capture and compare HTTP and HTTPS traffic using wireshark to understand how encrypted traffic protects web communication

## Tools Used
- Windows 11
- VirtualBox
- Wireshark
- Microsoft Edge
- HTTP and HTTPS websites

## Task Performed
- Capture web traffic using Wireshark
- Generated HTTP traffic using a non-encrypted website
- Generated HTTPS traffic using encrypted website
- Applied HTTP and TLS packet filters
- Examined HTTP request and responses
- Observed TLS handshak
- Analyzed encrypted HTTPS traffic
- Compared readable HTTP traffic with encrypted HTTPS traffic

## Screenshots
Wireshark Interface
<img width="1024" height="768" alt="6 1Wireshark_Interface_Selcted" src="https://github.com/user-attachments/assets/3e6dafde-e37f-4d66-804e-c73188b59b55" />

HTTP Neverssl
<img width="1024" height="768" alt="6 2htttp_Neverssl" src="https://github.com/user-attachments/assets/074f4512-51ed-4687-85a0-2ebc63ddb32c" />

HTTP Packets
<img width="1024" height="768" alt="6 3Http_Packets" src="https://github.com/user-attachments/assets/ca7c1e4f-17bd-43b4-9c7f-f12b9dc15bcb" />

HTTP Stream Readable
<img width="1024" height="768" alt="6 4Http_Stream_Readable" src="https://github.com/user-attachments/assets/105749a4-0f1a-43f8-8c5d-325e4d706243" />

HTTPS Google
<img width="1024" height="768" alt="6 5HTTPS_Google" src="https://github.com/user-attachments/assets/e3958cec-d2a0-4345-895d-6adc172e5a20" />

HTTPS Packets
<img width="1024" height="768" alt="6 6Https_Packets" src="https://github.com/user-attachments/assets/22339af7-1caa-4378-bc8d-ec56d8976609" />

## WHat I Learned
- HTTP traffic is transmitted in clear text
- HTTPS traffic is encrypted using TLS
- HTTP commonly uses TCP port 80
- HTTPS commonly uses TCP poer 443
- TLS handshakes establish secure communication between client and server
- Client Hello and Server Hello message initiate encrypted sessions
- Encrypted traddic appers as Application Data in Wireshark
- Wireshark can identify encrypted traffic but cannot read protected contents
- HTTPS protects credentials, request and web content from being viewed by unathorized parties

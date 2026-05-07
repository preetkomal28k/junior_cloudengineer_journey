## OSI LAYER
The OSI (Open Systems Interconnection) model is a 7-layer framework that describes how data flows through a network. It standardizes network communication by breaking it into logical layers, making troubleshooting easier.

#### 🔹Purpose:

- Standardize network communication.
- Identify where network problems occur.
- Allow devices from different vendors to communicate.
 
### ⭐OSI Layer
-  Physical Layer - Cables, signals
- Data Link Layer - MAC addresses, frames
- Network Layer - IP addresses, routing
- Transport Layer - TCP/UDP, ports
- Session Layer - Conversation management( maintain session between the devices )
- Presentation Layer - Encryption, compression
- Application Layer - HTTP, FTP, SMTP

#### 🔹 layer1 - physical layer 
The Physical Layer handles the actual transmission of data through physical media.

Components:

- Cables (Fiber Optic, Copper)
- Connectors (RJ45, USB)
- Hubs
- Repeaters
- Network interface cards (NIC)
- Data Unit: Bits (0s and 1s)

Example: When you plug an ethernet cable into your computer, that's Layer 1.

 #### 🔹 Layer 2 - data link layer
 it is responsible for error-free transfer of frames between adjacent nodes using MAC addresses.

 *Key Components*

- Switches
- MAC addresses
- Frames

Protocols:

- Ethernet
- PPP (Point-to-Point Protocol)
- Frame Relay
Example: A switch uses MAC addresses to forward frames to the correct port.
```bash
CopySource MAC: AA:BB:CC:DD:EE:FF
Dest MAC: 11:22:33:44:55:66
```

#### 🔹 Layer 3 -  Network Layer  
 routes data between different networks using IP addresses.

*Key Functions:*

- Logical addressing (IP addresses)
- Routing
- Path determination
- Devices: Routers

Protocols: IP, ICMP, IGMP
```bash
Example - How routing works:

CopySource: 192.168.1.10 → Destination: 10.0.0.5

Router checks routing table:
10.0.0.0/24 → Forward via Interface 2

Data reaches destination!
```
Key Point: If a packet can't reach directly, router finds the best path.

#### 🔹 Layer 4 - Transport Layer 
 manages end-to-end communication between applications and provides reliable or unreliable data delivery.

Protocols: TCP, UDP, SCTP

*TCP (Transmission Control Protocol):*

- Connection-oriented.
- Reliable delivery.
- Slower but safe.
Uses: Email, Web, File Transfer.

*UDP (User Datagram Protocol):*

- Connectionless.
- Fast delivery.
- No reliability.
Uses: Video streaming, VoIP, Gaming.

#### 🔹 Layer 5 - Session Layer
 manages conversations (sessions) between applications.

*Functions:*

- Session establishment.
- Maintenance.
- Termination.
  
Examples:

- Login sessions.
- Database connections.
- Chat conversations.
Real-world example: When you log into Facebook, a session is created. When you logout, the session ends.


#### 🔹 Layer 6 -  Presentation Layer 
 prepares data for the Application Layer by handling formatting, encryption, and compression.

*Functions:*

- Translation: Convert data formats.
-  Encryption: Secure data (SSL/TLS).
- Compression: Reduce data size.
- 
Examples:

JPEG/PNG image compression.
SSL/TLS encryption for HTTPS.
ASCII to EBCDIC conversion.
Video codec (H.264).
Real example:

CopyPlain text: "Hello"
Encrypted: "x7K#mP@9w"
#### 🔹  Layer 7 - Application Layer
is where users and applications interact with the network.

*Protocols:*

- HTTP/HTTPS - Web browsing
- SMTP/POP3/IMAP - Email
- FTP - File transfer
- DNS - Domain name resolution
- Telnet/SSH - Remote access
DHCP - IP assignment
Example: When you open Google Chrome and visit a website, you're using the Application Layer (HTTP protocol).


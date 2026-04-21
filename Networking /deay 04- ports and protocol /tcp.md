##  What are Protocols?

Protocols are a set of rules that define how data is sent and received over a network.

 🔹Simple words:

*“Protocol = the rulebook of communication”* 

Examples:
HTTP → used to load web pages
HTTPS → secure web communication
FTP → file transfer
TCP → reliable data delivery


#### ⭐ What are Ports?

A port is a logical number (0–65535) used to identify a specific application or service running on a system.

🔹 Simple words:

“IP address tells which device, and Port tells which service inside that device”

```bash
some popular ports
Port 80 → HTTP
Port 443 → HTTPS
Port 22 → SSH

IP address = building address
Port = room number
```

## 🔹 What is TCP (Transmission Control Protocol)?

TCP is a connection-oriented protocol that ensures reliable data transmission. It operates at the Transport Layer of the OSI model.

🔑 Key Features of TCP
- Reliable Delivery → Retransmits data if it is lost
- Ordered Data → Data arrives in the correct sequence
- Error Checking → Detects corrupted packets
- Acknowledgement (ACK) → Receiver confirms data reception
- Flow Control (Windowing) → Prevents overwhelming the receiver
- Connection-Oriented → Connection is established before data transfer

#### ⭐ Three-Way Handshake (Connection Establishment)

Before data transfer, TCP uses a process called the three-way handshake:

#### Step 1: SYN

Client → Server
👉 “I want to start a connection”

#### Step 2: SYN-ACK

Server → Client
👉 “Request received, I’m ready”

#### Step 3: ACK

Client → Server
👉 “Connection confirmed, let’s start”

#### 🔁 Flow Representation
```bash
Client        Server
  | --- SYN ---> |
  | <--- SYN-ACK |
  | --- ACK ---> |
```
 Now the connection is established, and data transfer can begin.

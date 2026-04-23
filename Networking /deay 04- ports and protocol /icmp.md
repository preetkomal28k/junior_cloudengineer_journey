##  What is ICMP?

ICMP (Internet Control Message Protocol) is a network layer protocol used for error reporting and diagnostics in IP networks.
 It does not carry actual application data like TCP or UDP. Instead, it helps systems understand what’s happening inside the network.

#### ⭐ Why ICMP is Important?

ICMP acts like a network health checker:

- Detects if a host is reachable
- Reports errors in packet delivery
- Helps trace the path of packets
  
#### ⭐ ICMP Message Structure

An ICMP message consists of:

1. Type (1 byte)

Defines the type of message
Examples:

8 → Echo Request
0 → Echo Reply
3 → Destination Unreachable

2. Code (1 byte)

Provides additional information about the Type
Example:

Destination unreachable → network unreachable / port unreachable

3. Checksum (2 bytes)

Used for error detection in the message

4. Data Section

Depends on the message type:

Identifier
Sequence number
Optional payload

#### 🔹 Common ICMP Message Types
```bash
Type	  Name                          	Purpose
8	     Echo Request                   Sent by ping
0      Echo Reply	                   Response to ping
3	     Destination Unreachable	     Cannot reach destination
11	   Time Exceeded	             TTL expired (used in traceroute)
```

#### ⭐ How ICMP Works (Example)
Using Ping
ping google.com

🔁 Flow:

- Your system sends Echo Request
- Destination replies with Echo Reply
- If reply received → host is reachable

#### ⭐ Key Characteristics
- No reliability (no guarantee of delivery)
- No sequencing
- No error correction
- Fast and lightweight
- Used for diagnostics, not data transfer

####  ⭐ Famous Network Attacks

🔹 1. ICMP Flood (Ping Flood)
 ICMP based attack

- Attacker bohot saare ping requests bhejta hai
- Server overload ho jata hai
- Legit users access nahi kar paate
 Type:

DoS / DDoS

🔹 2. Ping of Death
 ICMP attack

- Oversized ya malformed packet bheja jata hai
- System crash ya hang ho sakta hai

 Old attack hai but concept important hai

## What is UDP?

UDP (User Datagram Protocol) is a connectionless transport layer protocol that sends data without establishing a connection between sender and receiver.
 It focuses on speed over reliability

#### ⭐ How UDP Works
- No handshake (no connection setup)
- Data is sent as independent packets called datagrams
- No acknowledgement (ACK) from receiver
- No guarantee of delivery or order
 
##### 🔹 What is a Datagram?

A datagram is a small unit of data that:

- Travels independently
- Contains source & destination info
- May arrive out of order or not at all

#### ⭐ Real-Life Use Cases
- Online Gaming
- Voice/Video Calls (VoIP)
- Live Streaming
- DNS Queries

#### ⭐ Key Features of UDP
- Fast transmission (Low latency)
- Lightweight (8-byte header)
- No reliability (packet loss possible)
- No retransmission
- No ordering guarantee
- Supports broadcast & multicast
- No congestion control

#### ⭐ Advantages
- Very fast communication
- Low overhead → better performance
- Ideal for real-time applications
  
#### ⭐ Disadvantages
No data delivery guarantee
Packets can be lost or duplicated
No error correction

#### ⭐ UDP vs TCP
Feature	       UDP            	TCP 
Connection  	Connectionless	  Connection-oriented
Speed	        Fast	            Slower
Reliability	  No guarantee     	Reliable
Ordering	    Not guaranteed	  Maintained
Use Case	    Streaming, Gaming	Banking, File Transfer

## What is an IP Address?

An IP (Internet Protocol) address is a unique number assigned to each device to communicate  on a network. Just like your house has an address so that people can find it,
in the same way, every computer or device has an IP address.

House address → helps people reach your home.
IP address → helps data reach your device.

#### 🔹It helps in:

Identifying devices
Sending and receiving data

Example:
`192.168.1.1`


#### ⭐ Why do we need IP Address?

Every device on a network needs a unique identity to communicate. Just like we use phone numbers to call someone .Computers use IP addresses to send and receive data

#### 🔹Without IP addresses:

Devices cannot find each other Internet communication will not work

#### ⭐ How does IP Address work?

##### When you access a website:

- You enter a domain name (e.g., google.com)
- DNS converts it into an IP address
- Your system sends a request to that IP
- Server responds back with data

This process happens in milliseconds.

 ### ⭐  IP Classes (Basic Understanding)
```bash  Class	Range	Use
Class A	1.x.x.x – 126.x.x.x	Large networks
Class B	128.x.x.x – 191.x.x.x	Medium networks
Class C	192.x.x.x – 223.x.x.x	Small networks
 ``` 

 Today, classes are less used, but important for basics.

### ⭐ Usage Types of IP Address
These define where the IP is used:
#### 1. Public IP

A Public IP address is an IP address that is assigned by an Internet Service Provider (ISP) and is accessible over the internet. It is unique across the whole world, so any device on the internet can communicate with it.

NOTE: Multiple devices in a local network share one public IP using NAT, while maintaining unique private IPs internally.

🔹 Example
`8.8.8.8`

This is a public IP used by Google DNS.

#### 2. Private IP
Private IP addresses are used within a local network and are not routable on the public internet.They are assigned to devices inside a network (like home, office, etc.).

🔹 Reserved Private IP Ranges
```bash
- 10.0.0.0 – 10.255.255.255 (Class A)
- 172.16.0.0 – 172.31.255.255 (Class B)
- 192.168.0.0 – 192.168.255.255 (Class C)
   ```




### ⭐ Technical Types of IP Address
These define the format and size of the IP:
#### 🔹 IPv4

Pv4 is the fourth version of the Internet Protocol used to identify devices and enable communication over a network. It is the most widely & common used IP addressing system.

### Structure of IP Address (IPv4)

~ An IPv4 address is 32 bits written in dotted decimal notation.

Example:
`192.168.1.1`

It consists of:

Total bits = 32 bits
Divided into 4 octets
Each octet = 8 bits
```bash Example Breakdown
192     .168     .1     .1
|        |       |      |
8 bits   8 bits  8 bits 8 bits
 ``` 

- Each octet value ranges from:
0 to 255

 🔹 Network and Host Portion

An IPv4 address is divided into:

Network part → identifies the network
Host part → identifies the device

Example:

192.168.1.0/24
/24 → first 24 bits = network
Remaining 8 bits = host

### ⭐ Subnet Mask
A subnet mask is a 32-bit number used in IPv4 to separate the network portion and host portion of an IP address.

#### 🔹 Structure
It is written in dotted decimal notation Consists of 4 octets (32 bits) Uses continuous 1s and 0s in binary
```bash 
Example:

255.255.255.0
📌 Binary Representation
11111111.11111111.11111111.00000000
1s → represent network bits
0s → represent host bits
 ```
🔹 Structure

 Example:

IP Address:     192.168.1.10
Subnet Mask:    255.255.255.0
Network part → 192.168.1
Host part → 10

### ⭐  CIDR Equivalent ( classless inter domain routing)

Subnet masks are often written in CIDR notation . It defines how much part of IP is network and how much is host.

Example:

192.168.1.0/24

 /24 means:First 24 bits = network
Remaining 8 bits = host

24 bits for network
Remaining for hosts

## ⭐ What is IPv6?

**IPv6 (Internet Protocol Version 6)** is the latest version of the Internet Protocol designed to replace IPv4.

* IPv4 uses **32-bit addressing** (~4.3 billion addresses)
* IPv6 uses **128-bit addressing** (~3.4 × 10³⁸ addresses)

 Example:
`2001:db8::1`


#### 🔹 Why IPv6?

IPv4 limitations led to the development of IPv6:

##### Problems with IPv4:

* Address exhaustion
* Dependence on NAT (Network Address Translation)
* Broadcast overhead
* Limited scalability

##### IPv6 Improvements:

* Massive address space
* End-to-end connectivity (no NAT required)
* Efficient routing and simplified headers
* Built-in support for IPSec
* No broadcast (uses multicast instead)

### 🔹 How IPv6 Works?

IPv6 provides **globally unique addresses** to devices, enabling direct communication across networks.

* Uses **hexadecimal notation**
* Addresses divided into **8 groups (16 bits each)**
* Supports hierarchical addressing for efficient routing

###  ⭐ SLAAC (Stateless Address Auto Configuration
**SLAAC** allows a device to automatically configure its own IPv6 address without a DHCP server.

####  SLAAC Process
1. **Router Advertisement (RA):**
   Router sends network prefix (e.g., `2001:db8::/64`)

2. **Address Generation:**
   Device combines:

   * Network prefix
   * Interface identifier (EUI-64 or random)

3. **Duplicate Address Detection (DAD):**
   Ensures the address is unique

 Result:
`2001:db8::abcd:1234`

### ⭐ Key Features of SLAAC:

* Stateless (no server tracking)
* Automatic configuration
* Plug-and-play networking

####  IPv6 Communication Types

##### 🔸 1. Unicast

* One-to-one communication
* Used for standard client-server traffic

##### 🔸 2. Multicast

* One-to-many (group communication)
* Replaces broadcast in IPv6
* Example: Neighbor Discovery

##### 🔸 3. Anycast

* One-to-nearest communication
* Same IP assigned to multiple devices
* Closest node responds
 


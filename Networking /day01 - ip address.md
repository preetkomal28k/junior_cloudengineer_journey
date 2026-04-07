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
``` Class	Range	Use
Class A	1.x.x.x – 126.x.x.x	Large networks
Class B	128.x.x.x – 191.x.x.x	Medium networks
Class C	192.x.x.x – 223.x.x.x	Small networks 

👉 Today, classes are less used, but important for basics.

### ⭐ Types of IP Address
#### 1. Public IP

A Public IP address is an IP address that is assigned by an Internet Service Provider (ISP) and is accessible over the internet. It is unique across the whole world, so any device on the internet can communicate with it.

NOTE: Multiple devices in a local network share one public IP using NAT, while maintaining unique private IPs internally.

🔹 Example
`8.8.8.8`

This is a public IP used by Google DNS.

#### 2. Private IP
Private IP addresses are used within a local network and are not routable on the public internet.They are assigned to devices inside a network (like home, office, etc.).

🔹 Reserved Private IP Ranges

`- 10.0.0.0 – 10.255.255.255 (Class A)`

`- 172.16.0.0 – 172.31.255.255 (Class B)`

`- 192.168.0.0 – 192.168.255.255 (Class C)`





🔹 IPv4 Explained

IPv4 is the most commonly used IP version.
### Structure of IP Address (IPv4)

~ An IPv4 address is written in dotted decimal notation.

Example:
`192.168.1.1`

It consists of:

4 parts called octets
Each octet = 8 bits
Total = 32 bits (4 × 8)
- Example Breakdown
192     .168     .1     .1
|        |       |      |
8 bits   8 bits  8 bits 8 bits

- Each octet value ranges from:

0 to 255
32-bit address
Written in 4 parts (octets)
Each part ranges from 0–255

Example:

192.168.1.1

👉 Structure:

Network part
Host part

This helps identify:

Network
Device inside the network
🔹 Basic Idea of Subnetting

Subnetting means dividing a network into smaller networks.

Why we use it:

Better management
Improved security
Efficient IP usage

👉 Example:
Instead of one big network, we create smaller ones.

🔹 CIDR (Basic)

CIDR = Classless Inter-Domain Routing

It defines how much part of IP is network and how much is host.

Example:

192.168.1.0/24

👉 /24 means:

24 bits for network
Remaining for hosts

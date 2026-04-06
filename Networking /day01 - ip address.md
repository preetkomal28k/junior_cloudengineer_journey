
## What is an IP Address?

An IP (Internet Protocol) address is a unique number assigned to each device to communicate  on a network.
Example:
`192.168.1.1`

👉 It helps in:

Identifying devices
Sending and receiving data

🔹 Why do we need IP Address?

Every device on a network needs a unique identity to communicate.

Just like we use phone numbers to call someone
Computers use IP addresses to send and receive data

👉 Without IP addresses:

Devices cannot find each other
Internet communication will not work
🔹 How does IP Address work?

When you access a website:

You enter a domain name (e.g., google.com)
DNS converts it into an IP address
Your system sends a request to that IP
Server responds back with data

👉 This process happens in milliseconds.

🔹 Types of IP Address
1. Public IP
Assigned by ISP
Used on the internet
Unique globally
2. Private IP
Used inside local network
Not accessible from internet
Example ranges:
192.168.x.x
10.x.x.x
172.16.x.x – 172.31.x.x
🔹 IP Classes (Basic Understanding)
Class	Range	Use
Class A	1.x.x.x – 126.x.x.x	Large networks
Class B	128.x.x.x – 191.x.x.x	Medium networks
Class C	192.x.x.x – 223.x.x.x	Small networks

👉 Today, classes are less used, but important for basics.

🔹 IPv4 Explained

IPv4 is the most commonly used IP version.

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

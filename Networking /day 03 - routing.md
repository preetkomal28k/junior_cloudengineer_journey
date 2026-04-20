
## What is Routing?

Routing is the process of forwarding data packets from one network to another using the best possible path. Whenever you open a website, send data, or access a server, routing ensures that your data reaches the correct destination.

   #### *NOTE: MULTI- Layer switch is also known as router*

  there is  default sattic route (*0.0.0.0/0*) if yo don't know where to go
#### ⭐ What is a Router?
A router is a network device that:

- Connects multiple networks
- Forwards packets based on IP addresses
- Decides the best path using a routing table

⭐ What is a Routing Table?

A routing table is a database inside a router that stores path information.
```bash
🔹 Routing Table Structure
Destination Network | Next Hop     | Interface  | Metric
192.168.1.0/24      | Direct       | eth0       |  0
10.0.0.0/8          | 192.168.1.1  | eth1       | 10
```
 The router checks this table to decide where to send packets.

#### ⭐ How Does a Router Get Routes? (3 Ways)
1️⃣ Directly Connected Routes

When a router interface is connected to a network, the route is automatically added.
Example:
Interface: 192.168.1.1/24

2️⃣ Static Routing
Routes are manually configured by the network administrator.
ip route add 10.0.0.0/8 via 192.168.1.1
✔️ Simple
❌ Not scalable for large networks

3️⃣ Dynamic Routing

Routers automatically exchange routing information using protocols.
Common protocols:
RIP
OSPF
BGP

✔️ Automatic updates
✔️ Best path selection

#### ⭐ How Routing Works (Step-by-Step)

- Packet arrives at router
- Router checks destination IP
- Looks into routing table
- Chooses best path (Longest Prefix Match)
- Forwards packet to next hop

 This process repeats until the packet reaches its destination.

#### ⭐ What is a Routing Loop? 

A routing loop occurs when a packet keeps circulating between routers and never reaches the destination.

🔹 Example
Router A → Router B  
Router B → Router A  

 Packet gets stuck in a loop 

🔹 Why Routing Loops Occur?
- Incorrect routing updates
- Slow convergence
-  Outdated routing information

####  ⭐   How to Prevent Routing Loops 🔥
✔️ Split Horizon

Prevents sending route information back on the same interface.

✔️ Poison Reverse

Marks a route as unreachable and sends it back.

✔️ TTL (Time To Live)

Limits packet lifetime so it doesn’t loop forever.

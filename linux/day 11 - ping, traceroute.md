## Day 10 – Ping and Traceroute

### What I did today
- Learned about **ping** command
- Practiced different ping options
- Learned about **traceroute**
- Understood how packets travel through the network

### Ping Command
Today I learned that **ping** is used to check network connectivity between two systems.

Ping works using **ICMP packets** and helps to:
- Check if a host is reachable
- Measure network latency
- Detect packet loss

### Ping Commands I Practiced
- `ping google.com`  
- `ping 8.8.8.8` 
- `ping -c 3 google.com`  
- `ping -i 2 google.com`  
- `ping -c 5 -q google.com`  
- `sudo ping -f google.com`  
- `ping -s 500 google.com`  
- `ping -w 10 google.com`  
- `ping -D www.google.com`  
- `ping -a google.com`  

### Traceroute
I also learned about **traceroute**, which shows the path packets take from my system to the destination.

What I understood:
- Each hop represents a router
- It helps identify network delays and failures

### Traceroute Commands I Learned
- `traceroute google.com  `
- `traceroute google.com 100  `
- `traceroute -q 1 google.com ` 
- `traceroute -p 21101 google.com  `
- `traceroute -4 google.com ` 
- `traceroute -6 google.com ` 
- `traceroute -g 192.168.42.45 google.com ` 

### What I learned
- Ping checks connectivity and latency
- Traceroute shows the network path
- Packet size, interval, and count can be controlled
- These tools are useful for network troubleshooting

### Challenges faced
- Remembering many ping options
- Understanding traceroute hops initially

### Tip
Networking tools feel complex at first.  
Practicing different options helps understand how networks actually work.
  
### Tomorrow’s plan
- Learn **Shell Scripting**

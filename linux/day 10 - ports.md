# Day 9 – Ports and Services

### What I did today
- Learned about **ports** in Linux  
- Understood how **services use ports** to communicate  
- Practiced checking **open ports** using commands  
- Connected **ports with services and processes**  
- Ran a **Flask application**, created **multiple routes**, and used **HTML templates**

### Ports in Linux.
**Ports** are **logical endpoints** used for communication over a network.  

**Key points I understood:**
- A port works together with an **IP address** to identify communication endpoints.  
- **Services listen** on specific ports to accept connections.  
- Only **one service** can listen on a port at a time.

**Common port examples:**

| Service | Port |
|---------|------|
| SSH     | 22   |
| HTTP    | 80   |
| HTTPS   | 443  |

### Commands I practiced
- `ss -tuln` → Shows **listening TCP and UDP ports**  
- `netstat -tuln` → Displays **open ports** and their **listening services**  

**Example workflow:**
```bash
ss -tuln
```
- Shows: LISTEN 0 128 0.0.0.0:22 ... 
   This means sshd is listening on port 22

### Ports and Services Relationship
Clear understanding:

Service → starts a process
Process → listens on a port
Client → connects to the service via that port

Example:
SSH service → sshd process → listens on port 22

### Flask Practice
- Ran a Flask application on port 5000
- Created multiple routes (like /, /about, /contact)
- Used HTML templates with render_template
- Observed that Flask starts a process and listens on the assigned port

### What I learned
- Ports are essential for service communication
- Checking open ports is important for troubleshooting
- Flask apps also demonstrate how services, processes, and ports are connected

### Challenges faced
Remembering common port numbers
Differentiating listening vs established connections

### Tip
Visualizing service → process → port flow makes ports easier to understand

### Tomorrow’s Plan
- Learn about IP addresses: ip a, hostname -I
- Perform ping tests to check connectivity
- Understand server identity in a network

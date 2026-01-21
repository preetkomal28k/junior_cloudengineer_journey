## Day 9 – Services and systemctl

### What I did today
- Learned about Linux services
- Understood the relationship between processes and services
- Practiced service management using `systemctl`
- Checked service status and behavior

### Services in Linux
Today I learned an important concept:

**“All services are processes, but all processes are not services.”**

What I understood:
- A **process** is any running program
- A **service** is a special type of process
- Services usually:
  - Run in the background
  - Start at boot
  - Are managed by `systemd`

### systemctl Commands I Learned
I practiced the following commands:

- `systemctl start service-name`  
  → Starts a service

- `systemctl stop service-name`  
  → Stops a running service

- `systemctl status service-name`  
  → Shows current service status

- `systemctl restart service-name`  
  → Restarts the service

- `systemctl is-enabled service-name`  
  → Checks if the service starts at boot

- `systemctl enable service-name`  
  → Enables service at boot time

- `systemctl disable service-name`  
  → Disables service from starting at boot

- `systemctl mask service-name`  
  → Completely blocks the service from starting

- `systemctl unmask service-name`  
  → Removes the block and allows service to start
  
-  `systemctl poweroff`
  → Used to safely shut down the system

- `systemctl reboot`
  → Used to restart the system

- `systemctl --show-type --socket`
  → Used to view socket-based units and understand socket-activated services


### What I learned
- Services are controlled using `systemctl`
- Enable/disable affects boot time behavior
- Masking a service is stronger than stopping it
- systemd manages services and daemon processes

### Challenges faced
- Remembering many systemctl commands
- Understanding the difference between stop, disable, and mask

### Tip
It’s okay if service commands feel overwhelming at first.
With repetition, they slowly start to make sense.

### Tomorrow’s plan
Learn about **ports** and how services use them
- Practice checking open ports using:
  - `ss -tuln`
  - `netstat`
- Run a **Flask application on port 5000**
- Understand how a service listens on a specific port


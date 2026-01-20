## Day 8 – Signals and Daemon Processes

### What I did today
- Learned about Linux signals
- Understood how processes are controlled using signals
- Learned about daemon processes
- Practiced basic process control commands

### Signals
Today I learned that **signals are used to communicate with processes**.

Some important signals I understood:
- SIGTERM → politely stop a process
- SIGKILL → forcefully kill a process
- SIGSTOP → pause a process
- SIGCONT → continue a stopped process

Commands I practiced:
- `kill PID`
- `kill -9 PID`

I understood that the `kill` command does not directly kill a process,  
it **sends a signal to the kernel**, and the kernel delivers it to the process.

### Daemon Processes
Daemon processes are programs that **run in the background**.
They usually start automatically when the system boots.

Examples I learned:
- sshd
- cron
- systemd

What I understood:
- Daemon processes do not need user interaction
- They keep running in the background
- They perform important system tasks

### What I learned
- Signals help control running processes
- SIGKILL should be used carefully
- Daemon processes are always running in the background
- Process control is handled by the kernel

### Challenges faced
- Remembering signal names was confusing
- Understanding the difference between killing and signaling a process

### Tip  
Repeated practice helps signals and process behavior make sense.

### Tomorrow’s plan
- Learn about **services management**
- Check SSH service status



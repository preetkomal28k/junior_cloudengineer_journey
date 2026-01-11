## Day 6 – Linux Processes (ps, top, kill – Basics)

### What I did today
- Learned what a process is in Linux
- Understood how programs run as processes
- Practiced viewing running processes
- Learned how to stop and manage processes

### Understanding Linux processes
Today I learned that a **process** is a running instance of a program.
Every command or application running in Linux has a process ID (PID).

Processes help Linux manage:
- CPU usage
- Memory usage
- Running programs

### Viewing processes using ps
I practiced using the `ps` command to see running processes.

Commands used:
```bash
ps
ps -e
ps aux
```
### What I understood:

- ps shows current shell processes
- ps -e shows all processes
- ps aux gives detailed information

### What I observed:

- Live CPU and memory usage
- List of running processes
- PID, user, and process state
I learned that top updates continuously and is useful for monitoring system performance.

### Killing a process
I practiced stopping processes using kill.

```bash
kill PID
kill -9 PID
```
### What I understood:

- kill PID sends a normal termination signal
- kill -9 PID forcefully stops a process
- Killing processes should be done carefully

Commands I practiced
- `ps`
- `ps -e`
- `ps aux`
- `top`
- `kill`
- `kill -9`
- `htop (basic understanding)`

### What I learned
- Processes represent running programs
- Each process has a PID
- top helps in live monitoring
- kill is used to stop unwanted processes

### Challenges faced
- Understanding process information output
- Identifying correct PID to kill
- Learning when to use kill -9

### Tip
Always try a normal kill before using kill -9.
Force killing processes can cause issues.

### Tomorrow’s plan
Practice background and foreground processes. 
Learn jobs, bg, and fg
Explore process priorities

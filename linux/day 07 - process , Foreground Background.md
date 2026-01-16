## Day 7 – Linux Process Types, Foreground and Background

### What I did today
- Learned about different types of processes in Linux
- Understood foreground and background processes
- Practiced running commands in background
- Learned how to manage running jobs

### Types of processes in Linux
Today I learned that Linux has different types of processes based on how they run.

Some common types:
- **Foreground processes** – run in the terminal and need user interaction
- **Background processes** – run without blocking the terminal
- **Daemon processes** – run in the background and provide services

Understanding process types helped me see how Linux manages tasks efficiently.

### Foreground processes
Foreground processes run directly in the terminal.

Example:
```bash
sleep 30
```
#### What I observed:

- The terminal is busy until the process finishes
- I cannot run another command until it ends

### Background processes
Background processes allow the terminal to stay free.

Example:

```bash
sleep 30 &
```
#### What I observed:

- The process runs in the background
- I can continue using the terminal
- Linux assigns a job number and PID

#### # Managing background jobs
I practiced managing jobs using these commands:

```bash
jobs
fg %1
bg %1
```
#### What I understood:

- jobs shows running background jobs
- fg brings a background job to the foreground
- bg resumes a stopped job in the background

### Stopping a process
I learned how to stop a running process:
- `Ctrl + C` – terminate foreground process
- `Ctrl + Z` – stop (pause) a process
This helped me control processes without killing them immediately.

### Commands I practiced
- `sleep`
- `jobs`
- `bg`
- `fg`
- `ps`
- `kill`

### What I learned

- Linux supports multiple process types
- Foreground and background processes improve multitasking
- Jobs help manage background tasks efficiently

### Challenges faced

- Remembering job numbers
- Understanding when a process is stopped vs running
- Switching between foreground and background
  
### Tomorrow’s plan
- Learn about daemon processes
- Practice process signals
- Explore /proc for process details

### Tip
Use background processes to save time, but always monitor them.
Understanding process control makes Linux easier to manage.

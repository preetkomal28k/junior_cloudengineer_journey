## Day 3 – Linux Permissions, Ownership, and Bandit Practice

### What I did today
- Learned about Linux file permissions and ownership
- Understood how Linux controls access using users and groups
- Practiced viewing and changing permissions
- Continued solving the Bandit wargame up to level 12
- Applied Linux commands while solving real challenges

### Linux permissions
Today I learned that Linux uses permissions to control who can access files and directories.

There are three permission types:
- **r (read)** – read file or list directory contents
- **w (write)** – modify file or create/delete files
- **x (execute)** – run a file or enter a directory

Permissions are assigned to:
- User (owner)
- Group
- Others

### Ownership in Linux
Each file has an **owner** and a **group**.
This helps Linux manage access in multi-user systems.

Commands used:
```bash
ls -l
chown user file.txt
chgrp group file.txt
```
### Bandit wargame progress
- Connected to Bandit using SSH
- Solved Bandit levels from level 0 to level 12
- Learned how passwords are hidden in:
- Readable files
- Files with special characters
- Hidden files
- Compressed files

Practiced extracting and reading files using Linux commands

### Commands I practiced
`ls`
`ls -l`
`cd`
`cat`
`pwd`
`ssh`
`file`
`find`
`grep`
`chmod`
`tar`
`gzip`
`bzip2`
`xxd`

### What I learned 
- Permissions and ownership control file security
- Bandit improves command-line confidence
- Linux skills improve faster with hands-on challenges
- Understanding file types is very important in Linux
  
### Challenges faced

- Understanding permission symbols and numbers
- Identifying correct files among many files
- Extracting multiple compressed files
- Remembering commands and paths

### Tips
Don’t memorize commands blindly.
Use them daily and understand why they work.

### Tomorrow’s plan

-Practice more permission-related commands
-Learn about special permissions (setuid, setgid, sticky bit)
-Solve more Bandit levels
-Revise users and groups concepts




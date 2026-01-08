## Day 4 – Changing Ownership, setuid, and setgid (Practice-Based)

### What I did today
- Practiced changing file and directory ownership
- Learned how `setuid` and `setgid` work in Linux
- Understood why special permissions are needed
- Tested permissions using real files and users
- Practiced commands multiple times to reduce confusion

### Changing ownership in Linux
Today I practiced changing the **owner** and **group** of files.

Commands used:
```bash
chown user file.txt
chown user:group file.txt
chgrp group file.txt
  ```
  
### What I understood:
- chown changes ownership
- chgrp changes only the group
- Ownership affects who can control the file

#### Why ownership matters

- Ownership is important because
- Only the owner or root can change permissions
- Applications run with specific user access
- It improves security in multi-user systems

### Practice I did

- Created files and directories
- Changed ownership using chown
- Applied setuid and setgid
- Checked permissions using ls -l
- Observed permission behavior changes
- Practicing helped reduce confusion.

### Commands I practiced

- `chown`
- `chgrp`
- `chmod`
- `ls -l`
- `id`
- `groups`

### What I learned

- Ownership controls file authority
- setuid and setgid are special permissions
- These permissions are powerful and must be used carefully
- Practice is essential to understand permission behavior

### Challenges faced

- Understanding when to use setuid vs setgid
- Interpreting permission output correctly
- Remembering where s appears in permissions

### Tip

Don’t try to memorize special permissions.
Create test files and observe permission changes to understand them better.

### Tomorrow’s plan

- Learn about sticky bit
- Practice permissions on directories
- Solve more Bandit levels related to permissions
- Learn about Linux processes and how they work
- Understand running processes using /proc
- Practice process-related commands (ps, top, htop)




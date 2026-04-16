## What are Looping Statements?

Looping statements allow a program to execute a block of code repeatedly based on a condition or sequence.
 They are essential for:
- Automation
- Iteration over data
- Reducing code redundancy
  
### ⭐ Types of Looping Statements in Python
#####  1. for Statement
 Used when the number of iterations is known (fixed).

```bash
 Syntax:
for variable in range:
    # code block
 Example:
for i in range(5):
    print(i)

✔ Output:

0
1
2
3
4
```
##### 2. while Statement

 Used when the number of iterations depends on a condition
```bash
 Syntax:
while condition:
    # code block
 Example:
i = 1

while i <= 5:
    print(i)
    i += 1

✔ Output:

1
2
3
4
5
```
 ### ⭐ Loop Control Statements

These statements control the execution flow inside loops.

#### 1. break Statement

 Terminates the loop immediately
```bash
for i in range(5):
    if i == 3:
        break
    print(i)

✔ Output:

0
1
2
```

####  2. continue Statement

 Skips the current iteration and moves to the next
```bash
for i in range(5):
    if i == 2:
        continue
    print(i)

✔ Output:

0
1
3
4
```
#### 3. pass Statement

 Does nothing (placeholder)
```bash
for i in range(3):
    pass
```
 Used when a statement is syntactically required but no action is needed

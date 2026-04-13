## What are Conditional Statements?

Conditional statements allow a program to make decisions based on conditions. They control the flow of execution using Boolean expressions (True / False).

#### Use's case
we use conditional statement for automation , decision making ,monitoring system , handling deployment , scaling infrastructure , security check up .
### ⭐ Types of conditional statement .
##### 🔸 1. if Statement

Executes code only if condition is true
```bash
 Syntax:
if condition:
    # code block
💡 Example (Age Check)
age = 18
if age >= 18:
    print("You are an adult")
✔ Output:
You are an adult
```

##### 🔸 2. if-else Statement

 Executes one block if condition is true, otherwise another block
```bash
 Syntax:
if condition:
    # if block
else:
    # else block
💡 Example (Adult or Minor)
age = 16
if age >= 18:
    print("You are an adult")
else:
    print("You are a minor")
✔ Output:
You are a minor
```
##### 🔸 3. if-elif-else Statement

 Used when multiple conditions are checked
```bash
 Syntax:
if condition1:
    # block 1
elif condition2:
    # block 2
else:
    # default block
💡 Example (Days of Week)
day = input("enter your day")
if day == "Monday" or day == "tuesday" :
    print("Start of the week")
elif day == "Wednesday" or day == "thrusaday" :
    print("Midweek")
elif day == "Saturday" or day == "Sunday":
    print("Weekend")
else:
    print("spa day")
```

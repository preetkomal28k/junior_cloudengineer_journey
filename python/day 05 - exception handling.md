## Exception Handling

When you write a Python program, sometimes it crashes because of errors. Exception handling helps you handle those errors safely so your program doesn’t stop suddenly.

#### 🔹 Simple Example (Real Life)

Imagine you are using an app:
You enter wrong password ❌
App shows: "Wrong password, try again" ✅

🔹 It doesn’t crash — it handles the error.
That’s exactly what exception handling does in Python.

#### ⭐ Errors vs Exceptions (Easy Way)
##### 🔹 Errors

- Mistakes in code
- Program won’t run
- print("Hello)
🔹  Missing quote → Syntax Error

🔹 Exceptions

- Happen while program is running
- Can be handled
- (10 / 0)

🔹 This gives error during execution

#### ⭐ Common Exceptions (Simple Examples)
##### 1. ValueError
```bash
try:
    num = int("abc")
except ValueError:
    print("Please enter a number!")
```
- When input is wrong

##### 2. ZeroDivisionError
```bash
try:
    result = 10 / 0
except ZeroDivisionError:
    print("Cannot divide by zero!")
```
##### 3. TypeError
```bash
try:
    print("Hello" + 5)
except TypeError:
    print("Wrong data types!")
```
##### 4. NameError
```bash
try:
    print(x)
except NameError:
    print("Variable not defined!")
```
##### 5. IndexError
```bash
try:
    my_list = [1, 2, 3]
    print(my_list[5])
except IndexError:
    print("Index out of range!")
```
#### ⭐ try-except (Main Concept)
🔹 Basic Syntax
```bash
try:
    # risky code
except:
    # handle error
```
🔹 Example
```bash
try:
    age = int(input("Enter age: "))
    print(age)
except:
    print("Invalid input!")
```
#### ⭐ How It Works
- Python runs try block
- If error comes → goes to except 
- Error handled
- Program continues

## *write a code to print the files in a folder using exception handling*
```bash 
import os

files_list   = input("enter the files  :").split()  

for files in files_list:  


    try :
     files1 = os.listdir(files)
     print  (f"===the list of files for the folder " + files)
     for file in files1:
      print(file)

    except FileNotFoundError:
     print("please  enter valid folder name ")

    except PermissionError:
      print("you dont have permisssion for this folder")
```

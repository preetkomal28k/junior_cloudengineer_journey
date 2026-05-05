## Exception Handling

When you write a Python program, sometimes it crashes because of errors. Exception handling helps you handle those errors safely so your program doesn’t stop suddenly.

#### 🔹 Simple Example (Real Life)

Imagine you are using an app:

You enter wrong password ❌
App shows: "Wrong password, try again" ✅

🔹 It doesn’t crash — it handles the error.
That’s exactly what exception handling does in Python.

#### Errors vs Exceptions (Easy Way)
##### 🔹 Errors
```bash
Mistakes in code
Program won’t run
print("Hello
```
-  Missing quote → Syntax Error

🔹 Exceptions
```bash
Happen while program is running
Can be handled
10 / 0
```
🔹 This gives error during execution

#### 🔥 Common Exceptions (Simple Examples)
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
🧠 try-except (Main Concept)
🔹 Basic Syntax
try:
    # risky code
except:
    # handle error
🔹 Example
try:
    age = int(input("Enter age: "))
    print(age)
except:
    print("Invalid input!")
🔹 How It Works
Python runs try block
If error comes → goes to except
Error handled
Program continues

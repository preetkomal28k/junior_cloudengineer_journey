## What is a List?

A list is a fundamental data structure in programming that allows you to store a collection of items in a single variable. Lists are:
- Ordered
- Mutable (can be changed)
- Can store multiple data types (integers, strings, objects, etc.)
```bash
my_list = [1, 2, 3, 'apple', 'banana']
```
### ⭐ list function 
#### 🔢 List Indexing

Each element in a list has an index, starting from 0.
```bash
first_element = my_list[0] 
# Output: 1
```
 Index starts from 0, not 1

#### 📏 List Length

You can find the number of elements in a list using len():
```bash
list_length = len(my_list)
 # Output: 5
```
#### ⭐ List Operations

#### ➕ Append , insert , extend (Add Element)

*append* Adds an element to the end of the list
*inset* add an elemnt according to index
*extend* add multiple value

```bash
my_list.append(4)
my_list.insert(5,6) # 5 index 6 value
my_list.extend(,y_list2)
print(my_list)
```
#### ❌ Remove ,pop , pop() , clear (Delete Element)

*remove* Removes a specific value
*pop* remove last element
*pop()* remove with index
*clear* clear everything
```bash
my_list.remove('apple')
my_list.pop
my_list.pop(0)
my_list.clear
```
#### ✂️ Slicing

Extract a portion of the list:
```bash
subset = my_list[1:4]  # Index 1 to 3
```
#### 🔗 Concatenation

Combine two lists:
```bash
new_list = my_list + [5, 6]
```
#### 🔃 Sorting

Sort list elements:
```bash
my_list.sort()  # Ascending order
```
🔍 Check Element Exists

Check if an item is present:
```bash
list_of_student =(3,2, 4,5, 1)
is_present = 1 in list_of_student
print(is_present)

#output= true
```
## What is a Tuple?

A tuple is a data structure similar to a list, but with one key difference
 Tuples are immutable (cannot be changed after creation)

- Ordered
- Immutable
- Allows multiple data types
```bash 
my_tuple = (10, 20, 'cat', 'dog')
```
#### 🔢 Tuple Indexing

Access elements using index (starts from 0):
```bash 
my_tuple = (10, 20, 'cat', 'dog')
value = my_tuple[2]
print(value)
 # Output: cat
```
##### 📏 Tuple Length
```bash 
my_tuple = (10, 20, 'cat', 'dog')
length = len(my_tuple)
print(length)
 # Output: 4
```
#### ⚙️ Common Tuple Operations

⭐ Access Element
```bash 
my_tuple = (5, 15, 25)
element = my_tuple[1]
print(element) 
# Output: 15
```
⭐ Tuple Packing & Unpacking
```bash 
point = (7, 9)
x, y = point
print(x, y)
 # Output: 7 9
```
⭐ Concatenation
```bash 
t1 = (1, 2)
t2 = (3, 4)
print(t1 + t2)
  # Output: (1, 2, 3, 4)
```
⭐ Check Element Exists
```bash 
my_tuple = ('red', 'blue', 'green')
result = 'blue' in my_tuple
print(result)
 # Output: True
```
⭐ Multiple Return Values (Function)
def get_values():
    return (100, 200)

a, b = get_values()
print(a, b)  # Output: 100 200

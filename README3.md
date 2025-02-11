**Chapter 3: Python Program Flow Control**

### 1. Conditional Blocks
#### if…else Statement
```python
x = 10
if x > 5:
    print("x is greater than 5")
else:
    print("x is not greater than 5")
```

#### if…elif…else Statement
```python
num = 10
if num > 0:
    print("Positive number")
elif num == 0:
    print("Zero")
else:
    print("Negative number")
```

#### Nested if Statement
```python
x = 15
if x > 10:
    print("Above 10")
    if x > 20:
        print("Also above 20")
    else:
        print("Not above 20")
```

### 2. Use of while Loops
```python
count = 0
while count < 5:
    print(count)
    count += 1
```

### 3. Loop Manipulation: continue, break
```python
for i in range(5):
    if i == 3:
        break  # Exits loop at i == 3
    print(i)
```
```python
for i in range(5):
    if i == 3:
        continue  # Skips iteration at i == 3
    print(i)
```

### 4. For Loop Using Ranges
```python
for i in range(1, 6):
    print(i)
```

### 5. Nested Loops
```python
for i in range(3):
    for j in range(2):
        print(f"i: {i}, j: {j}")
```

---

**Chapter 4: Python Functions**

### 1. Built-in Functions & Commonly Used Modules
```python
print(len("Hello"))  # Built-in function
import math
print(math.sqrt(16))  # Module function
```

### 2. Function Definition and Calling
```python
def greet(name):
    print(f"Hello, {name}!")

greet("Alice")
```

### 3. The return Statement
```python
def square(num):
    return num * num

print(square(4))
```

### 4. Void Function
```python
def print_message():
    print("This is a void function")

print_message()
```

---

**Chapter 5: Strings**

### 1. Creating and Storing Strings
```python
s = "Hello, Python!"
print(s)
```

### 2. Basic String Operations
```python
s1 = "Hello"
s2 = "World"
print(s1 + " " + s2)  # Concatenation
print(s1 * 3)  # Repetition
```

### 3. Accessing Characters by Index
```python
s = "Python"
print(s[0])  # First character
print(s[-1])  # Last character
```

### 4. String Slicing & Joining
```python
s = "Hello, World!"
print(s[0:5])  # Slicing
words = ["Python", "is", "fun"]
print(" ".join(words))  # Joining
```

### 5. String Methods
```python
s = " python programming "
print(s.upper())  # Uppercase
print(s.strip())  # Removing spaces
print(s.replace("python", "Java"))  # Replacing
```


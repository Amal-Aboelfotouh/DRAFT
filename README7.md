# Intermediate Python Concepts

## 1. List Comprehensions
List comprehensions provide a concise way to create lists.

```python
numbers = [x for x in range(10) if x % 2 == 0]
print(numbers)
```

**Output:**
```
[0, 2, 4, 6, 8]
```

---

## 2. Lambda Functions
Lambda functions are small, anonymous functions.

```python
square = lambda x: x * x
print(square(5))
```

**Output:**
```
25
```

---

## 3. Map, Filter, and Reduce

### **Map:** Applies a function to all items in an iterable.
```python
double = list(map(lambda x: x * 2, [1, 2, 3, 4]))
print(double)
```
**Output:**
```
[2, 4, 6, 8]
```

### **Filter:** Filters elements based on a condition.
```python
even_numbers = list(filter(lambda x: x % 2 == 0, [1, 2, 3, 4, 5]))
print(even_numbers)
```
**Output:**
```
[2, 4]
```

### **Reduce:** Performs a rolling computation on a list.
```python
from functools import reduce
sum_numbers = reduce(lambda x, y: x + y, [1, 2, 3, 4])
print(sum_numbers)
```
**Output:**
```
10
```

---

## 4. Exception Handling
Exception handling prevents crashes by catching errors.

```python
try:
    result = 10 / 0
except ZeroDivisionError:
    print("Cannot divide by zero!")
finally:
    print("Execution completed.")
```

**Output:**
```
Cannot divide by zero!
Execution completed.
```

---

## 5. File Handling
Reading and writing files in Python.

### **Writing to a File:**
```python
with open("example.txt", "w") as file:
    file.write("Hello, World!")
```

### **Reading from a File:**
```python
with open("example.txt", "r") as file:
    content = file.read()
    print(content)
```
**Output:**
```
Hello, World!
```

---

## 6. Working with JSON
Handling JSON data in Python.

```python
import json

person = {"name": "Alice", "age": 25}
json_data = json.dumps(person)
print(json_data)
```

**Output:**
```
{"name": "Alice", "age": 25}
```

---

## 7. Using `args` and `kwargs`

### **Using `*args`:**
```python
def add_numbers(*args):
    return sum(args)

print(add_numbers(1, 2, 3, 4))
```
**Output:**
```
10
```

### **Using `**kwargs`:**
```python
def print_info(**kwargs):
    for key, value in kwargs.items():
        print(f"{key}: {value}")

print_info(name="Alice", age=25)
```
**Output:**
```
name: Alice
age: 25
```

---

## 8. Enumerate and Zip

### **Enumerate:** Gets index and value while iterating.
```python
names = ["Alice", "Bob", "Charlie"]
for index, name in enumerate(names):
    print(index, name)
```
**Output:**
```
0 Alice
1 Bob
2 Charlie
```

### **Zip:** Combines two lists element-wise.
```python
names = ["Alice", "Bob"]
ages = [25, 30]
for name, age in zip(names, ages):
    print(f"{name} is {age} years old")
```
**Output:**
```
Alice is 25 years old
Bob is 30 years old
```

---

This `README.md` file explains intermediate Python concepts with examples. Feel free to extend it! 🚀

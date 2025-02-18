# Advanced Concepts in Python

## 1. Decorators
### What are Decorators?
Decorators in Python are functions that modify the behavior of other functions or methods. They are commonly used for logging, enforcing access control, instrumentation, caching, and more.

### Example:
```python
def decorator_function(original_function):
    def wrapper_function():
        print(f'Wrapper executed before {original_function.__name__}')  # Before execution message
        return original_function()  # Call the original function
    return wrapper_function

@decorator_function  # Applying decorator

def display():
    print('Display function executed')

display()
```

---

## 2. Generators
### What are Generators?
Generators are iterators that yield values lazily, meaning they generate values on the fly and do not store them in memory.

### Example:
```python
def count_up_to(max):
    count = 1
    while count <= max:
        yield count  # Yielding value instead of returning
        count += 1

counter = count_up_to(5)
for num in counter:
    print(num)  # Printing each yielded value
```

---

## 3. Context Managers
### What are Context Managers?
Context managers simplify resource management, like handling files or database connections, ensuring that resources are properly released after use.

### Example:
```python
with open("example.txt", "w") as file:  # Open file in write mode
    file.write("Hello, World!")  # Writing data to file
# File automatically closes after the 'with' block
```

---

## 4. Metaclasses
### What are Metaclasses?
Metaclasses define the behavior of classes in Python. They allow customization of class creation.

### Example:
```python
class Meta(type):
    def __new__(cls, name, bases, class_dict):
        print(f'Creating class {name}')  # Logs class creation
        return super().__new__(cls, name, bases, class_dict)

class MyClass(metaclass=Meta):  # Using a metaclass
    pass
```

---

##5. Asynchronous Programming (async/await)
### What is Asynchronous Programming?
Asynchronous programming allows execution of tasks without waiting for the previous task to finish.

### Example:
```python
import asyncio

async def hello():
    await asyncio.sleep(1)  # Simulate a delay
    print("Hello, World!")

asyncio.run(hello())  # Run async function
```

---

## 6. Function Overloading with `singledispatch`
### What is Function Overloading?
Python doesn’t support traditional function overloading, but `functools.singledispatch` can achieve similar behavior.

### Example:
```python
from functools import singledispatch

@singledispatch

def process(data):
    print("Default processing")  # Default case

@process.register(int)  # Register int type

def _(data):
    print(f"Processing integer: {data}")

@process.register(str)  # Register string type

def _(data):
    print(f"Processing string: {data}")

process(42)  # Calls integer-specific function
process("hello")  # Calls string-specific function
```

---

## 7. Property Decorators
### What are Property Decorators?
They allow us to define methods that behave like attributes.

### Example:
```python
class Person:
    def __init__(self, name):
        self._name = name  # Private attribute

    @property
    def name(self):
        return self._name  # Getter method

person = Person("Alice")
print(person.name)  # Accessing property as an attribute
```

---

## 8. Reflection and Introspection
### What is Reflection?
Reflection allows inspection of object attributes and methods at runtime.

### Example:
```python
class Sample:
    def method(self):
        pass

obj = Sample()
print(dir(obj))  # Lists all attributes and methods
```

---

## 9. Monkey Patching
### What is Monkey Patching?
Monkey patching allows modifying or extending code at runtime.

### Example:
```python
class A:
    def method(self):
        return "Original Method"

def patched_method(self):
    return "Patched Method"  # New method replacing the original

A.method = patched_method  # Applying monkey patch
obj = A()
print(obj.method())  # Output: Patched Method
```

---

This guide covers advanced Python topics with detailed explanations and examples for better understanding.

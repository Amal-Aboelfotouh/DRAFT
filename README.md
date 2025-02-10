# DRAFT

**Chapter 1: Introduction to Python 3.x**

## 1. Installation and Working with Python
To get started with Python, you need to install it on your system.

### Installation Steps:
1. Download Python from the official website: [https://www.python.org](https://www.python.org)
2. Install the downloaded package and ensure you select "Add Python to PATH".
3. Open a terminal or command prompt and type:
   ```sh
   python --version
   ```
   If Python is installed correctly, it will display the installed version.
4. You can start the Python interactive shell by typing:
   ```sh
   python
   ```

## 2. Python Identifiers, Keywords, Statements, and Expressions
### Identifiers:
Identifiers are the names used for variables, functions, classes, etc.
- Must begin with a letter (A-Z or a-z) or an underscore (_)
- Cannot be a keyword
- Cannot contain special characters like @, $, %

Example:
```python
my_variable = 10
print(my_variable)
```

### Keywords:
Keywords are reserved words in Python.
Example of some keywords:
```python
import keyword
print(keyword.kwlist)
```

### Statements and Expressions:
A statement is an instruction executed by Python, and an expression is a combination of values and operators that evaluates to a value.
```python
x = 5 + 3  # Expression
print(x)  # Statement
```

## 3. Operators, Precedence, and Associativity
### Operators:
Python supports arithmetic, comparison, logical, bitwise, assignment, and special operators.
```python
a = 10
b = 5
print(a + b, a - b, a * b, a / b)  # Arithmetic operators
print(a > b, a == b, a != b)  # Comparison operators
```

### Precedence and Associativity:
- Multiplication (*) has higher precedence than addition (+).
- Operators with the same precedence follow left-to-right associativity.
```python
result = 10 + 5 * 2
print(result)  # 20 because * has higher precedence than +
```

## 4. Reading Input, Printing Output, Type Conversions
### Reading Input:
```python
name = input("Enter your name: ")
print("Hello,", name)
```

### Printing Output:
```python
age = 25
print(f"I am {age} years old")
```

### Type Conversions:
```python
num_str = "100"
num_int = int(num_str)
print(num_int, type(num_int))
```

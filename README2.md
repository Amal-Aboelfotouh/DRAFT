**Chapter 2: Python Data Types (cont.)**

## 1. Using String Data Type and String Operations
Strings in Python are sequences of characters enclosed in quotes.

### Defining Strings:
```python
string1 = "Hello, World!"
string2 = 'Python Programming'
print(string1)
print(string2)
```

### String Operations:
```python
# Concatenation
str1 = "Hello"
str2 = " Python"
result = str1 + str2
print(result)  # Output: Hello Python

# Repetition
print(str1 * 3)  # Output: HelloHelloHello

# Indexing
print(str1[1])  # Output: e

# Slicing
print(str1[1:4])  # Output: ell
```

### String Methods:
```python
s = "python programming"
print(s.upper())  # Convert to uppercase
print(s.lower())  # Convert to lowercase
print(s.replace("python", "Java"))  # Replace substring
```

## 2. Defining List and List Slicing
Lists are ordered, mutable collections of items.

### Defining Lists:
```python
my_list = [10, 20, 30, 40, 50]
print(my_list)
```

### List Operations:
```python
# Accessing elements
print(my_list[0])  # Output: 10
print(my_list[-1])  # Output: 50

# Slicing
print(my_list[1:4])  # Output: [20, 30, 40]

# Modifying Lists
my_list.append(60)
print(my_list)  # Output: [10, 20, 30, 40, 50, 60]

my_list[2] = 35
print(my_list)  # Output: [10, 20, 35, 40, 50, 60]
```

## 3. Use of Tuple Data Type
Tuples are immutable sequences in Python.

### Defining Tuples:
```python
tuple1 = (1, 2, 3, 4, 5)
print(tuple1)
```

### Accessing Tuple Elements:
```python
print(tuple1[0])  # Output: 1
print(tuple1[-1])  # Output: 5
```

### Tuple Operations:
```python
# Concatenation
new_tuple = tuple1 + (6, 7, 8)
print(new_tuple)  # Output: (1, 2, 3, 4, 5, 6, 7, 8)

# Repetition
print(tuple1 * 2)  # Output: (1, 2, 3, 4, 5, 1, 2, 3, 4, 5)
```

Tuples are useful for storing data that should not be modified after creation.

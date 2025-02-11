**Chapter 6: Lists, Tuples, Sets, and Dictionaries**

### 1. Lists

#### Creating Lists

```python
my_list = [1, 2, 3, 4, 5]
print(my_list)
```

#### Basic List Operations

```python
my_list.append(6)  # Adding an element
my_list.remove(2)  # Removing an element
print(len(my_list))  # Length of the list
```

#### Indexing and Slicing in Lists

```python
print(my_list[0])  # First element
print(my_list[-1])  # Last element
print(my_list[1:4])  # Slicing
```

#### Built-In Functions Used on Lists

```python
print(sum(my_list))  # Sum of elements
print(sorted(my_list))  # Sorting a list
```

### 2. Dictionaries

#### Creating Dictionary

```python
my_dict = {"name": "Alice", "age": 25}
print(my_dict)
```

#### Accessing and Modifying Key-Value Pairs

```python
print(my_dict["name"])  # Access value
my_dict["age"] = 26  # Modify value
```

#### Built-In Functions Used on Dictionaries

```python
print(my_dict.keys())  # Get all keys
print(my_dict.values())  # Get all values
```

---

**Chapter 7: Files**

### 1. Types of Files, Creating Files

```python
with open("example.txt", "w") as file:
    file.write("Hello, this is a test file.")
```

### 2. Understanding Read Functions

```python
with open("example.txt", "r") as file:
    content = file.read()
    print(content)
```

#### readline() and readlines()

```python
with open("example.txt", "r") as file:
    print(file.readline())  # Reads one line
    print(file.readlines())  # Reads all lines as a list
```

### 3. Write Data into Files

```python
with open("example.txt", "a") as file:
    file.write("\nAppending new content.")
```


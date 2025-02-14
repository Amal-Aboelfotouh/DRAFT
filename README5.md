# 100+ Python Challenging Programming Exercises

## 1. Level Description

| Level  | Description |
|--------|------------|
| Level 1 | Beginner: Someone who has just gone through an introductory Python course. Can solve problems using 1 or 2 Python classes or functions. Solutions are typically found in textbooks. |
| Level 2 | Intermediate: Someone who has learned Python and has a strong programming background. Can solve problems using multiple classes or functions, and solutions are not directly found in textbooks. |
| Level 3 | Advanced: Can solve complex problems using rich libraries, data structures, and algorithms, employing Python standard packages and advanced techniques. |

---

## 2. Problem Template

```
#----------------------------------------#
Question
Hints
Solution
```

---

## 3. Questions

### Question 1 (Level 1)

**Question:**
Write a program to find all numbers divisible by 7 but not multiples of 5, between 2000 and 3200 (both included). The numbers should be printed in a comma-separated sequence on a single line.

**Hints:**
Use `range(begin, end)` method.

**Solution:**
```python
l = []
for i in range(2000, 3201):
    if (i % 7 == 0) and (i % 5 != 0):
        l.append(str(i))
print(",".join(l))
```

---

### Question 2 (Level 1)

**Question:**
Write a program to compute the factorial of a given number.

**Example Input:**
```
8
```
**Example Output:**
```
40320
```

**Hints:**
Use recursion.

**Solution:**
```python
def fact(x):
    if x == 0:
        return 1
    return x * fact(x - 1)

x = int(input())
print(fact(x))
```

---

### Question 3 (Level 1)

**Question:**
Generate a dictionary that contains (i, i*i) for numbers between 1 and n (both included), then print the dictionary.

**Example Input:**
```
8
```
**Example Output:**
```
{1: 1, 2: 4, 3: 9, 4: 16, 5: 25, 6: 36, 7: 49, 8: 64}
```

**Solution:**
```python
n = int(input())
d = {i: i*i for i in range(1, n+1)}
print(d)
```

---

### Question 4 (Level 1)

**Question:**
Accept a sequence of comma-separated numbers from the console and generate a list and a tuple containing those numbers.

**Example Input:**
```
34,67,55,33,12,98
```
**Example Output:**
```
['34', '67', '55', '33', '12', '98']
('34', '67', '55', '33', '12', '98')
```

**Solution:**
```python
values = input()
l = values.split(",")
t = tuple(l)
print(l)
print(t)
```

---

### Question 5 (Level 1)

**Question:**
Define a class with methods:
- `getString`: to get a string from console input
- `printString`: to print the string in uppercase

**Solution:**
```python
class InputOutString:
    def __init__(self):
        self.s = ""
    
    def getString(self):
        self.s = input()
    
    def printString(self):
        print(self.s.upper())

strObj = InputOutString()
strObj.getString()
strObj.printString()
```

---

### Question 6 (Level 2)

**Question:**
Calculate the value using the formula:
```
Q = Square root of [(2 * C * D)/H]
```
With fixed values:
```
C = 50, H = 30
```
D is input as a comma-separated sequence.

**Example Input:**
```
100,150,180
```
**Example Output:**
```
18,22,24
```

**Solution:**
```python
import math
c, h = 50, 30
values = input().split(',')
result = [str(int(math.sqrt((2 * c * float(d)) / h))) for d in values]
print(",".join(result))
```

---

### Question 7 (Level 2)

**Question:**
Generate a 2D array where the element in the `i-th` row and `j-th` column is `i * j`.

**Example Input:**
```
3,5
```
**Example Output:**
```
[[0, 0, 0, 0, 0], [0, 1, 2, 3, 4], [0, 2, 4, 6, 8]]
```

**Solution:**
```python
dimensions = [int(x) for x in input().split(',')]
rowNum, colNum = dimensions[0], dimensions[1]
multilist = [[i * j for j in range(colNum)] for i in range(rowNum)]
print(multilist)
```

---



# Special Contest Problem Solution

## Problem Statement
"The contestant who achieves a score equal to or higher than that of the k-th placed contestant  
will advance to the next round, provided they have achieved a positive score."

### **Input Format**
- The first line contains two integers `n` and `k` separated by a space:
  - `n`: Total number of participants.
  - `k`: Position of the k-th place contestant.
- The second line contains `n` integers representing scores in **non-increasing order**.

### **Output Format**
- Print a single integer: the number of participants who qualify for the next round.

---

## Solution

```python
# Read input values
n, k = map(int, input().split())
scores = list(map(int, input().split()))

# Get the k-th place score
threshold = scores[k - 1]

# Count qualifying participants
count = sum(
 for score in scores
      if score >= threshold and score > 0)

# Print the result
print(count)

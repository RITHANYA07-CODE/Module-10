# Queue-Remove Two String Values from the Rear End in Python 🧵

This Python program demonstrates how to manage a list of strings and remove the last two elements (i.e., from the rear of the list).

## 🎯 Aim

To write a Python program to:
- Accept `n` string values from the user
- Remove the last two values (rear end of the list)
- Display the updated list

## 🧠 Algorithm

1. Create an empty list `q`.
2. Read an integer `n` from the user (number of strings).
3. Loop `n` times:
   - Read a string input.
   - Append it to the list `q`.
4. Remove the last element using `pop()`.
5. Remove the next last element using `pop()` again.
6. Display the updated list.

##  Program:
```
from collections import deque

q = deque()
n = int(input())

for i in range(n):
    q.append(input())

for i in range(2):
    if q:
        q.pop()  

print("Updated Queue:", q)

```

### Output:
<img width="1066" height="442" alt="image" src="https://github.com/user-attachments/assets/b203f83a-70cf-43aa-84dd-9fc399c8a258" />

## Result:
Thus, this Python program demonstrates how to manage a list of strings and remove the last two elements (i.e., from the rear of the list).

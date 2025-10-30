# Queue-Queue Values in Descending Order Using Python 🧮

This Python program simulates a queue using a list, removes the first two elements (FIFO order), and displays the remaining values in descending order.

## 🎯 Aim

To write a Python program to:
- Accept user inputs into a list (queue)
- Remove the first two elements (simulating dequeue)
- Display the remaining values in **descending order**

## 🧠 Algorithm

1. Create an empty list `q`.
2. Read an integer `n` to determine how many elements will be added.
3. Loop `n` times:
   - Read an input value.
   - Append it to the list `q`.
4. Remove the first element using `pop(0)`.
5. Remove the second element using `pop(0)` again.
6. Sort the list in descending order.
7. Print the updated list.

## 🧪 Program: 
```
# Step 1: Create an empty list
q = []

# Step 2: Read an integer n
n = int(input("Enter the number of elements: "))

# Step 3: Loop n times to get input values
for i in range(n):
    value = int(input("Enter a number: "))
    q.append(value)

# Step 4: Remove the first element
if len(q) > 0:
    q.pop(0)

# Step 5: Remove the second element (now the new first one)
if len(q) > 0:
    q.pop(0)

# Step 6: Sort the list in descending order
q.sort(reverse=True)

# Step 7: Print the updated list
print("Updated list in descending order:")
print(q)

```

### Output:
<img width="366" height="496" alt="image" src="https://github.com/user-attachments/assets/a46b1446-2643-41ec-a458-eb14ff8b4e1f" />

## Result:
Thus, this Python program simulates a queue using a list, removes the first two elements (FIFO order), and displays the remaining values in descending order.

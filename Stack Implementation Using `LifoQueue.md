# Stack Implementation Using `LifoQueue` (Max Size 5) 🔄

This Python program demonstrates a stack implemented using the `LifoQueue` class from the `queue` module. It allows up to 5 elements, checks if the stack is full, and then prints the elements in reverse (LIFO) order.

## 🎯 Aim

To create a Python program that:
- Implements a stack using `LifoQueue` with a maximum size of 5
- Adds user-inputted values to the stack
- Checks whether the stack is full
- Prints the stack elements in reverse order (LIFO)

## 📋 Algorithm

1. Import the `LifoQueue` class from the `queue` module.
2. Create a stack with a maximum size of 5.
3. Read the number of elements (`n`) to be added to the stack.
4. Loop `n` times:
   - Read a value from the user.
   - Use `put()` to push it onto the stack if it's not full.
5. Use `full()` to check if the stack is full and print the result.
6. Use `get()` repeatedly to pop and print elements in reverse order.

## Program
```
from queue import LifoQueue
stack = LifoQueue(maxsize=5)
n= int(input())
for i in range(n):
    stack.put(input())
print(stack.full())
for i in range(n):
    print(stack.get())
```

## 🧪 Sample Input and Output
<img width="368" height="417" alt="image" src="https://github.com/user-attachments/assets/7ac6c321-d4d9-4b0d-b08e-a3f03f71f2de" />

## Result:
Thus this Python program successfully demonstrates a stack implemented using the `LifoQueue` class from the `queue` module.

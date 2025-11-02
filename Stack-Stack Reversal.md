# # Stack-Stack Reversal Program 🔁

To write a Python program that reverses a given string using recursion and basic swap operations.

## 🎯 Aim

To write a Python program that reverses a given string using recursion and basic swap operations.

## 📋 Algorithm

1. **Define a function `swap(s, i, j)`**

   * Swap the characters at positions `i` and `j` in the list `s`.

2. **Define a recursive function `reverse(s, i=0, j=0)`**

   * Base Case: If `j` equals the length of `s`, return `i`.
   * Recursive Step:

     * Call `reverse(s, i, j + 1)` to move to the end of the string.
     * After returning from recursion, if `i <= j`, call `swap(s, i, j)` to swap characters.
     * Increment `i` by 1 and return it.

3. **Main Program:**

   * Take a string input from the user.
   * Convert the string to a list of characters (since strings are immutable).
   * Call the `reverse()` function.
   * Join the characters back into a string.
   * Print the reversed string.


### Program:
```
def swap(s, i, j):
    temp = s[i]
    s[i] = s[j]
    s[j] = temp

def reverse(s, i=0, j=0):
    if j == len(s):
        return i
 
    i = reverse(s, i, j + 1)
    if i <= j:
        swap(s, i, j)
        i += 1
 
    return i
 

s = input()

chars = [*s]
reverse(chars)
s = ''.join(chars)

print(s)
```

## 🧪 Sample Input and Output
<img width="387" height="149" alt="image" src="https://github.com/user-attachments/assets/2cf2fff4-1c71-4e48-aa41-47a94651788c" />

## Result
The program successfully reverses a string using recursion without relying on Python’s built-in slicing or reverse functions.

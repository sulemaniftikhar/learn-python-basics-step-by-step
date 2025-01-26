# Loops

## Overview

Loops allow you to execute a block of code repeatedly. Python provides two primary types of loops: the `for` loop and the `while` loop. You can also control the flow of loops using control statements like `break`, `continue`, and `pass`.

---

## 1. `for` Loops

The `for` loop is used to iterate over a sequence (such as a list, tuple, string, or range). It executes the code inside the loop for each item in the sequence.

### Syntax:
```python
for item in sequence:
    # Code to execute for each item
```

### Example: Iterating over a list
```python
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)
# Output:
# apple
# banana
# cherry
```

### Example: Using `range()` with `for` loop
The `range()` function generates a sequence of numbers. It’s commonly used in `for` loops when you need to repeat a block of code a specific number of times.

```python
for i in range(5):  # Iterates over numbers 0 to 4
    print(i)
# Output:
# 0
# 1
# 2
# 3
# 4
```

---

## 2. `while` Loops

The `while` loop repeats the code as long as the given condition is `True`. If the condition becomes `False`, the loop stops.

### Syntax:
```python
while condition:
    # Code to execute as long as condition is True
```

### Example: Counting from 1 to 5 using `while` loop
```python
count = 1
while count <= 5:
    print(count)
    count += 1
# Output:
# 1
# 2
# 3
# 4
# 5
```

---

## 3. Loop Control Statements

Python provides control statements that allow you to modify the behavior of loops.

### `break`:
The `break` statement is used to exit the loop prematurely.

```python
for i in range(5):
    if i == 3:
        break
    print(i)
# Output:
# 0
# 1
# 2
```

### `continue`:
The `continue` statement skips the current iteration and moves to the next iteration of the loop.

```python
for i in range(5):
    if i == 3:
        continue
    print(i)
# Output:
# 0
# 1
# 2
# 4
```

### `pass`:
The `pass` statement is a placeholder that does nothing. It is used when a statement is syntactically required but you don't want to perform any action.

```python
for i in range(5):
    if i == 3:
        pass  # Placeholder, does nothing
    print(i)
# Output:
# 0
# 1
# 2
# 3
# 4
```

---

## 4. Nested Loops

A nested loop is a loop inside another loop. The inner loop runs completely every time the outer loop iterates.

### Example: Using nested `for` loops
```python
for i in range(1, 4):
    for j in range(1, 4):
        print(f"i={i}, j={j}")
# Output:
# i=1, j=1
# i=1, j=2
# i=1, j=3
# i=2, j=1
# i=2, j=2
# i=2, j=3
# i=3, j=1
# i=3, j=2
# i=3, j=3
```

---

## 5. Iterating Over Sequences

You can iterate over different types of sequences, like strings, ranges, and lists, using loops.

### Example: Iterating over a string
```python
word = "Python"
for letter in word:
    print(letter)
# Output:
# P
# y
# t
# h
# o
# n
```

### Example: Iterating over a range with a step
```python
for i in range(0, 10, 2):  # Range with a step of 2
    print(i)
# Output:
# 0
# 2
# 4
# 6
# 8
```

---

## Summary

- **`for` Loops**: Used for iterating over sequences like lists, strings, and ranges.
- **`while` Loops**: Continues execution as long as the condition is `True`.
- **Control Statements**: `break`, `continue`, and `pass` control the flow of loops.
- **Nested Loops**: Loops within loops to handle multi-dimensional tasks.
- **Iterating Over Sequences**: You can loop through strings, lists, ranges, and more.

---
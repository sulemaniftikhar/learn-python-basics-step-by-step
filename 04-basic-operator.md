# Basic Operators

## Overview

Operators are special symbols used to perform operations on values and variables. Python supports several types of operators, including arithmetic, comparison, logical, and assignment operators.

---

## 1. Arithmetic Operators

Arithmetic operators are used to perform mathematical operations such as addition, subtraction, multiplication, etc.

### Operators:
- `+`: Addition
- `-`: Subtraction
- `*`: Multiplication
- `/`: Division (returns a float)
- `//`: Floor division (returns an integer)
- `%`: Modulus (returns the remainder of division)
- `**`: Exponentiation (raises a number to a power)

### Examples:
```python
x = 10
y = 3

# Addition
print(x + y)  # Output: 13

# Subtraction
print(x - y)  # Output: 7

# Multiplication
print(x * y)  # Output: 30

# Division
print(x / y)  # Output: 3.333333...

# Floor Division
print(x // y)  # Output: 3

# Modulus
print(x % y)  # Output: 1

# Exponentiation
print(x ** y)  # Output: 1000
```

---

## 2. Comparison Operators

Comparison operators are used to compare two values. These operators return `True` or `False` based on the comparison.

### Operators:
- `==`: Equal to
- `!=`: Not equal to
- `<`: Less than
- `>`: Greater than
- `<=`: Less than or equal to
- `>=`: Greater than or equal to

### Examples:
```python
x = 10
y = 5

# Equal to
print(x == y)  # Output: False

# Not equal to
print(x != y)  # Output: True

# Less than
print(x < y)   # Output: False

# Greater than
print(x > y)   # Output: True

# Less than or equal to
print(x <= y)  # Output: False

# Greater than or equal to
print(x >= y)  # Output: True
```

---

## 3. Logical Operators

Logical operators are used to combine conditional statements. They allow you to check multiple conditions at once.

### Operators:
- `and`: Returns `True` if both conditions are true
- `or`: Returns `True` if at least one condition is true
- `not`: Inverts the boolean value of the condition

### Examples:
```python
x = 10
y = 5

# and (both conditions must be true)
print(x > 5 and y < 10)  # Output: True

# or (at least one condition must be true)
print(x > 5 or y > 10)   # Output: True

# not (inverts the boolean value)
print(not(x > 5))        # Output: False
```

---

## 4. Assignment Operators

Assignment operators are used to assign values to variables. In addition to basic assignment, Python provides shorthand operators for performing operations and assignment in one step.

### Operators:
- `=`: Assigns a value
- `+=`: Adds and assigns the value
- `-=`: Subtracts and assigns the value
- `*=`: Multiplies and assigns the value
- `/=`: Divides and assigns the value
- `//=`: Floor divides and assigns the value
- `%=`: Modulus and assigns the value
- `**=`: Exponentiates and assigns the value

### Examples:
```python
x = 10

# Addition assignment
x += 5
print(x)  # Output: 15

# Subtraction assignment
x -= 3
print(x)  # Output: 12

# Multiplication assignment
x *= 2
print(x)  # Output: 24

# Division assignment
x /= 4
print(x)  # Output: 6.0

# Floor division assignment
x //= 2
print(x)  # Output: 3.0

# Modulus assignment
x %= 2
print(x)  # Output: 1.0

# Exponentiation assignment
x **= 3
print(x)  # Output: 1.0
```

---

## Summary

- **Arithmetic Operators**: Used for mathematical operations like addition, multiplication, and exponentiation.  
- **Comparison Operators**: Used to compare values, returning `True` or `False`.  
- **Logical Operators**: Used to combine conditions using `and`, `or`, and `not`.  
- **Assignment Operators**: Used to assign values to variables, with shorthand operators for combined operations and assignment.

---
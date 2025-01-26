# Variables and Data Types

## Overview

In Python, variables are used to store data values. Python is dynamically typed, meaning you don’t have to declare the type of a variable explicitly. You can store different data types in variables and perform operations on them.

---

## 1. Variable Declaration and Naming Conventions

A variable in Python is created when you assign a value to it. Python does not require explicit declaration of variables, and the type is determined dynamically based on the assigned value.

### Syntax:
```python
variable_name = value
```

### Naming Conventions:
- Variable names must start with a letter (a-z, A-Z) or an underscore (`_`).
- The rest of the name can contain letters, digits (0-9), and underscores.
- Variable names are case-sensitive (e.g., `name` and `Name` are different).
- It is recommended to use lowercase letters for variable names, with underscores between words (e.g., `my_variable`).
- Avoid using Python reserved keywords (e.g., `if`, `else`, `for`).

### Example:
```python
age = 25          # Valid
_name = "Alice"   # Valid
1name = "Bob"     # Invalid (cannot start with a number)
```

---

## 2. Basic Data Types

Python has several built-in data types. The most common ones include integers, floats, strings, and booleans.

### a) Integers (`int`)

Integers are whole numbers (positive, negative, or zero) without decimal points.

### Example:
```python
x = 10       # Integer
y = -5       # Integer
```

### b) Floats (`float`)

Floats represent numbers that have a decimal point.

### Example:
```python
x = 3.14     # Float
y = -2.5     # Float
```

### c) Strings (`str`)

Strings represent sequences of characters enclosed in single (`'`) or double (`"`) quotes.

### Example:
```python
name = "Alice"    # String
greeting = 'Hello' # String
```

### d) Booleans (`bool`)

Booleans represent one of two values: `True` or `False`. They are often used in conditionals.

### Example:
```python
is_active = True   # Boolean
is_finished = False # Boolean
```

---

## 3. Type Checking and Type Conversion

### a) Type Checking (`type()`)

The `type()` function returns the type of an object.

### Syntax:
```python
type(object)
```

### Example:
```python
x = 10
print(type(x))  # Output: <class 'int'>

y = 3.14
print(type(y))  # Output: <class 'float'>

name = "Alice"
print(type(name))  # Output: <class 'str'>
```

### b) Type Conversion

You can convert one data type to another using type conversion functions.

### Common Type Conversion Functions:
- `int()`: Converts to an integer.
- `float()`: Converts to a float.
- `str()`: Converts to a string.
- `bool()`: Converts to a boolean.

### Example:
```python
# Convert string to integer
num_str = "100"
num_int = int(num_str)
print(num_int)  # Output: 100

# Convert integer to string
x = 10
x_str = str(x)
print(x_str)  # Output: "10"

# Convert float to integer (loses decimal part)
y = 3.14
y_int = int(y)
print(y_int)  # Output: 3

# Convert integer to boolean
z = 0
z_bool = bool(z)
print(z_bool)  # Output: False (0 is considered False, any non-zero value is True)
```

---

## Summary

- **Variable Declaration**: Variables are created by assigning a value. Naming conventions recommend lowercase letters with underscores for multi-word names.  
- **Basic Data Types**:  
   - **Integers**: Whole numbers.  
   - **Floats**: Numbers with decimal points.  
   - **Strings**: Sequences of characters.  
   - **Booleans**: Values representing `True` or `False`.  
- **Type Checking**: Use the `type()` function to check the type of a variable.  
- **Type Conversion**: You can convert between different types using functions like `int()`, `float()`, `str()`, and `bool()`.

---
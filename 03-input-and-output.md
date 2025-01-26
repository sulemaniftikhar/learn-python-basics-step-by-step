# Input and Output

## Overview

In Python, input and output are essential for interacting with the user or displaying data. The `print()` function is used to display output, and the `input()` function is used to take user input. String formatting is useful for creating dynamic strings.

---

## 1. `print()` Function

The `print()` function is used to output data to the console. You can pass one or more arguments to `print()`, and it will display them in the console.

### Syntax:
```python
print(object, sep=' ', end='\n', file=sys.stdout, flush=False)
```

- `object`: The value(s) to be printed.
- `sep`: The separator between values (default is a space).
- `end`: The string appended at the end of the output (default is a newline).
- `file`: Specifies where the output is sent (default is standard output).
- `flush`: Whether to forcibly flush the output buffer.

### Example: Basic usage
```python
print("Hello, World!")  # Output: Hello, World!
```

### Example: Printing multiple values
```python
name = "Alice"
age = 25
print(name, age)  # Output: Alice 25
```

### Example: Using `sep` and `end`
```python
print("Hello", "World", sep="-", end="!")  # Output: Hello-World!
```

---

## 2. `input()` Function

The `input()` function is used to take input from the user. It reads a line of text entered by the user and returns it as a string.

### Syntax:
```python
input(prompt)
```

- `prompt`: A string that is displayed to the user (optional).

### Example: Basic usage
```python
name = input("Enter your name: ")
print("Hello, " + name)  # Output: Hello, (user input)
```

### Example: Converting input to a specific data type
The `input()` function returns a string by default. You can convert it to other types (like `int`, `float`, etc.) using type casting.

```python
age = int(input("Enter your age: "))
print("You are " + str(age) + " years old.")  # Output: You are (user input) years old.
```

---

## 3. String Formatting

String formatting allows you to create strings dynamically by embedding values into a string. There are multiple ways to format strings in Python.

### a) f-strings (Python 3.6+)

F-strings (formatted string literals) are a concise and efficient way to embed expressions inside string literals using curly braces `{}`.

### Syntax:
```python
f"string {expression}"
```

### Example: Using f-strings
```python
name = "Alice"
age = 25
greeting = f"Hello, my name is {name} and I am {age} years old."
print(greeting)  # Output: Hello, my name is Alice and I am 25 years old.
```

### b) `format()` Method

The `format()` method allows you to insert values into placeholders defined by `{}` in a string.

### Syntax:
```python
"string {}".format(value)
```

### Example: Using `format()`
```python
name = "Bob"
greeting = "Hello, my name is {}.".format(name)
print(greeting)  # Output: Hello, my name is Bob.
```

### c) `%` Formatting (Old-style)

The `%` operator can be used to format strings, but it is considered less modern than f-strings or `format()`.

### Syntax:
```python
"string % value"
```

### Example: Using `%` formatting
```python
name = "Charlie"
greeting = "Hello, my name is %s." % name
print(greeting)  # Output: Hello, my name is Charlie.
```

---

## Summary

- **`print()`**: Used to display output. You can format the output using separators and endings.  
- **`input()`**: Used to take user input, which is returned as a string. You can convert it to other types.  
- **String Formatting**:  
   - **f-strings**: Concise and efficient method for embedding expressions in strings.  
   - **`format()`**: Older but still useful method for string formatting.  
   - **`%`**: The traditional method for string formatting.

---
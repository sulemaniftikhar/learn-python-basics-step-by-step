# Functions

## Overview

Functions are a way to group reusable pieces of code. In Python, functions are defined using the `def` keyword. Functions allow you to pass data into them (through parameters) and return results (via the `return` statement).

---

## 1. Defining Functions with `def`

You can define a function using the `def` keyword, followed by the function name and parentheses `()`. Inside the parentheses, you define any parameters the function takes. The function body is indented and contains the code to be executed.

### Syntax:
```python
def function_name(parameters):
    # Function body
    return result  # Optional
```

### Example: Defining a simple function
```python
def greet():
    print("Hello, World!")
    
greet()  # Output: Hello, World!
```

---

## 2. Parameters and Return Values

Functions can accept parameters (arguments) that provide data to work with. The `return` keyword is used to return the result from the function.

### Example: Function with parameters and return value
```python
def add(a, b):
    return a + b

result = add(5, 3)
print(result)  # Output: 8
```

### Explanation:
- `a` and `b` are parameters.
- `return a + b` returns the sum of `a` and `b`.

---

## 3. Default and Keyword Arguments

### Default Arguments:
You can assign default values to parameters. These values are used if no argument is provided for that parameter when calling the function.

```python
def greet(name="Guest"):
    print(f"Hello, {name}!")

greet()         # Output: Hello, Guest!
greet("Alice")  # Output: Hello, Alice!
```

### Keyword Arguments:
You can pass arguments by specifying the parameter names when calling the function. This is useful when a function has many parameters or default values.

```python
def greet(name, age):
    print(f"Hello, {name}. You are {age} years old.")

greet(name="Bob", age=25)  # Output: Hello, Bob. You are 25 years old.
```

---

## 4. Scope of Variables (Local vs. Global)

### Local Scope:
A variable defined inside a function is local to that function and can only be accessed within it.

```python
def example():
    x = 10  # Local variable
    print(x)

example()  # Output: 10
# print(x)  # This will raise a NameError because x is local to example()
```

### Global Scope:
A variable defined outside any function is global and can be accessed by any function in the script.

```python
x = 10  # Global variable

def example():
    print(x)  # Accessing global variable

example()  # Output: 10
```

To modify a global variable inside a function, you must use the `global` keyword:

```python
x = 10

def change_global():
    global x
    x = 20

change_global()
print(x)  # Output: 20
```

---

## Summary

- **Defining Functions**: Use the `def` keyword to define a function. Functions can accept parameters and return values.  
- **Parameters and Return Values**: Functions can take parameters and return results.  
- **Default and Keyword Arguments**: Provide default values for parameters or pass arguments by name.  
- **Scope**: Variables defined inside a function are local, while variables defined outside are global. Use the `global` keyword to modify global variables inside a function.

---
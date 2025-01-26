# Control Flow

## Overview

Control flow allows you to control the order in which statements are executed based on conditions. Python provides `if`, `elif`, and `else` statements to evaluate conditions and decide which block of code to execute.

---

## 1. `if`, `elif`, `else` Statements

The `if` statement is used to test a condition. If the condition is `True`, the associated block of code is executed. If the condition is `False`, the program moves on to the `elif` or `else` block (if they exist).

### Syntax:
```python
if condition:
    # Code to execute if condition is True
elif another_condition:
    # Code to execute if the second condition is True
else:
    # Code to execute if no conditions are True
```

### Example: Using `if`, `elif`, and `else`
```python
age = 18

if age < 18:
    print("You are a minor.")
elif age == 18:
    print("You are 18 years old.")
else:
    print("You are an adult.")
# Output: You are 18 years old.
```

---

## 2. Nested Conditionals

You can place one conditional statement inside another, which allows for more complex decision-making processes.

### Syntax:
```python
if condition1:
    if condition2:
        # Code to execute if both conditions are True
    else:
        # Code to execute if condition1 is True but condition2 is False
else:
    # Code to execute if condition1 is False
```

### Example: Nested `if` statements
```python
age = 20
if age >= 18:
    if age < 21:
        print("You are an adult, but not yet 21.")
    else:
        print("You are 21 or older.")
# Output: You are an adult, but not yet 21.
```

---

## 3. Logical Expressions in Conditionals

You can use logical operators (`and`, `or`, `not`) in conditionals to combine multiple conditions. These operators allow for more flexibility in testing multiple conditions.

### `and`:
The condition is `True` only if both conditions are `True`.

```python
x = 10
y = 5
if x > 5 and y < 10:
    print("Both conditions are true.")
# Output: Both conditions are true.
```

### `or`:
The condition is `True` if at least one of the conditions is `True`.

```python
x = 10
y = 15
if x > 5 or y < 10:
    print("At least one condition is true.")
# Output: At least one condition is true.
```

### `not`:
The `not` operator inverts the boolean value of a condition.

```python
x = 10
if not x < 5:
    print("x is not less than 5.")
# Output: x is not less than 5.
```

---

## Summary

- **`if`, `elif`, `else`**: Used for decision-making based on conditions.  
- **Nested Conditionals**: Place `if` statements inside one another for more complex logic.  
- **Logical Expressions**: Use `and`, `or`, and `not` to combine or invert conditions.

---
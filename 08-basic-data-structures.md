# Basic Data Structures

## Overview

In Python, basic data structures allow us to store and manage data efficiently. The fundamental data structures include strings and lists. This section will focus on string operations and list operations, including common methods and techniques.

---

## 1. Strings

Strings are sequences of characters. In Python, strings are immutable, meaning they cannot be changed once they are created. However, you can perform various operations on them.

### String Slicing and Indexing

You can access individual characters of a string using indexing and slice substrings using slicing.

#### Indexing:
Each character in a string has an index. The first character has an index of 0, and negative indices start from -1 for the last character.

```python
text = "Hello, World!"
print(text[0])  # Output: H
print(text[-1])  # Output: !
```

#### Slicing:
You can extract a part of a string using slicing, specifying a start, stop, and optional step.

```python
text = "Hello, World!"
print(text[0:5])  # Output: Hello
print(text[7:])   # Output: World!
print(text[::2])  # Output: Hoo ol!
```

### String Methods

Python provides several built-in methods to manipulate strings.

#### Common Methods:
- `len(string)`: Returns the length of the string.
- `string.lower()`: Converts the string to lowercase.
- `string.upper()`: Converts the string to uppercase.
- `string.split()`: Splits the string into a list based on a delimiter (default is space).
- `string.join(iterable)`: Joins elements of an iterable into a single string.
- `string.replace(old, new)`: Replaces all occurrences of the substring `old` with `new`.

#### Example:
```python
text = "Hello, World!"
print(len(text))           # Output: 13
print(text.lower())        # Output: hello, world!
print(text.upper())        # Output: HELLO, WORLD!
print(text.split(", "))    # Output: ['Hello', 'World!']
print(" ".join(['Hello', 'World!']))  # Output: Hello World!
```

---

## 2. Lists

Lists are ordered collections that can hold items of any data type. Lists are mutable, meaning you can modify them after creation. They can store duplicates and support indexing and slicing like strings.

### Creating and Modifying Lists

You can create a list using square brackets, and you can modify a list by adding, removing, or changing its elements.

```python
fruits = ["apple", "banana", "cherry"]
fruits.append("orange")  # Adds "orange" to the end of the list
print(fruits)  # Output: ['apple', 'banana', 'cherry', 'orange']
```

### Indexing, Slicing, and Nested Lists

You can access individual elements using indexing or create sublists with slicing. Lists can also contain other lists (nested lists).

#### Indexing and Slicing:
```python
numbers = [1, 2, 3, 4, 5]
print(numbers[0])   # Output: 1
print(numbers[1:3]) # Output: [2, 3]
print(numbers[-1])  # Output: 5
```

#### Nested Lists:
```python
nested_list = [1, [2, 3], 4]
print(nested_list[1])      # Output: [2, 3]
print(nested_list[1][0])   # Output: 2
```

### List Methods

Python provides a variety of methods to manipulate lists.

#### Common Methods:
- `append(item)`: Adds an item to the end of the list.
- `remove(item)`: Removes the first occurrence of an item from the list.
- `pop(index)`: Removes and returns the item at the specified index.
- `sort()`: Sorts the list in ascending order.
- `reverse()`: Reverses the list.
- `extend(iterable)`: Adds all elements of an iterable to the list.

#### Example:
```python
fruits = ["apple", "banana", "cherry"]
fruits.append("orange")
fruits.remove("banana")
fruits.sort()
print(fruits)  # Output: ['apple', 'cherry', 'orange']
```

---

## Summary

- **Strings**: Strings are immutable sequences of characters. You can access, slice, and manipulate strings using various methods.  
- **Lists**: Lists are mutable, ordered collections that support indexing, slicing, and nesting. Lists can be modified using built-in methods such as `append()`, `remove()`, and `sort()`.

---
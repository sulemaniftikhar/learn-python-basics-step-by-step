# Sets

## Overview

A set in Python is an unordered collection of unique elements. Sets do not allow duplicate values and are mutable, meaning you can add or remove elements after creation. Sets are often used to perform mathematical set operations like union, intersection, and difference.

---

## 1. Creating Sets

You can create a set by placing items inside curly braces `{}`, or by using the `set()` constructor.

### Syntax:
```python
my_set = {item1, item2, item3}
```
or
```python
my_set = set([item1, item2, item3])
```

### Example: Creating a set
```python
fruits = {"apple", "banana", "cherry"}
print(fruits)  # Output: {'apple', 'banana', 'cherry'}
```

### Note:
- Sets automatically remove duplicate elements.
```python
numbers = {1, 2, 3, 2, 3}
print(numbers)  # Output: {1, 2, 3}
```

---

## 2. Set Operations

Sets allow you to perform several mathematical operations such as union, intersection, and difference.

### Union (`|` or `.union()`):
The union of two sets combines all elements from both sets, removing duplicates.

```python
set1 = {1, 2, 3}
set2 = {3, 4, 5}
union_set = set1 | set2
print(union_set)  # Output: {1, 2, 3, 4, 5}
```

Alternatively, you can use the `.union()` method:
```python
union_set = set1.union(set2)
```

### Intersection (`&` or `.intersection()`):
The intersection of two sets returns the common elements.

```python
set1 = {1, 2, 3}
set2 = {3, 4, 5}
intersection_set = set1 & set2
print(intersection_set)  # Output: {3}
```

Alternatively, you can use the `.intersection()` method:
```python
intersection_set = set1.intersection(set2)
```

### Difference (`-` or `.difference()`):
The difference between two sets returns the elements in the first set that are not in the second.

```python
set1 = {1, 2, 3}
set2 = {3, 4, 5}
difference_set = set1 - set2
print(difference_set)  # Output: {1, 2}
```

Alternatively, you can use the `.difference()` method:
```python
difference_set = set1.difference(set2)
```

---

## 3. Set Methods

Python provides several built-in methods to manipulate sets.

### Common Methods:
- `add(item)`: Adds an item to the set. If the item already exists, it is ignored.
- `remove(item)`: Removes the specified item from the set. Raises a `KeyError` if the item is not found.
- `discard(item)`: Removes the specified item from the set. Does not raise an error if the item is not found.
- `pop()`: Removes and returns an arbitrary item from the set. Raises a `KeyError` if the set is empty.
- `clear()`: Removes all items from the set.
- `copy()`: Returns a shallow copy of the set.

#### Example:
```python
numbers = {1, 2, 3}
numbers.add(4)  # Adds 4 to the set
numbers.remove(2)  # Removes 2 from the set
numbers.discard(5)  # Does nothing, as 5 is not in the set
print(numbers)  # Output: {1, 3, 4}
```

### Example using `pop()`:
```python
numbers = {1, 2, 3}
removed_item = numbers.pop()
print(removed_item)  # Output: (an arbitrary item, e.g., 1)
print(numbers)  # Output: {2, 3}
```

---

## Summary

- **Sets**: Unordered collections of unique elements. Useful for operations like union, intersection, and difference.  
- **Set Operations**: Perform union, intersection, and difference with the `|`, `&`, `-` operators or corresponding methods.  
- **Methods**: Use `add()`, `remove()`, `discard()`, `pop()`, and `clear()` to modify sets.

---
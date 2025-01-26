# Tuples

## Overview

A tuple is an ordered collection of elements, similar to a list, but unlike lists, tuples are **immutable**, meaning their contents cannot be changed once they are created. Tuples are used to store a fixed collection of items.

---

## 1. Creating and Using Tuples

You can create a tuple by placing items inside parentheses `()` and separating them with commas. A tuple can contain elements of any data type, including other tuples.

### Syntax:
```python
my_tuple = (item1, item2, item3)
```

### Example: Creating a tuple
```python
person = ("Alice", 30, "New York")
print(person)  # Output: ('Alice', 30, 'New York')
```

### Single-element Tuples:
To create a tuple with a single element, you must include a comma after the element.
```python
single_item_tuple = (5,)
print(single_item_tuple)  # Output: (5,)
```

---

## 2. Tuple Immutability

Tuples are immutable, meaning that their elements cannot be changed, added, or removed after creation. If you try to modify a tuple, Python will raise an error.

### Example: Attempting to modify a tuple
```python
person = ("Alice", 30, "New York")
# person[1] = 31  # This will raise a TypeError: 'tuple' object does not support item assignment
```

Although you cannot change individual elements, you can perform operations such as concatenation or slicing to create a new tuple.

```python
new_person = person + ("Engineer",)
print(new_person)  # Output: ('Alice', 30, 'New York', 'Engineer')
```

---

## 3. Packing and Unpacking Tuples

### Packing:
When you create a tuple, you are "packing" multiple items into a single tuple.

```python
coordinates = (4, 5)  # Packing
```

### Unpacking:
Unpacking allows you to assign individual elements of a tuple to separate variables.

```python
person = ("Alice", 30, "New York")
name, age, city = person  # Unpacking
print(name)  # Output: Alice
print(age)   # Output: 30
print(city)  # Output: New York
```

### Example with extra values:
If the number of variables does not match the number of tuple elements, Python will raise a `ValueError`. However, you can use the `*` operator to capture extra values.

```python
person = ("Alice", 30, "New York", "Engineer")
name, *rest = person  # Unpacking with extra values
print(name)  # Output: Alice
print(rest)  # Output: [30, 'New York', 'Engineer']
```

---

## 4. Tuple Methods

Tuples have a few built-in methods that can be used to retrieve information about their contents.

### Common Methods:
- `count(item)`: Returns the number of times the specified item appears in the tuple.
- `index(item)`: Returns the index of the first occurrence of the specified item. Raises a `ValueError` if the item is not found.

#### Example:
```python
numbers = (1, 2, 3, 1, 4, 1)
print(numbers.count(1))  # Output: 3
print(numbers.index(3))  # Output: 2
# print(numbers.index(5))  # This will raise a ValueError
```

---

## Summary

- **Tuples**: Ordered, immutable collections. Useful for storing fixed collections of items.  
- **Immutability**: Tuples cannot be modified after creation, but you can create new tuples by combining or slicing them.  
- **Packing and Unpacking**: Pack values into a tuple and unpack them into variables.  
- **Methods**: Use `count()` and `index()` to interact with tuple contents.

---
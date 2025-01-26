# Dictionaries

## Overview

A dictionary in Python is an unordered collection of key-value pairs. Each key is unique, and the value associated with it can be of any data type. Dictionaries are mutable, allowing you to modify, add, or delete key-value pairs.

---

## 1. Creating and Accessing Dictionaries

You can create a dictionary using curly braces `{}` with key-value pairs separated by a colon. Keys are unique, and values can be of any data type.

### Syntax:
```python
my_dict = {"key1": value1, "key2": value2}
```

### Example: Creating and accessing a dictionary
```python
person = {"name": "Alice", "age": 30, "city": "New York"}
print(person["name"])  # Output: Alice
print(person["age"])   # Output: 30
```

### Explanation:
- `person["name"]` accesses the value associated with the key `"name"`.
- If the key does not exist, it will raise a `KeyError`.

---

## 2. Adding, Updating, and Deleting Key-Value Pairs

Dictionaries are mutable, so you can add, update, and delete key-value pairs.

### Adding or Updating Key-Value Pairs:
If the key already exists, the value will be updated. If the key does not exist, a new key-value pair is added.

```python
person = {"name": "Alice", "age": 30}
person["city"] = "New York"  # Adding a new key-value pair
person["age"] = 31           # Updating the value of an existing key
print(person)  # Output: {'name': 'Alice', 'age': 31, 'city': 'New York'}
```

### Deleting Key-Value Pairs:
You can use the `del` keyword to remove a key-value pair from a dictionary.

```python
del person["age"]
print(person)  # Output: {'name': 'Alice', 'city': 'New York'}
```

You can also use the `pop(key)` method to remove a key-value pair and return the value.

```python
city = person.pop("city")
print(person)  # Output: {'name': 'Alice'}
print(city)    # Output: New York
```

---

## 3. Dictionary Methods

Python provides several built-in methods to manipulate and access data in a dictionary.

### Common Methods:
- `keys()`: Returns a view object of all keys in the dictionary.
- `values()`: Returns a view object of all values in the dictionary.
- `items()`: Returns a view object of all key-value pairs (tuples).
- `get(key)`: Returns the value associated with the specified key. If the key doesn’t exist, it returns `None` (or a specified default value).
- `pop(key)`: Removes the specified key and returns its value.

#### Example:
```python
person = {"name": "Alice", "age": 30, "city": "New York"}

# Get all keys
print(person.keys())  # Output: dict_keys(['name', 'age', 'city'])

# Get all values
print(person.values())  # Output: dict_values(['Alice', 30, 'New York'])

# Get all key-value pairs
print(person.items())  # Output: dict_items([('name', 'Alice'), ('age', 30), ('city', 'New York')])

# Get value using get() method
print(person.get("name"))  # Output: Alice
print(person.get("country", "Not Available"))  # Output: Not Available
```

---

## Summary

- **Dictionaries**: Dictionaries are unordered collections of key-value pairs. Keys must be unique, and values can be of any data type.  
- **Adding, Updating, Deleting**: You can add, update, and delete key-value pairs using simple syntax and built-in methods.  
- **Methods**: Use `keys()`, `values()`, and `items()` to access keys, values, and key-value pairs, respectively. The `get()` method is used to safely retrieve a value by key.

---
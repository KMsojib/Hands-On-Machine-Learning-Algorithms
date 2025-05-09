# Python Variables: A to Z

## A. Assigning Variables
- Variables in Python are created when you assign a value to them.
```python
x = 10
name = "John"
```

## B. Basic Rules for Variable Names
- Variable names must start with a letter or an underscore (_).
- They cannot start with a number.
- They can contain letters, numbers, and underscores (_).
- They are case-sensitive (`age` and `Age` are different).

## C. Constants
- By convention, variables meant to be constants are written in uppercase.
```python
PI = 3.14159
```

## D. Data Types
- Variables can hold data of different types: `int`, `float`, `str`, `bool`, `list`, `tuple`, `dict`, etc.
```python
age = 25        # int
height = 6.1    # float
is_happy = True # bool
fruits = ["apple", "banana"] # list
```

## E. Empty Variables
- You can initialize a variable with `None` to indicate it has no value.
```python
x = None
```

## F. Formatting Strings
- Use f-strings or `.format()` to include variables in strings.
```python
name = "Alice"
greeting = f"Hello, {name}!"
```

## G. Global and Local Variables
- Variables defined outside a function are global.
- Variables defined inside a function are local.
```python
x = "global"

def my_function():
    x = "local"  # Local variable
    print(x)

my_function()
print(x)
```

## H. Hot-Swapping Values
- You can swap values of two variables directly in Python.
```python
a, b = 5, 10
a, b = b, a
```

## I. Immutable vs Mutable
- Some data types like `int`, `float`, and `str` are immutable.
- Others like `list` and `dict` are mutable.
```python
x = [1, 2, 3]  # Mutable
y = 10          # Immutable
```

## J. Joining Strings
- Concatenate strings using `+` or `.join()`.
```python
first = "Hello"
second = "World"
result = first + " " + second
```

## K. Keywords
- Avoid using Python keywords as variable names (e.g., `def`, `class`, `if`).

## L. Length of Variables
- There is no strict limit on the length of variable names, but keep them meaningful.

## M. Multiple Assignments
- Assign multiple variables in one line.
```python
a, b, c = 1, 2, 3
```

## N. Naming Conventions
- Use `snake_case` for variable names (e.g., `user_name`).
- Use descriptive names for clarity.

## O. Object References
- Variables are references to objects in memory.
```python
x = [1, 2, 3]
y = x  # Both refer to the same object
```

## P. Print Variables
- Use the `print()` function to display variable values.
```python
x = 42
print(x)
```

## Q. Quoting Strings
- Strings can be enclosed in single, double, or triple quotes.
```python
single = 'Single quotes'
double = "Double quotes"
triple = """Triple quotes"""
```

## R. Raw Strings
- Use `r` before a string for raw string literals (useful for file paths).
```python
path = r"C:\Users\Name\Folder"
```

## S. Scope of Variables
- Variables have a scope: global, local, or nonlocal.
```python
def outer_function():
    x = "outer"
    def inner_function():
        nonlocal x
        x = "inner"
```

## T. Type Checking
- Use `type()` to check the type of a variable.
```python
x = 42
print(type(x))  # Output: <class 'int'>
```

## U. Unpacking
- Unpack values from iterables into variables.
```python
a, b, c = [1, 2, 3]
```

## V. Variable Deletion
- Use `del` to delete a variable.
```python
x = 10
del x
```

## W. Weak References
- Use `weakref` for weak references to objects for garbage collection control.
```python
import weakref
```

## X. XOR for Swapping
- Swap variables without a temporary variable using XOR.
```python
a, b = 5, 10
a = a ^ b
b = a ^ b
a = a ^ b
```

## Y. Yielding Variables
- In generators, use `yield` to return values lazily.
```python
def my_generator():
    yield 1
    yield 2
```

## Z. Zipping Variables
- Use `zip()` to pair elements from multiple iterables.
```python
names = ["Alice", "Bob"]
ages = [25, 30]
zipped = zip(names, ages)
```

---

This guide covers Python variables from A to Z. Use this as a quick reference for best practices and features!
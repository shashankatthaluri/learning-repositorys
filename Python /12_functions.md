# Funcions 📦

- functions are like neatly packaged boxes of code designed to do specific tasks, where the `def` keyword and `return` statements hold the key. 🔧

## def 🛠️

- The `def` keyword signals the start of defining a function.

```python
# Function Definition with Print Statement
def greet(name):
    # This function prints a greeting message with the provided name
    print(f"Hello, {name}!")

# Using the function
greet("Alice")  # Output: Hello, Alice!
```

## Parameters 📦

- Parameters are like the ingredients a function needs to perform its magic. They make a function versatile and ready for different scenarios.

```python
# Function definition to multiply two numbers
def multiply(x, y):
    # Output: Returns the product of the two numbers
    return x * y

# Calling the multiply function with 3 and 5 as arguments
product = multiply(3, 5)
# Output: product variable will hold the value 15
```

## Return 🔄

- The return statement is the special command that lets a function share its magical creation with the outside world.

```python

def add(a, b):
    """A function to add two numbers and return the sum."""
    sum_result = a + b
    return sum_result

# Using the function with values and capturing the result
total_sum = add(7, 8)  #  # Output: the total_sum variable will hold the value 15.
```

## Void_fuction 🔍

- Not all functions give something back. Some just do things without handing out a prize. This emptiness is like a silent companion called None in Python.

```python
def greet_void(name):
    """A greeting function without a return value."""
    print(f"Hello, {name}!")

# Using the void function
greet_void("Bob") # Output: Hello, Bob!
```

- greet_void shares warm greetings without expecting anything in return ✨.

## ✨ Truthiness Unveiled

Delve into truthiness as Python evaluates values in boolean contexts either `True` or `False`.

```python
x = 1
print(x is 1)  # True
print(x is 0)  # False

print(bool("Hello"))  # True
print(bool(""))       # False
print(bool(" "))      # True
```

- In Python, any non-empty string is "truthy", while an empty string is "falsy":
  - `bool("")` is `False`
  - `bool(" ")` is `True`

## 🔍 Comparison Operators

Python provides a lot of operators for comparing values:

- `==`: equal to
- `!=`: not equal to
- `>`: greater than
- `<`: less than
- `<=`: less than or equal to
- `>=`: greater than or equal to
- `is`: is the same object

```python
print(1 == 1)  # True
print(1 != 1)  # False
print(1 < 1)   # False
print(1 > 1)   # False
print(1 >= 1)  # True
print(1 <= 1)  # True
```

# 🌐 Conditional in Python

Make informed choices in your Python journey with conditional statements that execute different code blocks based on conditions.

```python
if 3 > 5:
    print("3 is greater than 5")
elif 5 > 3:
    print("5 is greater than 3")
else:
    print("3 is equal to 5")
```

## 📁 Nested Conditionals

Explore the depths of logic with nested conditional statements in Python.

```python
if age != '':
    if age >= 18:
        print("Welcome! You can enter with a wristband.")
    elif age >= 21:
        print("You can enter and enjoy a drink.")
    else:
        print("Sorry, you can't come in. Maybe when you're older! :(")
else:
    print("Please provide your age.")
```


## 🤝 Logical Operators

Logical operators are used to combine conditional statements:

- `and`: both conditions must be true
- `or`: At least one condition must be true
- `not`: negates the truth value

```python
print(1 < 2 and 2 < 3)  # True
print(1 < 2 and 2 > 3)  # False
print(1 < 2 or 2 > 3)   # True
```

## ↩️ Ternary Operator

The ternary operator in Python allows writing conditional statements in a single line.

```python
age = 22
message = "Eligible" if age >= 18 else "Not Eligible"
print(message)  # Eligible
```

## 🆚 Identity vs. Equality

Understand the distinction between the `is` and `==` operators in Python.

```python
x = [1, 2, 3]
y = [1, 2, 3]
print(x == y)  # True
print(x is y)  # False

a = [1, 2]
clone = a
print(a is clone)  # True
```

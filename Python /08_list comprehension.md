# List Comprehension 💡

- List comprehension is a concise way to create lists. 🚀

## Basic Example 🌟

```python
# Traditional approach using a loop
numbers = [1, 2, 3, 4, 5]
doubled_numbers = []

for number in numbers:
    doubled_numbers.append(number * 2)

# Using list comprehension
doubled_numbers = [number * 2 for number in numbers]
```

## Transforming Strings 📚

```python
name = 'colt'
uppercased_chars = [char.upper() for char in name]  # ['C', 'O', 'L', 'T']
```

## Applying Conditional Logic 🌐

```python
numbers = [1, 2, 3, 4, 5, 6]
evens = [number for number in numbers if number % 2 == 0]
odds = [number for number in numbers if number % 2 != 0]

# Ternary within list comprehension
transformed = [num * 2 if num % 2 == 0 else num / 2 for num in numbers]

# Removing vowels from a string
with_no_vowels = [char for char in 'amazing' if char not in 'aeiou']
```

## Exercises 🏋️‍♂️

- Divisible by 12: Create a list of numbers divisible by 12 (up to 100).

```python
answer = [num for num in range(1, 101) if num % 12 == 0]
```

- Vowel-Free Zone: Craft a list excluding vowels from "amazing".

```python
answer = [char for char in 'amazing' if char not in 'aeiou']
```

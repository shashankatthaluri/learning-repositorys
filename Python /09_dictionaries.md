# Mastering Dictionaries 📚

- Dictionaries store data in key:value pairs. 🗝️
- They are unordered, changeable, and do not allow duplicates. 🔀

## Basic Example 🌟

```python
person = {
    "name": "Bob",
    "age": 45,
    "country": "Norway"
}
```

## Creating a Dictionary 🛠️

- Use `dict()` to create dictionaries.

```python
animals = dict(cat='meow', dog='woof', cow='moo')
```

## Accessing Items 🔑

- Key names are the keys to accessing the treasures.

```python
x = person["age"]
```

## Iterating Through a Dictionary 🔁

- Use loops to iterate through dictionaries.

```python
# Echoing values
for value in person.values():
    print(value)

# Echoing keys
for key in person.keys():
    print(key)

# Echoing both keys and values
for key, value in person.items():
    print(key, value)
```

## Checking for Keys 🕵️

- Use the `in` operator to check for keys.

```python
if "age" in person:
    print("Age is present")
```

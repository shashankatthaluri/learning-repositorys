# Dictionary Methods 🧰

- Python provides built-in methods for dictionaries. 🔧

## Clear() 🧹

- Erase all elements from a dictionary.

```python
person = {
    "name": "Bob",
    "age": 45,
    "country": "Norway"
}

person.clear()

print(person) #  output: {}
```

## Copy() 📋

- Returns a copy of the dictionary.

```python

person = {
    "name": "Bob",
    "age": 45,
    "country": "Norway"
}

x = person.copy()

print(x) #  output: {'name': 'Bob', 'age': 45, 'country': 'Norway'}
```

## Fromkeys() 🔑

- Creates a dictionary with specified keys and values.

## Fromkeys()

- The fromkeys() method returns a dictionary with the specified keys and the specified value.

```python

#Easy

{}.fromkeys(['name', 'age', 'country'], 'unknown')

# output: {'name': 'unknown', 'age': 'unknown', 'country': 'unknown'}

# Advance
x = ('key1', 'key2', 'key3')
y = 0

thisdict = dict.fromkeys(x, y)

print(thisdict) #  output: {'key1': 0, 'key2': 0, 'key3': 0}
```

## Get() 🔍

- Returns the value of a specified key.

```python
person = {
    "name": "Bob",
    "age": 45,
    "country": "Norway"
}

x = person.get("age")

print(x) #  output: 45
```

## Pop() 🚫

- Removes an item with a specified key.

```python
person = {
    "name": "Bob",
    "age": 45,
    "country": "Norway"
}

person.pop("age")

print(person) #  output: {'name': 'Bob', 'country': 'Norway'}
```

## Popitem() 💥

- Removes the last inserted item.

```python
person = {
    "name": "Bob",
    "age": 45,
    "country": "Norway"
}

person.popitem()

print(person) #  output: {'name': 'Bob', 'age': 45}
```

## Update() 🔄

- Inserts specified items into the dictionary.

```python

person = {
    "name": "Bob",
    "age": 45,
    "country": "Norway"
}

person.update({"age": 50})

print(person) #  output: {'name': 'Bob', 'age': 50, 'country': 'Norway'}

#  This is also possible

first = {
    "name": "Bob",
    "age": 45,
    "country": "Norway"
}

second = {
    "name": "John",
    "age": 50,
    "country": "Norway"
}

first.update(second)

print(first) #  output: {'name': 'John', 'age': 50, 'country': 'Norway'}
```

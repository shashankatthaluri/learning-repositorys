 # Classes 📐

- In Python, a class is like a blueprint for creating objects. 🏗️
- Objects are instances of a class, and each object can have attributes and methods. 🧑‍💻

## Defining a Class 📝

- You can define a class using the class keyword. 🕵️‍♂️

```python
class Person:
    pass
```

## Creating an Object 🛠️

- Once you have a class, you can create an object or instance of that class. 🆕

```python

person1 = Person()
```

## Adding Attributes 📌

- You can add attributes to a class to represent data. 📊

```python
class Person:
    def __init__(self, name, age, country):
        self.name = name
        self.age = age
        self.country = country
```

## Using the Class with Dictionaries 🧑‍💼

- Classes can be used to create objects that resemble dictionaries. 🤝

```python
person = Person(name="Bob", age=45, country="Norway")
```

## Dictionary Methods in Classes 🔧

- Now, let's integrate dictionary methods into our class. 🔄
```python
class Person:
    def __init__(self, name, age, country):
        self.data = {
            "name": name,
            "age": age,
            "country": country
        }

    def clear_data(self):
        self.data.clear()

    def copy_data(self):
        return self.data.copy()

    def fromkeys_data(self, keys, value):
        return dict.fromkeys(keys, value)

    def get_age(self):
        return self.data.get("age")

    def pop_age(self):
        self.data.pop("age")

    def popitem_data(self):
        self.data.popitem()

    def update_age(self, new_age):
        self.data.update({"age": new_age})
```

## Using the Class Methods 🚀

- Let's use our class methods to manipulate the data. 🔄

```python
# Creating a person object
person = Person(name="Bob", age=45, country="Norway")

# Clearing data
person.clear_data()
print(person.data)  # Output: {}

# Copying data
copy_of_data = person.copy_data()
print(copy_of_data)  # Output: {'name': 'Bob', 'age': 45, 'country': 'Norway'}

# Using fromkeys
keys = ['name', 'age', 'country']
default_value = 'unknown'
fromkeys_result = person.fromkeys_data(keys, default_value)
print(fromkeys_result)  # Output: {'name': 'unknown', 'age': 'unknown', 'country': 'unknown'}

# Getting age
age = person.get_age()
print(age)  # Output: 45

# Popping age
person.pop_age()
print(person.data)  # Output: {'name': 'Bob', 'country': 'Norway'}

# Popping last item
person.popitem_data()
print(person.data)  # Output: {'name': 'Bob', 'age': 45}

# Updating age
person.update_age(50)
print(person.data)  # Output: {'name': 'Bob', 'age': 50, 'country': 'Norway'}
```

- Now, you have a class with dictionary-like functionality using various dictionary methods. 🎉

# Lists 📝

- Lists are an ordered list of elements 📚
- Lists can include any type of data, even other lists. 🔄
- Lists are mutable, meaning they can be changed. 🛠️

```python
# list of numbers
numbers = [1, 2, 3, 4, 5]

# list of mixed data types
mixed = [1, 'John', 2, 'Bob', 3, 'Mosh', 4, 'Sarah', 5, 'Mary']
```

## Check Length of a List 🔍

```python
# check length of a list
numbers = [1, 2, 3, 4, 5]
print(len(numbers))  # Outputs 5
```

## List of Numbers from 1 to 99 🎯

```python
nums = list(range(1, 100))
print(nums)
```

## Accessing Items in a List 🔑

```python
# access items in a list
numbers = [1, 2, 3, 4, 5]
print(numbers[0]) # Outputs 1
print(numbers[1]) # Outputs 2
```

## Check if a Value is in a List 🕵️

```python
# check if a value is in a list
numbers = [1, 2, 3, 4, 5]
print(1 in numbers) # Outputs True
print(6 in numbers) # Outputs False
```

## Iterating Over a List ➿

```python
# For Loop
numbers = [1, 2, 3, 4, 5]
for number in numbers:
    print(number)

# While Loop
i = 0
while i < len(numbers):
    print(numbers[i])
    i += 1
```

## Nested Lists 🧩

- Nested lists are lists that contain other lists.
- Perfect for encapsulating data in a tabular form.
```python
# nested lists
nested_list = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
print(nested_list[0][1]) # Outputs 2

# for loop
for l in nested_list:
    for val in l:
        print(val)
```

# List Methods 🛠️

## Append: Add item to your list ➕

- If you want to add an item to the end of a list, use `append`.
- Remember it takes only one value as argument. 


```python
numbers = [1, 2, 3]
numbers.append('pink')
print(numbers)  # Outputs [1, 2, 3, 'pink']
```

## Extend: Add Multiple Items to the End of a List 📈

- If you want to add multiple items to the end of a list, use `extend`. 
- It takes a list as an argument. 

```python
first_list = [1, 2, 3]
second_list = [4, 5, 6]
first_list.extend(second_list)
print(first_list)  # Outputs [1, 2, 3, 4, 5, 6]
```

## Insert: Add an Item at any Given Position 🔀

- If you want to add an item at a given position, use `insert`.
- It takes two arguments: the index and the value (Index: the position you want to add and value: whats the value).

```python
numbers = [1, 2, 3]
numbers.insert(0, 'pink')
print(numbers)  # Outputs ['pink', 1, 2, 3]

# Trick to insert at the last position
numbers.insert(len(numbers), 'pink')
print(numbers)  # Outputs ['pink', 1, 2, 3, 'pink']
```

## Clear: Remove All Items from a List 🧹

- If you want to remove all items from a list, use `clear`.

```python
numbers = [1, 2, 3]
numbers.clear()
print(numbers)  # Outputs []
```

## Pop: Remove an Item from a List and Return It ✂️

- If you want to remove an item from a list and return it, use `pop`.
- It takes one optional argument, the index of the item to be removed. If no index is specified, it removes the last item.

```python
numbers = [1, 2, 3]
popped_item = numbers.pop()
print(popped_item)  # Outputs 3
print(numbers)  # Outputs [1, 2]
```

## Remove: Remove a specific Item from a List ❌

- If you want to remove a specific item from a list, use `remove`.
- It takes one argument, the value of the item to be removed.
- If there are multiple items with the same value, it will remove the first one.

```python
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
numbers.remove(5)
print(numbers)  # Outputs [1, 2, 3, 4, 6, 7, 8, 9, 10]
```

## Index: Find the Index of an Item in a List 🔍

- If you want to find the index of an item in a list, use `index`.
- It takes one argument, the value of the item to be found.
- You can also specify the start and end index for the search.

```python
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
print(numbers.index(5))  # Outputs 4

# specify start and end index
nums = [1, 2, 3, 4, 5, 6, 7, 8, 8, 9, 10]
print(nums.index(8, 8, 10))  # Outputs 8
```

## Count: Count the Number of Times an Item Appears in a List 🔢

- If you want to count the number of times an item appears in a list, use `count`.
- It takes one argument, the value of the item to be counted.

```python
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 8, 9, 10]
print(numbers.count(8))  # Outputs 2
print(numbers.count(11))  # Outputs 0
```

## Reverse: Reverse the Order of Items in a List 🔄

- If you want to reverse the order of items in a list, use `reverse`.

```python
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 8, 9, 10]
numbers.reverse()
print(numbers)  # Outputs [10, 9, 8,

 8, 7, 6, 5, 4, 3, 2, 1]
```

## Sort: Sort the Items in a List 🔢

- If you want to sort the items in a list, use `sort`.
- It doesn't take any arguments.
- It will sort the list in ascending order by default.
- To sort in descending order, use the `reverse=True` argument.

```python
numbers = [5, 2, 7, 4, 0, 9, 8, 6, 1, 3]
numbers.sort()
print(numbers)  # Outputs [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]

# sort in descending order
numbers.sort(reverse=True)
print(numbers)  # Outputs [9, 8, 7, 6, 5, 4, 3, 2, 1, 0]
```

## Join: Join the Items in a List ⛓️

- `join` is a string method, not a list method.
- It is used to join the items in a list into a single string.
- The string used to call `join` is placed between each list item.

```python
words = ['Coding', 'is', 'fun']
sentence = ' '.join(words)
print(sentence)  # Outputs 'Coding is fun'

friends = ['John', 'Bob', 'Mosh']
friends_str = ', '.join(friends)
print(friends_str)  # Outputs 'John, Bob, Mosh'
```

## Slicing: Get a Subset of a List 🔪

- Slicing is a way of making a copy of a list.
- It takes two arguments: the start index and the end index.
- It returns a new list with the items from the start index to the end index.
- You can also specify a step value.

```python
colors = ['red', 'orange', 'yellow', 'green', 'blue', 'indigo', 'violet']
print(colors[0:3])  # Outputs ['red', 'orange', 'yellow']
print(colors[:3])   # Outputs ['red', 'orange', 'yellow']
print(colors[3:])   # Outputs ['green', 'blue', 'indigo', 'violet']
print(colors[::2])  # Outputs ['red', 'yellow', 'blue', 'violet']
print(colors[::-1]) # Outputs ['violet', 'indigo', 'blue', 'green', 'yellow', 'orange', 'red']
```

### Tricks with Slicing 🎩

```python
# Reverse a list
colors = ['red', 'orange', 'yellow', 'green']
reversed_colors = colors[::-1]
print(reversed_colors)  # Outputs ['green', 'yellow', 'orange', 'red']

# Modify every third element
colors[::3] = ['1', '2']
print(colors)  # Outputs ['1', 'orange', 'yellow', '2']

# Reverse the third element
reversed_third_element = colors[3][::-1]
print(reversed_third_element)
```

## Swapping Values in Lists ↔️

- Swapping values in a list is straightforward.
- It is often used in shuffling, sorting, or algorithms.

```python
names = ['James', 'Michelle']
names[0], names[1] = names[1], names[0]
print(names)  # Outputs ['Michelle', 'James']
```

## Creating a List of Even Numbers (List Comprehension) 🌟

Given a list `[1, 2, 3, 4, 5, 6]`, create a new variable called `answer2`, which is a new list of all the even values.

```python
original_list = [1, 2, 3, 4, 5, 6]
answer2 = [num for num in original_list if num % 2 == 0]
print(answer2)  # Outputs [2, 4, 6]
```

# Mastering Variables in Python 🛠️
## 📦 Variables

````markdown
Variables act as containers, holding various data values.

- They need to be given a value before they can be used.
- Changing and reassigning values is allowed.
- Variables can hold different types of data.


```Python
current_value = 7
result = current_value * 2  # Outputs 14
print(current_value)  # Outputs 7
```
````

### 🔄 Variable Assignment

You can link one variable to another.

```Python
current_value = 7
next_value = current_value
print(next_value)  # Outputs 7
```

### 🆕 Reassignment

Variables can undergo a transformation with new values.

```Python
current_value = 7
print(current_value)  # Outputs 7
current_value = 14
print(current_value)  # Outputs 14
```

### 🚀 Multiple Assignment

Assign multiple variables in a single go.

```Python
x, y = 7, 14
print(x)  # Outputs 7
print(y)  # Outputs 14
```

## ✏️ Naming Variables

Selecting the right names for variables is key.

- Begin with a letter or an underscore.
- Use letters, numbers, and underscores only.
- Keep in mind the case sensitivity (cats vs Cats).

### 📚 Naming Conventions

- Choose `snake_case` for most variable names. (snake_case: Itsnaming convention in which each space is replaced with an underscore (_) character, and words are written in lowercase.)
- Opt for  `CAPITAL_SNAKE_CASE` for constants.
- Go with `UpperCamelCase` for classes.
- Aviod variables with double underscores (`__like_this__`).

## 🧵 String Concatenation

Merging strings with `+` and repeating with `*`.

- `+` combines strings.
- `*` repeats strings.

```Python
name = "Alice"
print("Hello " + name)  # Outputs Hello Alice
print(name * 3)  # Outputs AliceAliceAlice
```

### 🚫 Mixing Types

Avoid directly combining strings and numbers.

- `"5" + "apples"` results in an error.

### 💬 String Formatting

Embed variables with placeholders.

```Python
apples = 5
formatted = f"I have {apples} apples!"  # Using f-string
# or
formatted = "I have {} apples!".format(5)  # Using format()
```

## 🔗 Interpolation

Integrate variables into strings with f-strings.

```Python
name = "Alice"
print(f"Hello {name}")  # Outputs Hello Alice
```

## 🔢 Strings & Indices (Indexes)

Strings in Python are indexed, with each character having a designated position.

```Python
word = 'Python'
first_letter = word[0] # 'P'
second_letter = word[1] # 'y'
```

### 📍 Accessing Characters

Access specific characters in a string using their index.

```Python
name = "Python"
print(name[0]) # Outputs 'P'
print(name[3]) # Outputs 'h'
```

### ✂️ Slicing Strings

Obtain parts of strings by slicing with indices.

```Python
name = "Python"
slice = name[0:3] # 'Pyt'
print(slice)
```

### 🔄 Reverse Indexing

Use negative numbers to start from the end of the string.

```Python
name = "Python"
last_letter = name[-1] # 'n'
second_last = name[-2] # 'o'
```

## 🛑 Important Notes on String Usage

- Stay consistent with single (`' '`) or double (`" "`) quotes.
- Escape quotes inside strings with a backslash (`\"` or `\'`).

```Python
quote = "He said, \"Python is awesome!\""
conversation = 'She replied, \'I agree!\''
```

- Triple quotes are handy for strings spanning multiple lines.

```Python
multi_line_string = """This is a string
that spans across multiple lines
in the Python script."""
```

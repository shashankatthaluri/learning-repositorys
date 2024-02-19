# Reading and Writing files 🧰

- process of reading and writing to a file is like finding a book and opening a book.
- First, the file is located, opened to the first page, then reading/writing begins until it reaches
the end of the file. 🔧

## open( ) 🧹

- open( ) returns a file object, and is most commonly used with two arguments:

```python
open(filename, mode)
```
- mode is describing the way in which the file will be used. mode can be:
    - 'r' when the file will only be read,
    - 'w' for only writing (an existing file with the same name will be erased),
    - 'a' opens the file for appending; any data written to the file is automatically added to end.
    - 'r+' opens the file for both reading and writing.
    - 'b' appended to the mode opens the file in binary mode: now the data is read and written in the form of bytes objects. This mode should be used for all
    files that don’t contain text.

The mode argument is optional; 'r' will be assumed if it’s omitted.

- Normally, files are opened in text mode, that means, you read and write strings from and to the file, which are encoded in a specific encoding.
- If encoding is not specified, the default is platform dependent (see open()).

## Good practice 🔧
It is good practice to use the with keyword when dealing with file objects. The advantage is that the file is properly closed after its suite finishes, even if an exception is raised a some point. Using with is also much shorter than writing equivalent try-finally blocks:

## Open files "without" using `with` statement:

```python
# Open files without using 'with' statement.
    file = open('src/files/file_name.txt', 'r') #'src/files/file_name.txt' is file path 

    assert not file.closed

    read_data = file.read()

    assert read_data == (
        'first line\n'
        'second line\n'
        'third line'
    )

    file.close()

    assert file.closed
```
## Open file using `with` statement: 

```python
# Open file using with.
    with open('src/files/file_name.txt', 'r') as file:
        read_data = file.read()

        assert read_data == (
            'first line\n'
            'second line\n'
            'third line'
        )

    assert file.closed
```

- If you’re not using the with keyword, then you should call f.close() to close the file and immediately free up any system resources used by it. If you don’t explicitly close a file, Python’s garbage collector will eventually destroy the object and close the open file for you, but the file may stay open for a while.
-  Another risk is that different Python implementations will do this clean-up at different times.


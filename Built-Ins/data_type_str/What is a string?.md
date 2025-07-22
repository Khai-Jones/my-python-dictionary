A string is an *immutable* object in Python. It can contain letters, numbers, symbols, or any characters as text. 

Most programs use strings in some shape or form. It's usage can range from user input/output, data formats, file paths, filenames, identifiers, etc. 


A string is created with "". 

``` python
string_val = "Hello World"
```

A string has 48 utility methods, which are used to manipulate or inspect strings. All uses of methods for strings return a new string.

### Case & Format manipulation

- [[-.upper()]], [[-.lower()]], `capitalize`, `title`, `swapcase`, `casefold
- center, ljust, rjust, zfill, format, format_map
### Search and Find
- find, rfind, index, rindex, startswith, endswith

### Content checks (boolean tests)

- isalnum, isalpha, isascii, isdigit, isnumeric, isdecimal
- islower, isupper, isspace, istitle, isidentifier, isprintable
### Modification/cleanup

- strip, lstrip, rstrip, replace, removeprefix, removesuffix
- split, rsplit, splitlines, partition, rpartition, expandtabs, translate

### Encoding
- encode, maketrans


### Joining
- join
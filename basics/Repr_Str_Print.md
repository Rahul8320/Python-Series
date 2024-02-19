# repr | str | print

All three, repr, str, and print, deal with displaying information in Python, but they each have distinct purposes:

### repr:

    - Stands for "representation."
    - Returns an unambiguous string representation of an object, meant to be reproducible.
    - Often includes quotes, escape characters, and class information.
    - Useful for debugging as it shows the exact syntax to recreate the object.

### str:

    - Stands for "string."
    - Returns a human-readable string representation of an object, meant to be understandable.
    - Prioritizes clarity over exactness, omitting unnecessary details.
    - Used for general output when you want the information to be clear for users.

### print:

    - Not a function, but a built-in statement.
    - Takes any number of expressions and prints their string representations (using str by default) to the console.
    - Convenient for displaying output during program execution.

## Example:

```python
>>> my_list = [1, "hello", 3.14]
>>> repr(my_list)
"[1, 'hello', 3.14]"
>>> str(my_list)
"[1, 'hello', 3.14]"
>>> print(my_list)
[1, 'hello', 3.14]
```

```python
>>> username = "learning_python"
>>> repr(username)
"'learning_python'"
>>> str(username)
'learning_python'
>>> print(username)
learning_python
```

Here's a table summarizing the key differences:

| Feature       | repr                          | str                      | print                |
| ------------- | ----------------------------- | ------------------------ | -------------------- |
| Purpose       | Unambiguous                   | Human-readable           | Display to console   |
| Output format | Exact, detailed               | Clear, simplified        | Varies (str default) |
| Use cases     | Debugging, recreating objects | User output, readability | Simple display       |

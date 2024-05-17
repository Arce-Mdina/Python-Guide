## Python Comments
Comments are lines of text that will be ignored by Python when executing. This is useful to clearly split your code into a more readable manner or for debugging, such as when you want to know your mistakes, you can comment lines of code so that they are not executed anymore and you can work out what is wrong.

Python comments start with `#`. This indicates to Python that it should ignore the rest of the line. 

You can easily make text or code comments by using the shortcut `⌘ + /` on a Mac, or `^ + /` on a Windows.

## Python Indentation
Indented code:
```python
if x == true:
  print("x is true")
```

Non-indented code:
```python
if x == true:
print("x is true")
```

See the difference? For the first line, the print function is indented, indicating to Python that it is a block of code and belongs to the previous non-indented code (in this case is the `if` statement).

In addition, Python will give you an error if you incorrectly indent a line of code.

The indentation space is up to the programmer, but it must be indented and make sure it is readable!

```python
# This still works
if x == true:
      print("x is true")
```

## Python Assignment
You can assign something in Python using the equal sign (`=`).
```python
num = 2
text = "Hi!"

# The value could be anything, and so can the variable name be anything.
# Make sure every time you are making a variable, it is readable and understandable to you
```

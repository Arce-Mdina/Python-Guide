## Python Output
We can output data by using the `print()` function. 
```python
print("Hello world!")

# Output: Hello world!
```
This function outputs whatever is between the brackets - for strings it removes the quotation marks.

This can also be used for variables.
```python
x = 4
print(x)
# Output: 4
```
### f-strings
There is something in Python called the f string, which is basically an easier to output something when a string needs one or more variable's data within it.

```python
x = input("What is your favourite color?")

print(f"Your favourite color is {x}")
```


## Python Input
In Python, you can allow the user to input something using the `input()` function.
```python
name = input("Enter your name: ")
```

You can also let users enter a number
```python
x = int(input("Enter a number: ")) # This tells Python that the data entered is an integer
y = float(input("Enter a number with 1 decimal")) # This tells Python that the data entered is a float
```

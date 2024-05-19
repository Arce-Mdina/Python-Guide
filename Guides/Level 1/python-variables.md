## What are Variables?
You can think of a variable as a space for storing data, much like your drawers storing your stationary and notebooks!

## Creating Variables
In Python, you can create a variable but just assigning to it (equal sign `=`).

Python does not really care about the type of data you assign it to, you can even change it afterwards!

```python
name = "Sally"
name = 'John'
print(name)

# Output: John
# This is because the second assignment overrided the first value.
# ------------
# Please also note that using single or double quotes for strings (text) is the same to Python
# ------------
```

## Casting
Casting is a method where you want to specify a type of data to a piece of data or value. 

For example:
```python
value = str(1134) # value = '1134'
value = int(1134) # value = 1134
value = float(1134) # value = 1134.0
```
### Further examples

For strings:
```python
x = str(3) # x = '3'
y = str(3.6) # y = '3.6'
z = str("Hello world!") # z = "Hello world!"
```

For integers:
```python
x = int(3) # x = 3
y = int(3.6) # y = 3
z = int("2") # z = 2
```

For floats:
```python
x = float(3) # x = 3.0
y = float(3.6) # y = 3.6
z = float("3.573946592") # z = 3.573946592
```


## Testing the Type
You can check the type of data a variable is storing by using the `type` function.
```python
x = 4.0
print(type(x)) # Output: float
```
You can see our data types file [here](https://github.com/Arce-Mdina/Python-Guide/blob/main/Guides/Level%201/python-data-types.md)

## Case Sensitivity
Python is case sensitive, meaning that a variable named `a` and `A` is not the same.

## Variable Naming
Believe it or not, but Python does have restrictions to variable naming.

Python variables:
- must start with a letter or underscore
- can only contain alpha-numeric characters and underscores
- cannot start with a number
- cannot be the same as any of the [Python keywords](https://github.com/Arce-Mdina/Python-Guide/blob/main/Guides/Level%201/python-keywords.md)

<details>
  <summary>Correct Python variables</summary>
  
  ```python
  var4 = "string"
  _var_var = "string"
  var = "string"
  ```
</details>

<details>
  <summary>Variable names that causes errors</summary>
  
  ```python
  4var = "string"
  global = "string"
  var-var = "string"
  var var = "string"
  ```
</details>

## Multiple Values, Multiple Variables
Python allows you to assign multiple variables with different values in one line.

```python
fruit_1, fruit_2, fruit_3 = "apple", "banana", "orange"

print(fruit_1)
print(fruit_2)
print(fruit_3)

# Output: apple // banana // orange
```

## One Value, Mutiple Variables
Python allows you to assign the same value to different variables.

```python
num = num_1 = num_2 = 1134

print(num_1)

# Output: 1134
```

## Unpacking
Python allows you to extract the values from a list, tuples etc. by using different variables.

```python
my_list = [1, 4, 8]
x, y, z = my_list

print(y)
# Output: 4
```

## Outputting Variables
You can output variables by using the `print()` function. 

```python
x = "Hello world!"

print(x)
# Output: Hello world!
```

You can also add **variables that have the same type of data** together using the `+` operator.

You can combine a number variable to a string variable by using the `,` operator.

```python
x = "Hello"
y = "world!"

print(x + y)
# Output: Hello world!

print(x, y)
# Output: Hello world!

# If you are adding two variables which its data type is integers or floats, Python is going to add them together when outputted
```

# Global Variables
These are variables that could be used anywhere in the program. In most occasions, these are declared outside of a loop or a function.

When you create a variable inside a function or a loop, the variable is local, meaning that it could be used by anything else outside of that loop or function. But the `global` keyword in Python allows the variable to globally declared, whether it is in a function or loop. This is good if you want to change a variable's value inside a function.

```python
x = 5

def func():
  global x
  x = 4

func()

print(x)
# Output: 4
```

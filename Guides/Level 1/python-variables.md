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

## Testing the Type
You can check the type of data a variable is storing by using the `type` function.
```python
x = 4.0
print(type(x)) # Output: float
```

## Case Sensitivity
Python is case sensitive, meaning that a variable named `a` and `A` is not the same.

## Variable Naming
Believe it or not, but Python does have restrictions to variable naming.

Python variables:
- must start with a letter or underscore
- can only contain alpha-numeric characters and underscores
- cannot start with a number
- cannot be the same as any of the Python keywords (list below)

<details>
  <summary>Correct Python variables</summary>
  
  ```python
  var4 = "string"
  _var_var = "string"
  var = "string"
  ```
</details>

<details>
  <summary>Python variables errors</summary>
  
  ```python
  4var = "string"
  global = "string"
  var-var = "string"
  var var = "string"
  ```
</details>

___
<details>
  <summary>Python Keywords</summary>

  | Keyword (Python) | Description/Function |
  | ---------------- | -------------------- |
  | and              | Logical operator     |
  | as               | Creating an alias    |
  | assert | Debugging |
  | break | Breaking out of a loop |
  | class | Defining a class |
  | continue | Continue to the next iteration of the loop |
  | def | Defining a function |
  | del | Deleting an object |
  | elif | A conditional statement; same as else if |
  | else | A conditional statement |
  | except | Tells Python what to do if an exception happens |
  | False | Boolean value |
  | finally | Tells Python to execute a block of code no matter the exception |
  | for | To create a for loop |
  | from | Used when importing a specific package or thing |
  | global | Declaring a global variable |
  | if | To make a conditional statement |
  
</details>
___

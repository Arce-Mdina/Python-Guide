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

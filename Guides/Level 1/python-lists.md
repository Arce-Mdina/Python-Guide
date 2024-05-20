# Python Lists
Lists are used for storing multiple values in one variable. They can contain more than one data type! See all the data types in Python [here](https://github.com/Arce-Mdina/Python-Guide/blob/main/Guides/Level%201/python-data-types.md)

They are created with square brackets `[]`.

List items are changeable (this means that we can add, remove, or change items within a list after it has been created), ordered (meaning that the order will not change, if anything new is added it will be placed at the end of the list) and they even allow duplicates (this is because lists are indexed so they allow duplicates of values)!

### Length of a list
We can the `len()` function to determine the length of a list

## Accessing List Items
A list is indexed, therefore we can refer to the index number to access a specific value. **Please note that the index numbers start with `0` not `1`.**

```python
mylist = ['Hello' 'world', 'John']

print(mylist[1]) # Output: ['world']
```

We can also refer the indexes as negative numbers, but this time it counts from the end of the list. **Please note that `-1` refers to the last item, `0` would still the be the first counting from the start.**

```python
mylist = ['Hello' 'world', 'John']

print(mylist[-1]) # Output: ['John']
```

### Range of Indexes

Python also allows us to do range of indexes. 

```python
mylist = ['Hello' 'world', 'John', 'Cherry', 1, 4, 6, 2, 78, True]

print(mylist[3:5]) # Output: ['Cherry', 1] (Index 3 is included in the list but index 5 is not)
```

We can also leave out the first value in a range. This will tell Python that it should start at the start of the list and then go up to (excluding) the second value.

```python
mylist = ['Hello' 'world', 'John', 'Cherry', 1, 4, 6, 2, 78, True]

print(mylist[:5]) # Output: ['Hello' 'world', 'John', 'Cherry', 1]
```

We can leave out the second value in range. This tells Python that it should continue to the end of the list.
```python
mylist = ['Hello' 'world', 'John', 'Cherry', 1, 4, 6, 2, 78, True]

print(mylist[3:]) # Output: ['Cherry', 1, 4, 6, 2, 78, True]
```

We can also do a range of negative indexes. This is the same thing, but instead of counting from the start, it counts from the end.

## Check if item exists in a list
We can use the `in` keyword in Python to determine if a value is in a list.

```python
mylist = ['Hello' 'world', 'John', 'Cherry', 1, 4, 6, 2, 78, True]

if 4 in mylist:
  print(True)
```

## Changing Items in a list
You can change a value of in a list by referring to its index number.
```python
mylist = ['Hello' 'world', 'John', 'Cherry', 1, 4, 6, 2, 78, True]

print(mylist[4]) # Output: 1

mylist[4] = False

print(mylist[4]) # Output: False
```

### Change a range of values
You can change a range by specifying that range and specifying the changes. If you insert more than the range, the new items will be inserted at the specified range, and the items after it will shift accordinly. This is the same if you insert less than the range.
```python
mylist = ['Hello' 'world', 'John', 'Cherry', 1, 4, 6, 2, 78, True]
mylist[2:9] = [False]

print(mylist) # Output: ['Hello' 'world', False, 78, True]
```

## Adding Items in a list

### insert()
You can use the insert function to insert it. Specify the index to insert it at that position.

```python
mylist = ['Hello' 'world', 'John', 'Cherry', 1, 4, 6, 2, 78, True]

mylist.insert(2, "Ben")
print(mylist) # Output: ['Hello' 'world', "Ben", 'John', 'Cherry', 1, 4, 6, 2, 78, True]
```

### append()
You can use the `append` function to add a new list item to the end of the list

```python
mylist = ['Hello' 'world', 'John', 'Cherry', 1, 4, 6, 2, 78, True]

mylist.append("apples")

print(mylist) # Output: mylist = ['Hello' 'world', 'John', 'Cherry', 1, 4, 6, 2, 78, True, "apples"]
```

### extend()
You can use the extend() function to extend a list. This function to connect two lists together. 

```python
mylist = ['Hello' 'world', 'John', 'Cherry']
mylist_2 = [1, 4, 6, 2, 78, True]

mylist.extend(mylist_2)
print(mylist) # Output: ['Hello' 'world', 'John', 'Cherry', 1, 4, 6, 2, 78, True]
```
This function could also be used for tuples, dictionaries etc.

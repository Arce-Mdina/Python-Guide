**Challenge:** Building a program where it tells whether two given strings are anagrams

**Skills required:** Basic input & output; variables; if statements; built-in functions

**Possible Solution**:
```python
string1 = input("Enter the first string: ")
string2 = input("Enter the second string: ")

str1 = ''.join(sorted(string1.lower()))
str2 = ''.join(sorted(string2.lower()))

if str1 == str2:
  print(f"\n{string1} and {string2} are anagrams.")
else:
  print(f"\n{string1} and {string2} are not anagrams.")
```

**Challenge:** Building a program where it tells whether a given line of text is a palindrome or not.

**Skills required:** Basic input & output; variables; if statements; Built-in functions

**Possible Solution**:
```python
word = input('Enter a text: ')
word_2 = word.lower()
reverse_word = word_2[::-1]


if word_2 == reverse_word:
  print(f'{word} is a palindrome')
else:
  print(f'{word} is not a palindrome')
```

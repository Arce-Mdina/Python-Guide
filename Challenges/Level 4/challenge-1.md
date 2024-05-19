**Challenge:** Building a program where it shows an entered number of mulitiplication questions that goes up to 12.

**Skills required:** Basic input & output (f-strings if you want); variables; if statements; for loops; Modules & Packages

**Possible Solution**:
```python
import random

score = 0

questions_num = int(input("Enter how many questions you want: "))

for x in range(questions_num):

  num_1 = random.randint(1, 12)
  num_2 = random.randint(1, 12)
  
  correct_answer = num_1 * num_2
  
  answer = int(input(f"{num_1} * {num_2} = "))

  if correct_answer == answer:
    print('Correct. \n')
    score = score + 1
  else:
    print(f'The answer is {correct_answer}. \n')

print(f'\nYour score is {score}/5.')
```

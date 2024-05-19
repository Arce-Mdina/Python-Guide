**Challenge:** Building a program where a user has 5 tries to guess a random number between 1 and 100

**Skills required:** Input & output; variables; loops (while); if statement; modules; 

**Possible Solution**:
```python
import random

𝑥 = random.randint(1, 100)

guesses_left = 5

while guesses_left > 0:
  player_guess = int(input("Enter a number between 1 and 100: "))

  if player_guess == 𝑥:
    print("You have correctly guessed the CPU's number")
    break
  else:
    guesses_left -= 1

  if player_guess > 𝑥:
    print("Think lower")
  elif player_guess < 𝑥:
    print("Think higher")
    
if guesses_left == 0:
  print(f"You ran out of tries. The number was {𝑥}")
```

# Number Guessing Game

## Introduction

In this game, the user will try to guess a number between a minimum and maximum range. The game will limit the number of chances a user has to guess the right number. If they guess correctly before their tries run out, they win!

**Example**

![Example Image](https://media.geeksforgeeks.org/wp-content/uploads/20200827185026/Outputsforguessinggame.JPG)

## Instructions

### Steps

- Ask the user what their minimum and maximum bounds are. Store those values as variables
- Generate and store a random number using the `random` Python package
- Ask the user to guess a number until they guess correctly or run out of tries.
- If the number is higher or lower than the correct number, notify the user.
- If the user wins, print a message to the user with the number of tries it took them to win
- If the user loses, tell the user that they suck :)

### Considerations

- Ensure that the maximum bound is greater than the minimum bound
- All inputs must be integers (bounds and guesses)
- For repetitive guessing, a while loop will be used
- If the number guessed is out of range, notify the user

### Helpful tips

To receive an integer input from the user use

```python
user_input = int(input("Enter a number: "))
```

To force leave a while loop you can use

```python
break
```

This is useful for ending the game.

For generating random numbers within a range, use the `random` Python package.

```python
import random

# Generates a random number between 6 and 10
rand_num = random.randint(6, 10)
```

When determining the maximum number of tries a user will have, you can either set it manually, or for an extra challenge, you can dynamically set it using the formula

```
Maximum tries = log2(Upper bound – lower bound + 1)
```

To do this, once the bound is set use

```python
import math

maximum_tries = round(math.log(upper - lower + 1, 2))
```

Want the answer?

[Solution with Source Code](https://www.geeksforgeeks.org/number-guessing-game-in-python/)

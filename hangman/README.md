# Hangman Game

## Introduction

It's Hangman. The user has to fill in the word by guessing the letters in that word. If they guess the wrong letter three times, they lose.

```python
# Word: hello

Welcome to Hangman. Find the word by guessing the letter.
You can only guess a wrong letter 2 times.

_ _ _ _ _

Guess a letter: l

_ _ l l _

Guess a letter: z

No 'z' found. You have 1 more wrong attempt.

Guess a letter: o

_ _ l l o

...

Guess a letter: h

h e l l o

You win!
```

## Instructions

### Steps

- Store a list of possible words to choose from. When the game starts, choose a word from the list at random and print the blanks for that word
- When letters are inputted, fill in the blanks that contain that letter. If letter not found in word, notify the user.
- If user runs out of attempts, end the game and notify user.
- If user fills in all the blanks, end the game

### Considerations

### Helpful tips

To select a random word from the list of possible words use

```python
import random

word = random.choice(possibleWords)
```

Want the answer?

[Solution with Source Code](https://www.geeksforgeeks.org/hangman-game-python/)

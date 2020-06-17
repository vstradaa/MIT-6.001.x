# MIT 6.001.X Computer Science 

## - Victor E. 06/05/2020

# Simple Algorithms

# Approximate Solutions

You can approximate a solution by incrementing by really small numbers. Subtracting the new number by the answer will reveal the difference. You can compare this to the tolerance you set to see whether it should continue to execute or not. 

# Bissection Search

A better way to find numerical solutions is to do bissection searches which eliminate half the answers each time. It will basically guess and if the guess is too low, it will discard the numbers below that. And if too high, it will discard the numbers above. 

## Bissection Search

```python
# Bissection Search
# Guess my num
print("Pick a number between 0-100")
guessTrue = False
beginningNum = 0 
endNum = 100
compGuess = round((beginningNum + endNum)/2)
guesses = 0
while not guessTrue:
    guesses += 1
    compGuess = round((beginningNum + endNum)/2)
    ans = input("Is your number " + str(compGuess) + "?")
    if ans == "l": # TOO LOW
        beginningNum = compGuess
    elif ans == "h": # TOO HIGH
        endNum = compGuess
    elif ans == "c": # CORRECT
        guessTrue = True
        print("Game over, your number is " + str(compGuess) + " and it took " + str(guesses) + " tries!")
```
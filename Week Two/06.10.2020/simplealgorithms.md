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

# Floats and Fractions

When working with floats it is important to keep in mind that most of the time, approximation is used when a computer intreprets numbers. 

## Binary 

Binary is in base 2. 

To get an understanding of how this works let's look at how we represent a decimal number. 

 <code>130 is the same as (10**2) + (3) * (10 ** 1) + (0) * (10 ** 0)</code>

So binary has a base of 2. So everything is a representation on bases of 2

so 130 in base 2 would be (2 ** 5) + 0 * (2 ** 4) + 2 * (2 ** 3) + 0 + 0 + 0  each extra 0 representing 0 times the corresponding base to the nth number in order. 

## Floats and Binary

When dealing with Floats, converting a number to Float might be exhaustive and sometimes conversion might only be done through approximation. 

To convert a decimal float to binary you must first multiply the decimal with a base 2 to the power of a number that will make it all a whole number. You will then turn that number into binary. And divide the binary number by the binary number of the base 2 to the number you chose. 

For example <code>.375</code> can be done by first multiplying that by 2 ** 3 which will give you 8. Find the binary version of (.375 * (2 ** 3)) and then divide it by the binary version of (2 ** 3) to get .375 in binary. 

To learn more about floats in greater detail check out:
* [Floats and Fractions (Binary)](https://www.youtube.com/watch?v=LpuPe81bc2w)



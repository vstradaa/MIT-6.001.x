# MIT 6.001.X Computer Science 

## - Victor E. 06/05/2020

# Core Elements of Programs

# Strings

A string is a sequence of characters. They can be represented by quotation marks or single quotes as such:

```python
hi = "hello there"
```

This is a new data type object which is not a Scalar Object! (Because it is a sequence of characters)

### Concatenation

Concatenation allows you to add together strings to make new strings!

```python

name = "Eric"
greeting = hi + " " + name # prints out "hello there Eric" Look at the previous code block for the value of variable "hi"
```

Also, <code> Overloading </code> is the term for when you use an operator on multiple types of operands. The type of operation that it performs is dependent on the datatype of these operands. For example, adding two ints will result in the summation of two ints. And adding two strings will result in the concatenation of two strings. 

As we get further along, we'll eventually be able to create our own overloadable operators using functions!

### Successive Concatenation

Successive concatenation allows you to basically multiply a string!

```python
3* 'Eric' # Will return to the console 'EricEricEric'
5* 'Eric' # Will return to the console 'EricEricEricEricEric'
```

### Length or len()

You can also see how many characters are in a string by using len()
```python
len('eric is') # console returns, '7' it also includes the space!
```
### Getting Elements from Strings

In Python since Strings are made of multiple characters, it makes sense that you can take out these individual characters. We can do this by using square brackets. 

```python
'myName'[1] #We'd like to think that number 1 would return the first character but it doesnt
```

the number within the brackets is called the 'index'. The index starts at 0 because to computers, the 0 is very useful. 

So the above code block would actually return 'y'

### Slicing or Getting Parts from the String

You can also get parts of a string such as the last 3 letters of your name by referencing a starting point and an end point, where the end point is not included.

For example:

```python
'myName'[1:3] # returns the index values from 1 to 2 not including the 3rd index
'myName'[3:] # returns everything after the 3rd index
'myName'[:4] # returns everything up to the 3rd index because it doesn't include the 4th index
'myName'[:]  # returns a copy of the whole string
```

Using this we can return parts of a string to a variable, function, etc.

# Input/Output

We use the keyword <code>print()</code> to print things to the console.

We can put a variable, expression, or a raw datatype in the the parenthesis

When printing we can only concatenate strings. If there's a number you'd like to add to your string you must use a comma instead of a plus symbol.

```python
print(3,"dogs are outside") #if there are ints/floats you want to concatenate to a string
```

### Input

If you're going to input something it's a good idea to bind it to a variable. To do this you can set a variable equal to <code>input()</code>.

```python
yourName = input()
```

Now input will only return a string. So if you want to input an int (not including floats) you have to cast it like so:

```python
yourAge = int(input())
```

# IDE'S

An Integrated Development Environment (IDE) and it allows you to edit and store files before you run them. It's a simple and easy way to write down code for later use/edits.

# Control Flow (while and for loops)

### While Loop

More advanced versions of control flow will use a while loop. A while loop will execute a block of code while a condition is true. 

#### Here's a game example:

Say you are playing a game where it asks you to turn left or right. If you turn right it will continue to ask you to turn left or right because you are still in the same spot according to the program. 

How do you translate this into a program?

```python
leftOrRight = input()

while (leftOrRight == "right"):
    leftOrRight = input()
print("game over!")
```
# For Loop

A for loop is made for when you know how many times a program will execute. 
You can end the program early with a <code>break</code> It even uses a counter!

You can also rewrite a for loop using a while loop

```python
mySum = 0;
for i in range(5,12,2):
    mySum += i
# if printed the answer will be the sum of every other number from 5 to (12 - 1)
```
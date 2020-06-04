# Scalar Objects

In Python there are data type objects called Scalars. These scalars are types with only one value. This would technically not include a String even though it's a data type object. However it is not a Scalar because in python a string is actually an array of characters!

<code>Int-</code> represent <code>integers</code>, ex. <code>5</code> 

<code>Float</code> - represent <code>real numbers</code>, ex. <code>3.27</code>

<code>Bool</code> - represent <code>booleans</code>, ex. <code>True</code> and <code>False</code>

<code>Int</code> - <code>special</code>, with only one value: <code>None</code>

You can use <code>type()</code> to see the type of object something is with the value going between the parenthesis.

## Here's two examples from the primitives listed above; 'Int' & 'Bool'

Int Example:

```python
In[1]: type("example text")
Out[1]: str
```

Bool Example:

```python
In[1]: type(True)
Out[1]: bool
```

# Type Conversions (Casting)

You can convert scalars to other types using 'casting' to do so. (preferrably with numbers)

```python
In[1]: float(3)
Out[1]: 3.0
```
```python
In[1]: int(3.9)
Out[1]: 3
```

Keep in mind that when downcasting a <code>float</code> to an <code>int</code> you are not rounding, you are simply removing the digits following the dot.

# Printing to the console

When using the command prompt you are only seeing the final returned values. If you have a program that executes multiple lines of code and you want a specific value to be printed on the console, you can use the <code>print()</code> method!

```python
In[1]: print(3+2)
Out[1]: 5
```

# Expression

combine objects(variables, etc) and operators (+,-,*,etc)

```python
<object><operator><object>
```

or

```python
i+j #the sum
i-j #the difference
i*j #the product
i/j #division
i//j #int division (result is int without remainder ex. 4.5 ==> 4)
i%j #the remainder when i is divided by j
i**j #i to the power of j
```

When operating with ints and floats the fuller form is what dominates. Meaning that if you add an int with a float the result will be a float. Think of it this way. 3.3 + 3 is going to be 6.3 so it makes sense that 3.00000000000001 + 3 equals 6.00000000000001 and by that knowledge 3.0 + 3 equals 6.0. If they're both ints then the answer is an int!

# Simple Operations

When doing operations in pythong remember PEMDAS! The python interpreter will follow these rules by heart and if you don't specify hierarchy, your code might fall with a semantic error (An unintended meaning is given to your program).

In normal operations without parenthesis, all code will be executed from left to write as you would in a normal math problem!

# Binding variables and values

The <code>=</code> sign is an assignment of a value to a variable. 

```python
pi = 3.14159
```

or

```python
pi_approx = 22/7
```

This value is stored in computer memory and can be called with a variable name.

The benefits of adding names to the values of expressions are:

* You can reuse names instead of values
* It's easier to change your code later. 

# Programming vs Math

In programming you don't solve for "X"
You have to define values for variables always!

```python
pi = 3.14159
radius = 2.2

# area of a circle

area = pi * (radius ** 2)

radius = radius + 1 # because radius was reassigned/updated after area, the area variable will not be reassigned/updated 
```

You can rewrite the last area reassignment in shorthand form by using <code>+=</code>

```python
radius += 1
```

# Comparison operators on int and float

This will give your program the ability to make decisions based on tests. These results will usually evaluate to true or false before moving on to the next part of the program

Here are some tests you can perform on two or more ints/floats:

```python
i > j # i is greater than j
i >= j # i is greater than or equal to j
i < j # i is less than j
i <= j # i is less than or equal to j

i == j # Equality test, True, if i equals j
i != j # Inequality test, True if i not equal to j
```

# Logic operators on bools

<code>not a</code> => True if a is false and False if a is True

<code>a and b</code> => True if both are True

<code>a or b</code> => True if either or both are True

# Branching Programs

A simple branching statement is a conditional

They have three different parts

1. A test (Expression that evaluates to True or False)

2. A block of code to execute if the test is True

3. An optional block of code to execute if the test is false

Remember that the block of code to execute for the false test results is not required!

```python
x = int(input('Enter an integer: '))

if x%2 == 0:
    print('')
    print('Even')

else:
    print('')
    print('Odd')
print('Done with conditional')
```

The above code is an example of a branching program using conditionals!
It includes an if statement that says that "if the remainder of x/2 is 0" then it will pring the two statements in it's code block.

else is for the false statement.

You write a branching program using if/else statements

```python

if(condition):
    #statement
else:
    #statement
#end of statement
```

Indentation is important! It tells the program when the if/else statement has ended.
You can also nest conditionals within conditionals such as the following:

```python
if x%2 == 0:
    if x%3 == 0:
        print('Divisible by 2 and 3')
    else:
        print('Divisible by 2 and not by 3')

elif x%3 == 0:
    print('Divisible by 3 and not by 2')
```




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

### Successive Concatenation

Successive concatenation allows you to basically multiply a string!

```python
3* 'Eric' # Will return to the console 'EricEricEric'
5* 'Eric' # Will return to the console 'EricEricEricEricEric'
```

### Length or len()


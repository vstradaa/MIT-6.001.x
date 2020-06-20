# Decomposition and Abstraction

## Decomposition

Decomposition is the act of taking an idea/program and breaking into smaller usable parts.

Different components work together to achieve an end goal. 


## Abstraction

Abstraction is knowing how a program works but not exactly knowing what's inside. This concept is very useful for turning ideas into code.

You typically know the input/output behavior

It's the idea that once something is built, I don't need to know what's inside. As long I know how it works.

## More
Will achieve decomposition via functions and later on via classes

We will also achieve abstraction by using function specifications and docstrings

Decomposition and abstraction are powerful together and can be reused multiple times to create clean and efficient code!

# Introducing Functions

In order to write a function you need to define a function using the keyword <code>def</code> followed with a name for the function; for example: <code>is_even</code>. You then follow that with two paranthesis with parameters in between. This is then followed by a semicolon. 

It is not required but highly recommended to use docstrings in order to describe what the program does (abstraction).

## formal vs actual parameters

<cod>Formal parameters</code> are made within the function you defined. When calling the function you are passing an <code>actual parameter</code>. 

It is important to note the scope of both. The scope of formal parameters is within the function only and the scope of actual paramters is outside of the function. When you are calling/invoking a function, you are passing an actual parameter into the function which then is used within the function. It will not change the value of the parameter. It will only take it in. 

##### In actual sense, the formal parameter gets bound to the actual parameter when a function is called. It's like binding a value to a variable. So if you have a function with a formal parameter of x the actual parameter will be bound to the formal parameter of x. So x will now be usable within the function. But not outside. 

#### It is also important to note that you can reference outside variables inside but you can not change them on the inside. The function will first check to see if a variable is inside before checking outside the scope to reference such a variable/data.

# Return vs Print

If there is no explicit return the default return value will be of <code>None</code> in which case it will return nothing to the one that's calling the function. 

You can only use a return inside of a function.

You can only use it once per function. 

The code inside a function but after the return statement will not be executed. 



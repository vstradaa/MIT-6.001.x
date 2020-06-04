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



<center><u><H1>Lists </H1></u></center>

In Python, a list contains multiple values in an ordered sequence. List are written within square brackets `[ ]`.  The elements in a list are separated with commas (comma-delimited).


```python
MyList=["a", "B", "b", "c", "a"]
```


```python
print(MyList)
```

    ['a', 'B', 'b', 'c', 'a']


We can modify the existing list by appending and extending elements to the list. We can do so using `append` and `extend` methods


```python
MyList.append("f")
print(MyList)
```

    ['a', 'B', 'b', 'c', 'a', 'f']



```python
MyList.extend("m")
print(MyList)
```

    ['a', 'B', 'b', 'c', 'a', 'f', 'm']


Lists can have different types of elements. They can contain floats, integers, strings, lists etc.


```python
MyList.append(['g', 'h'])
print(MyList)
```

    ['a', 'B', 'b', 'c', 'a', 'f', 'm', ['g', 'h']]



```python
MyNewList=['a', 'B', 'b', 'c', 'this is a string', 11, 3.5]

```

You can check the length of a list using the built-in `len` function.


```python
print(len(MyList))
print(len(MyNewList))
```

    8
    7


You can access characters in a list using square brackets.


```python
MyNewList[0]
```




    'a'




```python
MyNewList[1]
```




    'B'




```python
MyNewList[len(MyNewList)-1]
```




    3.5




```python
MyNewList[len(MyNewList)-3]
```




    'this is a string'




```python
MyNewList[0]
```




    'a'



#### Challenge: Grab element b from the following list `["a", ["b", "c", "d"], 13, 5, "d", "key"]` 

### Getting Sublists with Slices

You can get a slice can get several values from a list, in the form of a new list. A slice is typed between square brackets, like an index, but it has two integers separated by a colon. 


```python
["a", ["b", "c", "d"], 13, 5, "d", "key"][0:3]
```




    ['a', ['b', 'c', 'd'], 13]



You can leave out one or both of the indexes on either side of the colon in the slice. Leaving out the first index is the same as using 0, or the beginning of the list. Leaving out the second index is the same as using the length of the list, which will slice to the end of the list. 


```python
print(["a", ["b", "c", "d"], 13, 5, "d", "key"][:2])
print(["a", ["b", "c", "d"], 13, 5, "d", "key"][2:])

```

    ['a', ['b', 'c', 'd']]
    [13, 5, 'd', 'key']


### Tuples
In case we don't want the list to be modified, we use tupples. To declare tuples we use round brackets `()`. Tuples are rarely used, but they are indeed used.


```python
MyTuple=("a", ["b", "c", "d"], 13, 5, "d", "key")
```


```python
print(MyTuple)
```

    ('a', ['b', 'c', 'd'], 13, 5, 'd', 'key')



```python
MyTuple.append(["a"])
```


    ---------------------------------------------------------------------------

    AttributeError                            Traceback (most recent call last)

    <ipython-input-22-8233c0f1ce33> in <module>()
    ----> 1 MyTuple.append(["a"])
    

    AttributeError: 'tuple' object has no attribute 'append'


We can convert lists to tuples.


```python
FromListToTuple=tuple(MyList)
```


```python
print(type(MyList))
print(type(FromListToTuple))
```

### Sets 
We can store a list with the unique elements of a list. 


```python
MySet=set(["a", "B", "b", "c", "a"])
```


```python
type(MySet)
```

In Python you can declare a set using curly braces `{}`


```python
NewSet={2017, 2013, 2015, 2016, 2013}
print(NewSet)
```

You can also convert tuples into a lists.


```python
MyTuple = ('my', 'name', 'is', 'tuple')
FromTupleToList=list(MyTuple)
print(type(MyTuple))
print(type(FromTupleToList))
```

Indexing, slicing, and the length function that we use when dealing with lists work similarly to strings -- use the `len()` function and square brackets `[ ]`
to access data, with the first element at index 0. See respective `Strings` section.

### References
https://automatetheboringstuff.com/chapter4/

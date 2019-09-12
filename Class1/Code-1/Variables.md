
<center><u><H1>Values and Variables</H1></u></center>

In Python variables can be considered as containers. They contain everything. By assigning different data types to variables, you can store integers, decimals or characters in these variables. You can assign variables using `=` symbol which assigns the value on the right to the name on the left. The variable is created when a value is assigned to it.



```python
FlowerPrice=3.5
```


```python
FlowerType="Tuilpan" 
```

Python has various types of data which can be stored in variables. Three most common types are:

- integer numbers (whole numbers)
- floating point numbers
- strings. 
In Python strings are declared using `"` or `'`. You must be consistent with the use of single or double quotes


```python
FlowerType="Tuilpan'
```


      File "<ipython-input-39-822a5b8cdbce>", line 1
        FlowerType="Tuilpan'
                            ^
    SyntaxError: EOL while scanning string literal



If you mix and match quotes, Python will give you an error. If you read the error, it will tell you that's a syntax error. We'll learn more about those later.

We can check the type of the variable by using the built-in function `type`.



```python
type(FlowerPrice)

```




    float




```python
type(FlowerType)

```


    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    <ipython-input-1-272281e4314a> in <module>()
    ----> 1 type(FlowerType)
    

    NameError: name 'FlowerType' is not defined


Python is letting us know that the type of the variable is a string.

Python is case sensitive. 


```python
type(Flowertype)
```


    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    <ipython-input-27-a264aebd8f59> in <module>()
    ----> 1 type(Flowertype)
    

    NameError: name 'Flowertype' is not defined


Variables need to be assigned before its use.


```python
type(Potatotype)
```


    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    <ipython-input-58-4e323d39edf0> in <module>()
    ----> 1 type(Potatotype)
    

    NameError: name 'Potatotype' is not defined


### Naming variables in Python
- cannot start with a digit
- cannot contain spaces, quotation marks, or other punctuation
- may contain an underscore (typically used to separate words in long variable names)
- Underscores at the start like `__this_is_myvariable` or `_this_another_variable` have a special meaning in Python so don't use them unless you know the meaning.


### In Python you can overwrite a variable.


```python
FlowerPrice=5 
```

If we check the type of this variable, Python will let us know that the type of the variable is an integer.



```python
FlowerType=2.3 
```


```python
type(FlowerType)
```




    str



We can convert an integer to a string.


```python
FlowerPrice=str(FlowerPrice)
```


```python
print(FlowerPrice)
```

    4


Above we used the built-in `print` function to display the variable. Many functions in Python are built-in we are also going to see how to construct our own functions in the upcoming classes.

We can convert a string to an integer. And convert it back to integer (or float).


```python
FlowerPrice=2
FlowerPrice=int(str(FlowerPrice)) 
FlowerPrice=float(str(FlowerPrice))
```

### Operations with Variables

You can do operation between variables


```python
FlowerPrice=2
FlowerPrice=FlowerPrice+3

```


```python
FlowerPrice=2+"3.4"
```


```python
FlowerPrice=2+float("3.4")
```

You can perform operations among variables of the same type or between floats and integers. You cannot perform operations between floats and strings or integers and strings.


```python
FlowerType="Peruvian"+ "Lily"
```


```python
FlowerType="Peruvian"+ 3
```


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    <ipython-input-53-2561c75caf98> in <module>()
    ----> 1 FlowerType="Peruvian"+ 3
    

    TypeError: can only concatenate str (not "int") to str



```python
FlowerType="Peruvian"+ "3"
```


```python
FlowerType="Peruvian"*3
```

Concatenates the string three times.

## Reference:

https://librarycarpentry.org/lc-python-intro/02-variables/index.html

http://swcarpentry.github.io/python-novice-inflammation/01-numpy/index.html

https://automatetheboringstuff.com/chapter1/



<center><u><H1>Strings</H1></u></center>

In Python, strings are declared using `"` or "'" and are concatenated using `+`.


```python
string1 = "Budapest"
string2 = "is a beautiful city"
full_string=string1+" "+ string2
```


```python
print(string1)
print(string2)
print(full_string)
```

    Budapest
    is a beautiful city
    Budapest is a beautiful city


You apply upper, lower or title to convert the string into upper, lower, or title respectively.


```python
print(full_string.lower())
print(full_string.upper())
print(full_string.title())
```

    budapest is a beautiful city
    BUDAPEST IS A BEAUTIFUL CITY
    Budapest Is A Beautiful City


Similar to lists, you can check the length of a string using the built-in `len` function.


```python
len(full_string)
```




    28



Also, similar to lists, we use square brackets `[ ]` to access the characters of a string, with the first element at index 0.


```python
full_string[0]
```




    'B'




```python
full_string[1]
```




    'u'




```python
full_string[28]
```


    ---------------------------------------------------------------------------

    IndexError                                Traceback (most recent call last)

    <ipython-input-10-7a3100442353> in <module>()
    ----> 1 full_string[28]
    

    IndexError: string index out of range



```python
full_string[27]
```




    'y'




```python
full_string[-1]
```




    'y'



A string can be split using `split`.


```python
full_string.split()
```




    ['Budapest', 'is', 'a', 'beautiful', 'city']




```python
full_string.split("a")
```




    ['Bud', 'pest is ', ' be', 'utiful city']




```python
city_list=full_string.split()
```


```python
type(city_list)
```




    list



You can join elements of a list using the `join` method.


```python
" ".join(city_list)
```




    'Budapest is a beautiful city'



#### Challenge: Store the `full_string.split("a")` into a variable. What is the variable type? Convert the list back to a string using the join method.

String work similarly to lists -- use the len() function and square brackets [ ] to access data, with the first element at index 0. See respective Lists section.

#### Challenge: Create a variable named MyVar="This is my first string variable". What is the string that you get if you execute the following command: MyVar.lower().upper().title()


```python

```

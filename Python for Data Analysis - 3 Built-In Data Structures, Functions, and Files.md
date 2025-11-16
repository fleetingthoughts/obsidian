%%tags: #python #datascience #mckinney%%
parent::[Python for Data Analysis 3rd ed. - Wes McKinney](Python%20for%20Data%20Analysis%203rd%20ed.%20-%20Wes%20McKinney.md)

# ***Concepts***
- Tuples are immutable. You cannot change which object is stored in each slot but you can modify them in place
``` 
In [16]: tup[1].append(3)
In [17]: tup
Out[17]: ('foo', [1, 2, 3], True)
```
- Unpacking of tuples can be used to swap variable names without a 3rd "temp" variable. Convention to discard unwanted elements when unpacking the tuple is the underscore
    ```In [39]: a, b, *_ = values```
- List slicing is inclusive of the start index BUT NOT THE stop index
- Dictionary store key-value pairs and are sometimes called hash maps or associative arrays
- Dictionaries are a collection 2-tuples. One set of tuples being the keys and the other being the values
```
tup = (1,2,3,4)
tup2= (1,4,9,16)
dict = dict(((1,2),(4,5)))
```
- List comprehensions used to concisely create elements with certain conditions with the following syntax:
   ```[expr for value in collection if condition]```
- dictionary comprehensions are set up in a similar way
```
dict_comp = {key-expr: value-expr for value in collection if condition}
```
- functions have keyword arguments and positional arguments where the keyword arguments are optional with a default value. In the below example, z is the keyword argument
```
def my_function2(x, y, z=1.5):
    if z > 1:
        return z * (x + y)
    else:
        return z / (x + y)
```
- The scope of the variables is referred to as the namespace. Be aware of name binding when passing arguments. Although the namespace local, they do not reference a local copy of the objects they refer to.
- functions are objects too that can be passed as arguments
- Lambda functions are also called anonymous functions
- In for loops, the python interpreter attempts to create an iterator object out of your iterable object. The generator object is a succinct way to construct an iterator that only executes and iterates when it is called upon. This is a memory efficient way of dealing with very large datasets as the generator serves as a handy way to "zip up" the iterable. 
### Generators 
- Generators can be created with in-line expressions using normal parentheses. These generators are preferable to any other appropriate list comprehension depending on the number of elements. See below for example syntax :
```
In [216]: gen = (x ** 2 for x in range(100))
In [217]: gen
Out[217]: <generator object <genexpr> at 0x17d5feff0>
```
- The itertools module has a collection of generators

### 3.2 Errors and Exception Handling
- Use `try` and `except` blocks to fail gracefully and use `finally` to execute code regardless of success with try or not. The `try` block contains the code that may raise the exception and the `except` block executes excluding specific errors specified (e.g. will execute for any error if nothing specified)
### 3.3 Files and the Operating System
- example code to open a file using `open`with optional file encoding.  `encoding="utf-8"` is best practice
```
In [233]: path = "examples/segismundo.txt"
In [234]: f = open(path, encoding="utf-8")
```
- by default files are opened in `"r"` read only mode
  ```
```
def attempt_float(x):
    try:
        return float(x)
    except (TypeError, ValueError):
        return x
```
- default behaviour for python files is text mode where you intend to work with strings and the string conversion in Unicode is done in the background which is in contrast to binary mode. 
- `Unicode` and other encoding standards like `iso-8859-1` are standards that map characters to numerical values so computers can compute them. Currently `UTF-8` is the most popular encoding method
# ***Functions, Methods, and Attributes***
- the zip() function returns a zip object. The arguments are iterables and returns an iterable zip object where the 
```
In [104]: tuples = zip(range(5), reversed(range(5)))

In [105]: tuples
Out[105]: <zip at 0x17d604d00>

In [106]: mapping = dict(tuples)

In [107]: mapping
Out[107]: {0: 4, 1: 3, 2: 2, 3: 1, 4: 0}
```
- For tuples
	- tup.count
- For lists:
	- list.append(element)
	- list.remove(index)
	- list.extend(list)  this append each entry of a list to the list being extended. list.append would only add the entire list as an element
- For dictionaries
	- dict.pop(value) remove and return the element by key
	- dict.update(iterable) the dictionary analog to list append
	- dict.get (key, default_value)
	- dict.setdefault( key, defaultkey )
- enumerate(collection) = (i, value)  generates enumerable() object that is just a 2-tuple with the entries in the collection and the corresponding index, i.
- zip function
```
In [147]: seq1 = ["foo", "bar", "baz"]
In [148]: seq2 = ["one", "two", "three"]
In [149]: zipped = zip(seq1, seq2)
In [150]: list(zipped)
Out[150]: [('foo', 'one'), ('bar', 'two'), ('baz', 'three')]
```
- yield keyword
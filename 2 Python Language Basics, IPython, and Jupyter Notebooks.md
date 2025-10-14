parent:: [Python for Data Analysis - Wes McKinney](Python%20for%20Data%20Analysis%20-%20Wes%20McKinney.md)

## Keywords and useful functions
- is
- ==
- getattr, hasattr and setattr
- break
	- terminates innermost  for loop that it is a part of
- pass
## Terminology
- module
- scalar types
- method and attributes

## Concepts
- Name binding of variables and how they reference to objects for example with variable assignment
- Duck Typing
- Raw string:
```
In [74]: s = r"this\has\no\special\characters"

In [75]: s
Out[75]: 'this\\has\\no\\special\\characters'
```
- `{0:.2f}` means to format the first argument as a floating-point number with two decimal places.
- `{1:s}` means to format the second argument as a string.
- `{2:d}` means to format the third argument as an exact integer
- f-strings

```
In [81]: amount = 10

In [82]: rate = 88.46

In [83]: currency = "Pesos"

In [84]: result = f"{amount} {currency} is worth US${amount / rate}"
```
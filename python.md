# Python Programming
Python developed in the late 1980s and early 90s by Guido van Rossum

Two main versions in use currently Python2 and Python3. Python2 will reach EOL in 2020.

## Design Philosophy

OO and Structured.
>**Zen of Python**  
>Beautiful is better than ugly.  
>Explicit is better than implicit.  
>Simple is better than complex.  
>Complex is better than complicated.  
>Readability counts.

Highly extensible with libraries. Has a package manager: PiPy.

## Differences Between Python2 and Python3

Print statements differ.  
`Python2`
```Python
    print "";
```
`Python3`
```Pythong
    print();
```

Integer Division in `Python2` yields an integer. In `Python3` it yields a floating point number.

`Python3` strings are unicode by default.

## Data Types
* Int
* Float
* Complex Number
* Boolean
* String

## Operators
* Addition `+`
* Subtraction `-`
* Multiplication `*`
* Division `/`
* Integer Division `//`
* Modulus `%`
* Exponentiation `**`

## Strings
Can be surrounded by `'single quotes'`, `"double quotes"`, or either `'''triple single quotes'''` or `"""triple double quotes"""`. Triple quotes are for multiline strings.

Concatencate with `+`.

They're strings... they are used like strings in all other programming languages. This is some nonsense to include this in course notes.

## Python Features
Handles data type conversion and memory management so you don't have to.

## Advanced Data Types
### Lists
* Mutable
* Add, Remove and Manipulate elements.
* Can store any data type or mixture of data types.
* Defined with `[]`
* Accessed by index, updated by index.

```Python
    my_list = [1, 2, 3, "eggs", 3.14]
```
* Can grab segments with slice.
* Can check for membership.
* Can find idex of item in list.
### Tuples
* Immutable
* Any data type or mix of data types.
* Defined with `()` but not mandatory.
```Python
    my_tuple = (1, 2, 3, "eggs",  3.14)
    #To make a tuple with a single element use a trailing comma.
    my_single_tuple = (99, )
```
### Dictionary
* Works like any implementation of hash map or dictionary.
* Mutable. Because it would be useless if it was immutable.
* Initialized with `{}`.
```Python
    my_dic = {}
    # With Values
    my_dic = {'eggs':'spam'}
```
### Set
* A list but objects must be distinct.
* Initialized with `{}`
```Python
    my_set = {1, 2, 3}
```
## Control Statements

Python has semantic whitespace. This is what separates logical statements and allows these structures to exist without end statements or being defined by curly braces.
### If
Marked with `if` and `:`
```Python
if x == 'This is x':
    print("It sure is")
elif x == 'Why not use else if':
    print("It's a much nicer syntax.")
else:
    print('These notes are tedious')
```

### Comparison Operators
* `<`
* `>`
* `<=`
* `>=`
* `==`
* `!=`
* `is` (used to evaluate object equality)
* `is not`

### For
```Python
    for i in range(5):
        print(i)
```

### Foreach
```Python
    mylist= [1, 2, 3]
    for myitem in mylist:
        print(myitem)
```

### While
```Python
    i = 0
    while i < 10:
        i += 1
        print(i)
```

I'm probably not going to finish with these notes. It's pretty basic.
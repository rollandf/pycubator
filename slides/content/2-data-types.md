# Basic data types
<!-- .slide: data-background="img/monty-python.jpg" -->

---

### Datatypes overview

*   None
*   Booleans (True, False)
*   Integers, Floats
*   Sequences
*   Lists
*   Tuples
*   Strings
*   Dictionaries
*   Classes and class instances
*   Modules and packages

--

### Booleans

*   Booleans: `True, False`
*   The following act like `False`:

*   `None`
*   `0`
*   `[]`(Empty sequences)

*   Everything else acts like `True`

--

### Boolean operations

| Operation | Result
| --------- | ---------------------------------------------
|`x or y`   | if `x` is `False`, then `y`, else `x`
|`x and y`  | if `x` is `False`, then `x`, else `y`
|`not x`    | if `x` is `False`, then `True`, else `False`

`and`, `or` are **short-circuit** operators

--

### Boolean examples

    >>> not True
    False

    >>> True or False
    True

    >>> False and True
    False

    >>> (1 + 1) or True
    2

    >>> True and (2 + 2)
    4

    >>> not 0
    True

Go to socrative quiz!

---

### Integers and floats

*   Numeric operators: `+ - * / // % **`
*   No i++ or ++i, but we do have += and -=
*   Int and Float:

    >>> type(2)
    int

    >>> type(2.5)
    float

    >>> 5/2 #python3
    2.5
    >>> 5/2 #python2
    2
    >>> 5/2.0 #python2
    2.5

---

### Assignments

    >>> a = b = 0
    >>> a, b = 3, 5

Super cool:

    >>> a, b = b, a
    >>> a
    5
    >>> b
    3

---

### Comparisons

    >>> 5 == 5
    True

    >>> 'hello' == 'hello'
    True

    >>> 1 != 2
    True

    >>> 5 > 3
    True

    >>> 'b' > 'a'
    True

---


### If Statements

    if a == 0:
        print 'a is 0'
    elif a == 1:
        print 'a is 1'
    else:
        print 'a is something else'

---

### For Loops

    >>> range(5)
    [0, 1, 2, 3, 4]

    for i in range(5):
        print(i, end=' ')

    0 1 2 3 4

---

### Break and Continue

    for i in range(10):
        if i == 3:
            continue
        elif i == 8:
            break
        print(i, end=' ')

    0 1 2 4 5 6 7

---

### While Loops

    i = 0
    while i <= 3:
        print(i, end=' ')
        i += 1

    0 1 2 3

---

### Ranges

*   range(n) produces [0, 1, ..., n-1]*   range(i, j) produces [i, i+1, ..., j-1]*   range(i, j, k) produces [i, i+k, ..., m]

    >>> range(5, 25, 3)
    [5, 8, 11, 14, 17, 20, 23]

---

### Functions

    >>> def increment(x):
            return x + 1
    >>> increment(3)
    4

*   Colon (:) indicates start of a block
*   Following lines are indented
*   Function declaration doesn’t specify return type
*   all functions return a value (None if not specified)
*   Parameter datatypes are not specified either
# python

## Exception handling
There are two types of erros that typically occur while writing programs. The first one is known as syntax error,simply means that the programmer has made mistake in the structure of the statement or expression.
For example, it is incorrect to write a for statement and forget the colon.
```python
>>> for i in range(10)
SyntaxError: invalid syntax (<pyshell#61>, line 1)
```

The other type of the error, known as a logic error, denotes a situation where the program executes but gives the wrong result. Some logical errors lead to the bad situatioon such as trying to divide by zero or trying to access the item where the index of the item is outside the bounds of the list. In this case logical error leads to the runtime error that causes the program to terminate. These types of runtime errors are called exceptions

``` python
import math
number=int(input())
try:
    print(math.sqrt(number))
except:
    print('bad value for a square root')
    print("Absolute value instead")
    print(math.sqrt(abs(number)))
```

```python
import math
number=int(input())
if number<0:
    raise RuntimeError("you can't use negative number")
else:
    print(math.sqrt(number))
```

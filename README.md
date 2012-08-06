interceptor
===========

functools missing method

```
    >>> def add(x, y):
    ...   return x + y
    ...
    >>> intercepted = Interceptor(add, 1, 2)
    >>> intercepted['x']
    1
    >>> intercepted['y']
    2
    >>> intercepted['y'] = 3
    >>> intercepted()
    4
```
2. Variables
------------

Variables are names that can be used to refer to and remember the result of an
expression. The name of a variable can contain letters, numbers and
underscores, and should not start with a number. Variable names are case
sensitive, so ``rate``, ``RATE`` and ``Rate`` are 3 different variables.

The print statement takes an expression and writes out the result of that
expression to the screen.

>>> rate = 100
>>> Rate = 200
>>> print rate
100
>>> print Rate
200
>>> print RATE
Traceback (most recent call last):
 ...
NameError: name 'RATE' is not defined


The ``=`` operator is used to assign the result of the expression to the right
of it to the name (or names) to the left of it. The expression to the right can
be a literal value, like the 100 and 200 above, but it can also be a more
complex expression:

#TODO

Since the expression to the right is evaluated before assigning it to the
variable name(s) on the left, you can use it to change the value of one of more
variables as well:

>>> rate = 14
>>> rate = rate * 2
>>> print rate
28

And even to swap the values of two or more variables around:

>>> rate1, rate2 = 100, 200
>>> print rate1, rate2
100 200

>>> rate1, rate2 = rate2, rate1
>>> print rate1, rate2
200 100

>>> rate1, rate2 = rate1 / rate2, rate1 + 8
>>> print rate1, rate2
2 208

.. Note::
    In that last example that the values assigned to the variables rate1 and
    rate2 do not change until all the expressions on the right of the ``=`` are
    evaluated.


Footnotes
~~~~~~~~~

.. [#] https://en.wikipedia.org/wiki/Floating_point

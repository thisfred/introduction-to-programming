1. Expressions
--------------

The Python interpreter can be used as a calculator, by directly typing in
arithmetic expressions.

Addition:

>>> 1 + 3
4

Subtraction:

>>> 1 - 12
-11

Multiplication:

>>> 2 * 8
16

Division:

>>> 15 / 3
5

Exponents:

>>> 2 ** 5
32

>>> 5 ** 2
25

Order of Operations:

The order of operations is as commonly defined. [#]_

>>> 2 * 2 + 15 / 3
9

The order in which the operations are applied can always be explicitly given by
using parentheses:

>>> ((2 + 15) / (3 - 8)) * (6 / 2)
-12

Precision:

>>> 12 * 0.33
3.96

Note the decimal point: Numbers without a decimal point are called integers,
and numbers that have a decimal point are called floating points [#]_ or floats
for short.

Unlike in some other languages, Python allows you to use floats and integers in
the same expression. The result of the expression will always be converted to a
float if any of the constituents was a float. 

.. note::

   The result of the division of two integers will always be rounded down to
   the nearest integer, so if you need more precision, you have to make at
   least one of the arguments into a float.  You can do this by tacking on the
   decimal point, (or .0 to make the code more readable) or by using the
   :func:`float` function. (We'll get to functions in a little bit):

>>> 14 / 5
2
>>> 14 / 5.
2.8
>>> float(14) / 5
2.8
>>> 14.0 / 5.0
2.8


Footnotes
~~~~~~~~~

.. [#] https://en.wikipedia.org/wiki/Order_of_operations

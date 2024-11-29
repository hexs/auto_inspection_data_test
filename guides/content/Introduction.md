[back to Home Page](/README.md)
# Introduction

``` python
# this is the first comment
spam = 1  # and this is the second comment
# ... and now a third!
text = "# This is not a comment because it's inside quotes."
```

## 1. Numbers¶
The operators +, -, * and / can be used to perform arithmetic
``` python
2 + 2
50 - 5*6
(50 - 5*6) / 4
8 / 5  # division always returns a floating-point number
```

The integer numbers (e.g. 2, 4, 20) have type int,
the ones with a fractional part (e.g. 5.0, 1.6) have type float.
Division (/) always returns a float.
To do floor division and get an integer result you can use the // operator;
to calculate the remainder you can use %
``` python
17 / 3  # classic division returns a float
17 // 3  # floor division discards the fractional part
17 % 3  # the % operator returns the remainder of the division
5 * 3 + 2  # floored quotient * divisor + remainder
```

use the ** operator to calculate powers
``` python
5 ** 2  # 5 squared
2 ** 7  # 2 to the power of 7
```

The equal sign (=) is used to assign a value to a variable. Afterwards, no result is displayed before the next interactive prompt:
``` python
width = 20
height = 5 * 9
width * height
```

If a variable is not “defined” (assigned a value), trying to use it will give you an error:
``` python
n # try to access an undefined variable
```

``` python
tax = 12.5 / 100
price = 100.50
price * tax
```

``` python
price + _
```

``` python
round(_, 2)
```

## 2. Text

``` python
'spam eggs'  # single quotes
"Paris rabbit got your back :)! Yay!"  # double quotes
'1975'  # digits and numerals enclosed in quotes are also strings
```

``` python
'doesn\'t'  # use \' to escape the single quote...
"doesn't"  # ...or use double quotes instead
'"Yes," they said.'
"\"Yes,\" they said."
'"Isn\'t," they said.'
```

The print() function
``` python
s = 'First line.\nSecond line.'  # \n means newline
s  # without print(), special characters are included in the string
print(s)  # with print(), special characters are interpreted, so \n produces new line
```
print path

``` python
print('C:\some\name')  # here \n means newline!
print(r'C:\some\name')  # note the r before the quote
```

## 3. Lists¶

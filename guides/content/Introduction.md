[back to Home Page](/README.md)
# Introduction

``` python
# this is the first comment
spam = 1  # and this is the second comment
# ... and now a third!
text = "# This is not a comment because it's inside quotes."
```
---
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

---
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

multiple lines. One way is using triple-quotes: """...""" or '''...'''
``` python
print("""\
Usage: thingy [OPTIONS]
     -h                        Display this usage message
     -H hostname               Hostname to connect to
""")
```

Strings can be concatenated (glued together) with the `+` operator, and repeated with `*`:
``` python
'py' + 'thon'
3 * 'py' + 'thon'
'py' + 'thon' * 3
```

Strings can be indexed
``` python
word = 'Python'
word[0]  # character in position 0
word[5]  # character in position 5
```

``` python
word[0:2]  # characters from position 0 (included) to 2 (excluded)
word[2:5]  # characters from position 2 (included) to 5 (excluded)
```

``` python
word[:2]   # character from the beginning to position 2 (excluded)
word[4:]   # characters from position 4 (included) to the end
word[-2:]  # characters from the second-last (included) to the end
```

``` python
word[:2] + word[2:]
word[:4] + word[4:]
```

```
 +---+---+---+---+---+---+
 | P | y | t | h | o | n |
 +---+---+---+---+---+---+
   0   1   2   3   4   5
  -6  -5  -4  -3  -2  -1
```

Attempting to use an index that is too large will result in an error
``` python
word[42]  # the word only has 6 characters
```

``` python
word[4:42]
word[42:]
```

The built-in function len() returns the length of a string
``` python
s = 'supercalifragilisticexpialidocious'
len(s)
```

---
## 3. Lists

``` python
squares = [1, 4, 9, 16, 25]
squares
# [1, 4, 9, 16, 25]
```

``` python
squares[0]  # indexing returns the item
# 1
squares[-1]
# 25
squares[-3:]  # slicing returns a new list
# [9, 16, 25]
```

Lists also support operations like concatenation
``` python
squares + [36, 49, 64, 81, 100]
# [1, 4, 9, 16, 25, 36, 49, 64, 81, 100]
```

The `print()` function
``` python
cubes = [1, 8, 27, 65, 125]  # something's wrong here
4 ** 3  # the cube of 4 is 64, not 65!
# 64
cubes[3] = 64  # replace the wrong value
cubes
# [1, 8, 27, 64, 125]
```

``` python
cubes.append(216)  # add the cube of 6
cubes.append(7 ** 3)  # and the cube of 7
cubes
# [1, 8, 27, 64, 125, 216, 343]
```

``` python
rgb = ["Red", "Green", "Blue"]
rgba = rgb
id(rgb) == id(rgba)  # they reference the same object
# True
rgba.append("Alph")
rgb
# ["Red", "Green", "Blue", "Alph"]
```

``` python
correct_rgba = rgba[:]
correct_rgba[-1] = "Alpha"
correct_rgba
# ["Red", "Green", "Blue", "Alpha"]
rgba
# ["Red", "Green", "Blue", "Alph"]
```

``` python
letters = ['a', 'b', 'c', 'd', 'e', 'f', 'g']
letters
# ['a', 'b', 'c', 'd', 'e', 'f', 'g']
# replace some values
letters[2:5] = ['C', 'D', 'E']
letters
# ['a', 'b', 'C', 'D', 'E', 'f', 'g']
# now remove them
letters[2:5] = []
letters
# ['a', 'b', 'f', 'g']
# clear the list by replacing all the elements with an empty list
letters[:] = []
letters
# []
```

`len()` function
``` python
letters = ['a', 'b', 'c', 'd']
len(letters)
# 4
```

``` python
a = ['a', 'b', 'c']
n = [1, 2, 3]
x = [a, n]
x
# [['a', 'b', 'c'], [1, 2, 3]]
x[0]
# ['a', 'b', 'c']
x[0][1]
# 'b'
```

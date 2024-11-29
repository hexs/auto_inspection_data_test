[back to Home Page](/README.md)
# Control Flow Tools
---

## 1. `while`

``` python
a = 0
while a < 10:
    print(a)
    a = a + 1
```
---

## 2. `if`

``` python
x = int(input("Please enter an integer: "))
# Please enter an integer: 42
if x < 0:
    x = 0
    print('Negative changed to zero')
elif x == 0:
    print('Zero')
elif x == 1:
    print('Single')
else:
    print('More')
# More
```
---

## 3. `for`

``` python
words = ['cat', 'window', 'defenestrate']
for w in words:
    print(w, len(w))
# cat 3
# window 6
# defenestrate 12
```
---

## 4.  The  `range()` Function

Lists also support operations like concatenation
``` python
for i in range(5):
    print(i)
# 0
# 1
# 2
# 3
# 4
```
``` python
list(range(5, 10))
# [5, 6, 7, 8, 9]
list(range(0, 10, 3))
# [0, 3, 6, 9]
list(range(-10, -100, -30))
# [-10, -40, -70]
```

``` python
a = ['Mary', 'had', 'a', 'little', 'lamb']
for i in range(len(a)):
    print(i, a[i])
# 0 Mary
# 1 had
# 2 a
# 3 little
# 4 lamb
```
---

## 5.`break`  and  `continue`

``` python
for n in range(2, 10):
    for x in range(2, n):
        if n % x == 0:
            print(f"{n} equals {x} * {n//x}")
            break
# 4 equals 2 * 2
# 6 equals 2 * 3
# 8 equals 2 * 4
# 9 equals 3 * 3
```

``` python
for num in range(2, 10):
    if num % 2 == 0:
        print(f"Found an even number {num}")
        continue
    print(f"Found an odd number {num}")
# Found an even number 2
# Found an odd number 3
# Found an even number 4
# Found an odd number 5
# Found an even number 6
# Found an odd number 7
# Found an even number 8
# Found an odd number 9
```
---

## 6. `else`  Clauses on Loops

``` python
for n in range(2, 10):
     for x in range(2, n):
         if n % x == 0:
             print(n, 'equals', x, '*', n//x)
             break
     else:
         # loop fell through without finding a factor
         print(n, 'is a prime number')

# 2 is a prime number
# 3 is a prime number
# 4 equals 2 * 2
# 5 is a prime number
# 6 equals 2 * 3
# 7 is a prime number
# 8 equals 2 * 4
# 9 equals 3 * 3
```


## 1. `while`

``` python
a = 0
while a < 10:
    print(a)
    a = a + 1
```

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

## 3. `for`

Lists also support operations like concatenation
``` python
words = ['cat', 'window', 'defenestrate']
for w in words:
    print(w, len(w))
# cat 3
# window 6
# defenestrate 12
```

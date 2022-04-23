# python-study-notes

## get substring
```
letters = "abcdef"
r = letters[0]
print(r)

>> "a"
```

```
letters = "abcdef"
r = letters[:-1]
print(r)

>> "abcde"
```

```
letters = "abcdef"
r = letters[1:]
print(r)

>> "bcdef"
```

```
letters = "abcdef"
r = letters[1:-1]
print(r)

>> "bcde"
```
-----
## remove item
```
items = [1,2,3,4,5]
del items[0:2]
print(items)

>> [3, 4, 5]
```

```
items = [1,2,3,4,5]
items.pop(2)
print(items)

>> [1, 2, 4, 5]
```
-----
## add item
```
items = [1,2,3,4,5]
items.append(6)
print(items)

>> [1, 2, 3, 4, 5, 6]
```

```
items = [1,2,3,4,5]
items.insert(2, 'r')
print(items)

>> [1, 2, 'r', 3, 4, 5]
```
-----
## filter list
```
items = [1,2,3,4,5,6,7,8]
r = [i for i in items if i % 2 == 0]
print(r)

>> [2, 4, 6, 8]
```

```
items = [1,2,3,4,5,6,7,8]
r = list(filter(lambda i: i % 2 == 0, items))
print(r)

>> [2, 4, 6, 8]
```
-----
## map list
```
items = [1,2,3,4,5]
r = [i * 2 for i in items]
print(r)

>> [2, 4, 6, 8, 10]
```

```
items = [1,2,3,4,5]
r = list(map(lambda i: i * 2, items))
print(r)

>> [2, 4, 6, 8, 10]
```
-----
## split by delimiter
```
letters = 'a b c d e f'
r letters.split(' ')
print(r)

>> ['a', 'b', 'c', 'd', 'e', 'f']
```
-----
## join with delimiter
```
items = ['a','b','c','d','e']
r = " ".join(items)
print(r)

>> "a b c d e"
```
-----
## reverse list
```
items = [1,2,3,4,5]
r = items[::-1]
print(r)

>> [5, 4, 3, 2, 1]
```

```
items = [1,2,3,4,5]
items.reverse()
print(items)

>> [5, 4, 3, 2, 1]
```
-----
## sort list
```
items = [2,4,6,1,2,3]
r = sorted(items)
print(r)

>> [1, 2, 2, 3, 4, 6]
```

```
items = [2,4,6,1,2,3]
r = sorted(items, reverse=True)
print(r)

>> [6, 4, 3, 2, 2, 1]
```
-----
## get max
```
items = [1,2,3,6,5,4]
r = max(items)
print(r)

>> 6
```
-----
## get min
```
items = [6,5,4,1,2,3]
r = min(items)
print(r)

>> 1
```

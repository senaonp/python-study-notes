# python-study-notes
reference to do basic operations on iterable objects

| [get substring](#get-substring) | [add item](#add-item) | [remove item](#remove-item) | [filter list](#filter-list)  | [map list](#map-list) |
| :-: | :-: | :-: | :-: | :-: |
| [split by delimiter](#split-by-delimiter) | [join with delimiter](#join-with-delimiter) | [reverse list](#reverse-list) | [sort list](#sort-list) | [get max](#get-max) |
| [get min](#get-min) | [is item in list](#is-item-in-list) | [is instance of type](#is-instance-of-type) | [get index of item in list](#get-index-of-item-in-list) | [get indices of item in list](#get-indices-of-item-in-list) | 
| [iterate by index](#iterate-by-index) | [get column in 2d matrix](#get-column-in-2d-matrix) | [uppercase string](#uppercase-string) | [lowercase string](#lowercase-string) | [get unique list items](#get-unique-list-items) |

-----

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
r = letters.split(' ')
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
-----
## is item in list
```
items = ['a','b','c','d','e']
print(True) if ('d' in items) else print(False)

>> True
```
-----
## is instance of type
```
isinstance([1,2,3], list)

>> True
```

```
isinstance({'a': 1, 'b': 2}, dict)

>> True
```
-----
## get index of item in list
```
items = ['a','b','c','d','e']
r = items.index('c')
print(r)

>> 2
```
-----
## get indices of item in list
```
items = [1,2,3,2,4,6,3,6,9]
r = [i for i in range(len(items)) if items[i] == 3]
print(r)

>> [2, 6]
```
-----
## iterate by index
```
items = ['a','b','c','d','e']
for i in range(len(items)):
  print(i, end=' ')

>> 0 1 2 3 4
```
-----
## get column in 2d matrix
```
items = [
  [1,2],
  [3,4],
  [5,6],
  ]
r = [i[0] for i in items]
print(r)

>> [1, 3, 5]
```
-----
## uppercase string
```
letters = "abcde"
r = letters.upper()
print(r)

>> 'ABCDE'
```
-----
## lowercase string
```
letters = "ABCDE"
r = letters.lower()
print(r)

>> 'abcde'
```
-----
## get unique list items
```
items = [1,2,2,3,3,3]
r = []
for i in items: i not in r and r.append(i)
print(r)

>> [1, 2, 3]
```

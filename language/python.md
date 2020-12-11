# Python Notes
Quick notes to refer, tested with Python 3.6.9
## Built-in
`/` division in Python3 will force float on the quotient (result) even if if both dividend and divisor are integer. This behavior is different from Python2 in which `/` is automatically integer division between 2 ints
```python
quotient = dividend //divisor
```

`range()` in Python3 is `xrange()` in Python2
```python
for i in range(5):
    # Do something with i
```

`ord()` is a function to get the ascii number or char
```python
# val will be 98
val = ord('a')
```

`set()` is how to initialise a set
Python's sets are backed by the dict data type; O(1) performance.
Any hashable object can be stored in set.
```python
mySet = set()
mySet.add(item)
mySet.remove(item)
```
`tuple` is an immutable sequence

`bin()` is to get binary representation of number

## General usage
Initialising Array With Certain Value
```python
arr = val * length
```

Crazy Set to find intersection, symetric difference, union, difference
```python
myPartySet = {"pikachu", "sandshrew", "dugtrio"}
theirPartySet = {"pikachu", "dugtrio", 'meowth'}
print(myPartySet & theirPartySet) # {'pikachu', 'dugtrio'}
print(myPartySet ^ theirPartySet) # {'sandshrew','meowth'}
print(myPartySet | theirPartySet) # {'meowth', 'sandshrew', 'pikachu', 'dugtrio'}
print(myPartySet - theirPartySet) # {'sandshrew'}
```

Stack
 + Can be implemented with Python List
 + Use `stack[-1:]`, get the last element in the list

Regex
 + Match pattern and assign to variable
```
import re

p = re.compile("([A-z]{5})-([0-9]*)")
sample = "Janet-1024"
group = p.match(sample)

print(group[0]) # Janet-1024
print(group[1]) # Janet
print(group[2]) # 1024
```

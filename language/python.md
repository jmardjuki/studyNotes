# Python Notes
Quick notes to refer
## Built-in
`range()` in Python3 is `xrange()` in Python2
<br>Usage example
```python
for i in range(5):
    # Do something with i
```

`ord()` is a function to get the ascii number or char
<br>Usage example
```python
# val will be 98
val = ord('a')
```

`set()` is how to initialise a set
<br> Usage exampl
Python's sets are backed by the dict data type; O(1) performance.
Any hashable object can be stored in set.

`bin()` is to get binary representation of number

## General usage
Stack
 + Can be implemented with Python List
 + Use `stack[-1:]`, get the last element in the list

Regex
 + Match pattern and assign to variable
<br>Usage example
```
import re

p = re.compile("([A-z]{5})-([0-9]*)")
sample = "Janet-1024"
group = p.match(sample)

print(group[0]) # Janet-1024
print(group[1]) # Janet
print(group[2]) # 1024
```

# TOPICS (PYTHON SPECIFIC)
1. MUST REMEMBER
2. Math Functions
3. String Functions
4. Others

## 1 MUST REMEMBER
- #No. of alphabets: 26
- #No. of cards in a standard deck: 52
- #No. of suites in a standard deck: 12
- 0 is `False` if used as a boolean
- Any Number != 0 is `True` if used as a boolean
- To find out what is the index of the alphabet in a len(arr) == 26, you can 
  - `ord(char) - ord('a')` for small case OR 
  - `ord(char) - ord('A')` upper case
- To convert from `small` letter to `capital` letter, you can
```python3
if (ord(char) >= ord('a')) and (ord(char) <= ord('z')):
  char = chr(ord(char) - (ord('a') - ord('A')))
```
- To convert from `capital` letter to `small` letter, you can
```python3
if (ord(char) >= ord('A')) and (ord(char) <= ord('Z')):
  char = chr(ord(char) + (ord('a') - ord('A')))
```
- 421 = `1*10^0 + 2*10^1 + 4*10^2`
- Use `%` to iterate through a circular array
``` python3
arr = [5,4,3,2,1]
index = 4
while True:
  index += 1
  print(arr[index%len(arr)])

# print
# 5, 4, 3, 2, 1, 5, 4, 3, 2, 1, 5, 4, ....
```

## 2 Math Functions

```python3
# max - get maximum number in a list
max(1) # ERROR
max(1,2,3,4,5) # 5
max([1,2,3,4,5]) # 5 - can input an array

# min - get minimum number in a list
max(1,2,3,4,5) # 1

# abs - get the absolute number (turn -ve into +ve)
abs(-123) # 123
abs(123) # 123

# pow - used for calculating power
pow(x,y,z) # x^y % z - z is OPTIONAL
pow(10,-1) # 0.1, 10^-1 = 1 / 10

# sum - sum up everything
sum([1,2,3]) # 6
```

## 2 String Functions

```python3
# chr - convert Unicode / ASCII Number into character
chr(97) # a

# ord - reverse of chr (To convert character into Unicode)
ord('a') # 97

# sorted - sort string
sorted('cbd') # ['b', 'c', 'd']
sorted([1,2,4,3]) # [1,2,3,4]

# reverse a string or array
str = 'rooroo'
str[::-1] # ooroor
arr = [5,4,3,2,1]
arr[::-1] # [1,2,3,4,5]
```

## 3 Others

```python3
# len - length
len([5,2,4]) # 3
len("abcd") # 4 - String is treated as an array

# bool - convert variable into boolean
bool([]) # False
bool([0]) # True
bool(5) # True

# or / and in if statement
if True or False:
  # Always True
if True and False:
  # Always False

# list and set *** REMOVE DUPLICATES
list(set([1,2,2,2,3])) # [1,2,3]
list(set('banana')) # ['a','n','b']

# for loop
for i in range(len(a)):
  # access a with a[i]
for i in range(10):
  # access a from 0 to 9

# for loop in reverse
a = ['r','o','o','r','o','o']
for i in range(len(a), 0, -1):
  # access a with a[i-1]
  
# dict - create a dictionary
a = dict({ 'x': 1, 'y': 3 })
a['b'] = 5 # {'x': 1, 'y': 3, 'b': 5}

# last element
[1,2,3][-1] # 3

# validate `not`
a = None
if a is not None:
  # will never execute
```

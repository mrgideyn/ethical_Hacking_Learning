# Section 21 : python bases

## datatype
- native : int, float, bool, str, list, tuple, set, dict, complex
- classes = custom types
- spezialized data types (module.*)
- None (=NULL)


# operators
`a ** b` = a^b
`a // b` = a/b round to lower integer
`a % b` = modulo (reste division euclienne -> a//b)

# math functions
https://docs.python.org/3
round(), abs(), https://docs.python.org/3/library/math.html#module-math
bin()

# variables

# expressions VS statement
- expression : "50/5", piece of code that produce value/results
- statement : line of code doing an action (var assign, etc.)

# Augmented assignment operator (+=, -=, etc)

# type conversion
str(), int()

# formatted string
```
vara='ddd'
varb='fff'
print(f'{vara} {varb}')
```

# string index
```
vara='ttrtaratat'
print(vara[2])
print(vara[2:5])
print(vara[start:stop:stepover])
print(vara[::-1]) #reverse string
```
**WARNING : string index starts at 1, not 0**

# Immutability
string in python are immutable (possible to reassign, but not modify)

## [builtin functions](https://docs.python.org/3/library/functions.html)
```
vara='azerty'
varb=vara.len()
```

possible to embed function in print fcuntion with f option :
```
print(f'{vara} {len(varb)}')
```

## data structures
### list
- ordered with index
- data structure = container around data with metho to access it
- = array in other languages
- **index starts at 0**
- list are mutable ( != vars)
- [methods](https://www.w3schools.com/python/python_ref_list.asp)
sort(li1) = sort li1
sorted(li1) = create a sorted copy of li1 (= new list)
range(101) # creates a list from 0 to 101

```
li = [1,2,3,4,5,6]
li2 = ['a','b','c']
li3 = [1,2,'a',True,8,9,6,5]
print(len(li))
print(li2[2])
print(li3[0:8:2])
li3[2] = 'patate'
print(li3[0:8:2]) #list slicing creates a new list, no modif on original list
li4 = li3
li5 = li3[:]
print(li4)
print(li5)
print('9' in li3)
sentence=' '
new_sent = sentence.joint(['word1','word2','word3'])
new_sent_bis = ' '.joint(['word1','word2','word3'])
```
list unpacking :
```
a,b,c = 1,2,3
print(a)
print(c)
a,b,c,*other,d = [1,2,3,4,5,6,7,8,9]
print(other)
print(d)
```


### matrix
```
matrix = [
    [1,2,3],
    [4,5,6],
    [7,8,9],
    [10,11,12],
]
print(matrix[1][2])
```
### Dictonary
- not ordered but k-v
- dic key must be immutable and unique
- dic are mutable
```

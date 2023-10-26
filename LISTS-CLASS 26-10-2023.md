Lists:

##> A list is a heterogenous sequential mutable data type. 
##> A list are used to store multiple items in a single variable and it allows duplicate values. 
##> lists are defined with []


```python
thislist=['apple', 'banana', 'cherry']
print(thislist)
```

    ['apple', 'banana', 'cherry']
    

Positive slicing:

syntax:
string [start :end :step]

start : it starts with 0.
end : n+1(length of datatype)
step(default): +1


```python
thislist=['apple', 'banana', 'cherry']
print(thislist, type(thislist), len(thislist))
```

    ['apple', 'banana', 'cherry'] <class 'list'> 3
    

negative slicing:

start: -1
end: -(n+1)
step: -1

Empty list:
    an empty list can be achieved in two ways i.e. either by using square brackets[] or using the list() constructor.
    lists are mutable.
    the list where we dont have any elements.

    


```python
z=[]
print(z, type(z), len(z))
```

    [] <class 'list'> 0
    

n list:
    


```python
l=list()
print(l, type(l), len(l), hex(id(l)), sep='\n')
```

    []
    <class 'list'>
    0
    0x231dfa1c840
    


```python
l=['string']
print(l, type(l), len(l), hex(id(l)), sep='\n')
```

    ['string']
    <class 'list'>
    1
    0x231dfa6f7c0
    


```python
l=list('string')
print(l, type(l), len(l), hex(id(l)), sep='\n')
```

    ['s', 't', 'r', 'i', 'n', 'g']
    <class 'list'>
    6
    0x231dfa535c0
    


```python
l=list({100,1,45,9999})
print(l)
```

    [1, 100, 45, 9999]
    


```python
Nested list:
    A list within another list is referred to as a nested list in Python

```


```python
num = [1, 2, [3, 4, [5, 6]], 7, 8]

print(num[2])
```

    [3, 4, [5, 6]]
    

Range():
The range() function returns a sequence of numbers, starting from 0 by default, and increments by 1 (by default), and stops before a specified number.


```python
r=range(1,11)
print(r, type(r), len(r), hex(id(r)), sep='\n')
```

    range(1, 11)
    <class 'range'>
    10
    0x231deecf750
    

Methods:

Methods are functions that are associated with an object or a class in Python programming. They are used to perform specific tasks or operations on the data stored within objects or classes.





```python
dir(l)
```




    ['__add__',
     '__class__',
     '__class_getitem__',
     '__contains__',
     '__delattr__',
     '__delitem__',
     '__dir__',
     '__doc__',
     '__eq__',
     '__format__',
     '__ge__',
     '__getattribute__',
     '__getitem__',
     '__getstate__',
     '__gt__',
     '__hash__',
     '__iadd__',
     '__imul__',
     '__init__',
     '__init_subclass__',
     '__iter__',
     '__le__',
     '__len__',
     '__lt__',
     '__mul__',
     '__ne__',
     '__new__',
     '__reduce__',
     '__reduce_ex__',
     '__repr__',
     '__reversed__',
     '__rmul__',
     '__setattr__',
     '__setitem__',
     '__sizeof__',
     '__str__',
     '__subclasshook__',
     'append',
     'clear',
     'copy',
     'count',
     'extend',
     'index',
     'insert',
     'pop',
     'remove',
     'reverse',
     'sort']



Append:
The append() method appends an element to the end of the list.

Syntax:
list.append(elmnt)


```python
a = ["apple", "banana", "cherry"]
b = ["Ford", "BMW", "Volvo"]
a.append(b)
print(a)
```

    ['apple', 'banana', 'cherry', ['Ford', 'BMW', 'Volvo']]
    


```python
Extend():
    The extend() method adds the specified list elements (or any iterable) to the end of the current list.

Syntax:
    list.extend(iterable)
```


```python
fruits = ['apple', 'banana', 'cherry']

points = (1, 4, 5, 9)

fruits.extend(points)
print(fruits)
```

    ['apple', 'banana', 'cherry', 1, 4, 5, 9]
    

Insert():

The insert() method inserts the specified value at the specified position.

Syntax:
list.insert(pos, elmnt)


```python
Remove():
    
    The remove() method removes the first occurrence of the element with the specified value.
    Syntax:
        list.remove(elmnt)
```


```python
fruits = ['apple', 'banana', 'cherry']

fruits.remove("banana")
print(fruits)
```

    ['apple', 'cherry']
    

pop():
    The pop() method removes the element at the specified position.

syntax:
    list.pop(pos)


```python
fruits = ['apple', 'banana', 'cherry']

fruits.pop(1)
print(fruits)
```

    ['apple', 'cherry']
    

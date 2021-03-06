Data types
====

strings:
---
- string methods: find, replace(actually creates another string object), split

- string types:

```python
#ascii:
s1='regular string'

#unicode:
s1 = u`to unicode string`

#raw format
s1 = r`to raw string`
```

- string operations: 

```python
#concatination:
s1 + s2

#repeat
buffer = "A" * 20

#slicing
string[start:end:steps]
```


 
- string convertion: 

```python
#convert to unicode string
s1 = unicode(str2)

#convert to regular string(ascii charecters)
str_unicoded = str(str2)
s1=str(42)
```
- strings are immutable objects: 

```python
name='someone'
#it is possible to print a charecter at spacific index:
print name[0]
#however - it is impossible to change it :
name[0] = 'x' #errr

```

numbers:
------
 
```python
#x to the power y
x**y
```



lists:
-------
- lists are heterogeneous collection of objects, they can be nested

```python
list1 = [ 1, 2 , [ 3, 4, 'nested list' ] , "a" ]

len( list1[0] ) #err
#Function: len() 
len( list1[2] )  #1 nested object
#Methods: reverse(), pop( the rightest item), extend([]) ..
list1.reverse()


list1.insert(0, 'put me first')
#Operators: del , + (to concatinate 2 lists)
del list1[0] 

```

Tuples:
-----
- basicly are immutable lists
- allow sequence unpacking:
- syntax:  using () instead of [] 

```python
list1=[1,2,'a']

#convert from list:
tuple1 = tuple( list1 )

#unpacking a tuple:
var1 , var2 = ('my secret', 42 )
```

sets:
----
- sets are unorderd lists
- convertion allowed: list(set1) , set(list1)
- allowed operations: 
- 
```python
a|b #union
a&b #intersection
a-b #difference
```

dictionaries:
------
- set of unordered key-value pairs
- methods: keys(), values(), items(), get('some key')

```python
dict1={} # empty dictionary 
dict1['contry']=972 #item gets appended to the dictionary
#OR
dict1(  country=972 , ... ) #note: no parenthesis
dict1={'country':972}
##
dict1.has_key('country') #true
#OR
'country' in dict1 #true
#fetch valude:
dict1.get('country') #972

#remove an item:
del dict1['country'] #1 item
#OR 
dict1.clear() #ALL items
```

getting help
----
- dir(some_object) #output is a list of object's attributes such as:  available methods.
- help( some_object.method1 ) #output: help for method1 (...)

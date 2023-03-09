# Python Objects and Data Structure Basics

## Python Data Types
| Name                | Type   | Description                                   |
| ------------------- |--------| ----------------------------------------------|
| Integers            | int    | Whole Numbers                                 |
| Floating Point      | float  | Numbers With Decimal                          |
| Strings             | str    | Ordered Sequence of Characters                |
| Lists               | list   | Ordered Sequence of Objects                   |
| Dictionaries        | dict   | Unordered Key:Value Pairs                     |
| Tuples              | tup    | Ordered Immutable Sequence of Objects         |
| Sets                | set    | Unordered Collection of Unique Objects        |
| Booleans            | bool   | Logical Value indicating False or True        |

## Mathematical Operations
| Name | Description    |
| ---  |----------------|
| -    | Minus          |
| +    | Plus           |
| *    | Multiplication |
| /    | Division       |
| %    | Mod            |
| **   | Power          |

## Variable Assignments
- To define a variable 
```python
 variablename = 2 
 ```
- Names can't start with a number.
- There can't be spaces in a variable name use _ instead.
- It can't have any of :'",<>/?|\()!@#$%^&*~-+ .
- Since Python uses Dynamic Typing, variables can be assigned with different data types.
- type(variablename) can be used to get the type of the variable.
- Avoid using builtin Python names (error will occur).


### Strings
- Wrapped in either ' ' or " ".
- It's an ordered sequence of characters.
- The index position starts from 0.
- The index can be done using negative indexing -1 is the last character -2 is the before the last...
- For indexing variablename[index].
- For slicing variablename[StartIndex:EndIndex:Steps].
- mystring[::-1] reverses a string.

```python
 indexSlicing = "Anas Kayra"
 print(indexSlicing[0]) # A
 print(indexSlicing[1]) #n
 print(
 print(indexSlicing[0:4]) #Anas
 print(indexSlicing[:4]) #Anas
 print(indexSlicing[0:4:2]) #As
 ```
 
#### Escape Sequences
| Name | Description       |
| ---  |-------------------|
| \n   | New Line          |
| \t   | Tab               |
| \b    | Backspace        |
| \\    | \                |
| \'    | '                |


#### Some built-in functions for strings

| Name           | Description                                                                                                    |
| -------------  |----------------------------------------------------------------------------------------------------------------|
| capitalize()   | First Letter Capital Others Small                                                                              | 
| lower()        | All Letters Small                                                                                              |
| title()        | First Letter of Each Word Capital                                                                              |
| upper()        | All Letters Capital                                                                                            |
| count()        | Amount of Times a String of Characters Appeared in the String (Can also add start and end index)               |
| find()         | Index of Characters in a String                                                                                |
| replace()      | Replaces Character/String in the String with another                                                           |
| swapcase()     | Swaps Capital to Small and Small to Capital                                                                    |
| split()        | Splits a String into a List by default based on white spaces but can be on different character                 |


#### Strings Properties
- Strings are immutable.
- \+ is used to add strings together.
- \* is used to multiply strings.

#### Print Formatting with Strings
2 Methods:
- .format() method 
String String {} String String {}.format('variableToBeInserted1','variableToBeInserted2')
Can also use index position for example:

```python
myname = "Anas/Kayra"
myjob = "Computer Scientist"
myage = "21"

print("Hello my name is {} I am a {} and I am {} years old".format(myname, myjob, myage)) # Hello my name is Anas/Kayra I am a Computer Scientist and I am 21 years old

#can also use index, like this:
print("Hello my name is {0} I am a {1} and I am {2} years old".format(myname, myjob, myage)) # Hello my name is Anas/Kayra I am a Computer Scientist and I am 21 years old

# can also use keywords, like this:
print("Hello my name is {a} I am a {b} and I am {c} years old".format(a = myname, b = myjob, c = myage))

 ```

- f-strings (formatted string literals)
Similar to .format() but different implementation 

```python
myname = "Anas/Kayra"
myjob = "Computer Scientist"
myage = "21"

print(f"Hello my name is {myname} I am a {myjob} and I am {myage} years old") # Hello my name is Anas/Kayra I am a Computer Scientist and I am 21 years old
 ```

- .format() method can be also used for floats formatting, it can adjust the width and precision.

```python
myage = "21"

result = 21/9 #2.33333333
print("The result is {x:10.3f}".format(x = result)) # will make the size the result takes 10 it will fill the rest with white space and then it will be up to 3 decimal points.

 ```
 
 
 ### Lists
 - Lists are ordered sequences of objects.
 - Uses [] and , to seperate the objects.
 - Supports indexing and slicing.
 - Can have different types of objects.
 - Can add two lists together using +.
 - .append(object) is used to add a new object to the end of the list.
 - .pop(index) is used to remove the object with the index specified from the list, if an index wasn't provided the last element in the list will be removed (it returns the object popped).
 - Reverse indexing also works in lists.
 - .sort() sorts the list in alphabetical order (it doesn't return anything).
 - .reverse() sorts the list in the reverse order (returns nothing as well).



### Dictionaries
- Unordered mappings for objects and keys.
- Uses {} and : to assign the key, {'key1':'value1','key2':'value2'} d['key1'] will return 'value1'.
- Can have different types of objects.
- Can be nested/stacked.
- dictionary.key() returns all the keys in the dictionary.
- dictionary.values() returns all the values in the dictionary.
- d.items() returns all the keys and values in the dictionary together.


### Tuples
- Similar to lists but it's immutable (can't be changed).
- it uses () instead of [].
- tuple.count('string') returns how many times this string occured in the tuple.
- tuple.index('string') returns the index of the first occurrence of string.

### Sets
- They are unordered collections of unique elements.
- Same object can occur only once in the set.
- set.add(object) addes object to the end of the set.
- adding the same object willn't result in an error but it won't be added/repeated.
- set(list) can be used to get unique items in a list.

### Booleans
- True or False


## Input/Output with Basic Files
- myfile = open('filename') is used to open a file.
- myfile.read() returns all string in the file with \n being a new file.
- retyping the myfile.read() command will return null because the cursor is at the end of the file use myfile.seek(0) to get the cursor back to the start of the file.
- myfile.readlines() returns each line as an element of its own.
- to open a text file that's not in the same directory use the full path.
- myfile.close() is used to close the file.
- It's best practice to use with open('filename') as my_new_file: then you type enter and you can type commands to edit the file and not care about closing it.
- the default of the open function is read-only to be able to write use mode='w' so the command will be open('filename', mode='w').
- myfile.write('text to add') is used to write to a file.

### File Modes
| Name  | Description                                            |
| ------|--------------------------------------------------------|
| r     | Read only                                              |
| w     | Write only                                             |
| a     | Append (add to the file)                               |
| r+    | Read & Write                                           |
| w+    | Write and Read (will overwrite or create a new file)   |

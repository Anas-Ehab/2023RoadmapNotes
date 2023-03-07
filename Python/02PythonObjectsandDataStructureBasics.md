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

### Variable Assignments
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
- 
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
- + is used to add strings together.
- * is used to multiply strings.

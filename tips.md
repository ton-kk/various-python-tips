# python tips

This content is just a reminder for me. and my english practice.
## Basics

### version
now, python has two major version. ver 2 and  3.  
there are some difference. be cared python scripts version and your compilers version.  

check the version on command line.  

```
python --version
```
### declaration
set encoding name
```python
-*- coding: utf-8 -*-
```
### number
number (int, float) is immutable(not renewable)  
binary, octal, hex is 0bXX, 0oXX, 0xXX  
```python
intNum = 10
floatNum = 12.34
num = 0b10; print(num) # 2
num = 0o10; print(num) # 8
num = 0x10; print(num) # 16
```
### strings
str is immutable. enclose "XXX" or 'XXX'  
in multiple lines case, enclose """ XXX """ or ''' XXX '''  
```python
string = "hello python.";print(stinrg) # hello python.
string = 'hello python.';print(stinrg) # hello python.
string = """ hello
    python """;print(stinrg) # hello\n python.
```
### operator
```python
# x // y  "//" is integer division
10 // 3 # 3
# x % y "%" is surplus：余剰
10 // 3 # 1 
# x ** y "**" is exponentiation：累乗
10 ** 3 # 1000
```
operator(addition and multiplication) can also be used for strings.  
```python
print("hello" + " python.") # hello python.
print("hello " * 3) # hello hello hello 
```
### Array
list and tuple (and str) are similer. manage the object array.    
list is mutable. tuple is immutable.  
and str is array of letters.  
```python
# don't need list sample
tuple1 = () # empty tuple
tuple2 = 1, 2, 3
tuple3 = (4, 5, 6)
# access array
str = "abcdef"; print(str[-1]) # f
str = "abcdef"; print(str[1:3]) # bc
```
### dictionary
```python
dict = {'key':'value'}
listIncludeDict = {'key': [1, 2, 3, ... ]}

numToString = {1: 'str1', 2: 'str2', 3: 'str3', ... }
strTonumber = {'str1': 1, 'str2': 2, 'str3': 3, ... }
```
### class
class is most important. that has functions and variables. like a blueprint.  
if use class, must make instance of class.  
and functions 1st argument must be "self".  
```python
class className:
  def __init__(self):
    ...
  def functionName(self, arg1, ...):
    ...
  def functionName(self, arg2, ...):
    ...
classInstance = className()
# when create instance, __init__ function be done.
```
### re
"findall" return list include only string.  
```python
str = "22, 777aaa"
result = re.findall('[0-9]+', targetStr)
print(result)
# ['22','777', ... ]
```
"finditer" return match object Include lication too.  
```python
str = "22, 777aaa"
result = re.finditer('[0-9]+', targetStr)
for r in result:
  print(r)
# <re.Match object; span=(0, 2), match='22'>
# <re.Match object; span=(4, 7), match='777'>
```

## python tips

python codes I used sometimes.
This content is just a reminder for me.

### dictionary

```python
dict = {'key':'value'}
listIncludeDict = {'key': [1, 2, 3, ... ]}

numToString = {1: 'str1', 2: 'str2', 3: 'str3', ... }
strTonumber = {'str1': 1, 'str2': 2, 'str3': 3, ... }
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

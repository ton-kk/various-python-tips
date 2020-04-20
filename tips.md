## python tips

pthon codes I used sometimes.
This content is just a reminder for me.

### dictionary

```python
dict = {'key':'value'}
listIncludeDict = {'key': [1, 2, 3, ... ]}

numToString = {1: 'str1', 2: 'str2', 3: 'str3', ... }
strTonumber = {'str1': 1, 'str2': 2, 'str3': 3, ... }
```

### re
"findall" is only string. return list object. Include only string.

```python
re.findall('[0-9]+', targetStr)
# ['22','777', ... ]
```

"finditer" return match object list. Include lication.

```python
re.findall('[0-9]+', targetStr)
# ['22','777', ... ]
```

2020/04 i practice nlp(Natural Language Processing) now.  
this is my note about nlp practice.

```shell
sudo apt update
sudo apt upgrade

pip3 list
```

unicode data cleansing -> unicodedata  
full-width characters can be unified into half-width characters.  
but some symbols need to be full-wides.  
MeCab can't done well if half-width symbols in.  
```python
text = unicodedata.normalize('NFKC', text)
```


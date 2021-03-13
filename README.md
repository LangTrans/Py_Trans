# Python_Trans
Customzied python syntax with [LangTrans](https://github.com/LangTrans/LangTrans)
## Customized Syntax
```js
p"Hello World"
add = (x) => x+1
print|add|add(1)
try add("1") Exception print("Error:",err)
test ="test"
=test.replace("test","")
x = True
print((x||False)?"Done":"Failed")
print("Done") if x
```
## Orginal Syntax
```python
print("Hello World")
add = lambda x: x+1
print(add(add(1)))
try:
  add("1")
except Exception as err:
  print("Error:",err)

test ="test"
test=test.replace("test","")
x = True
print("Done" if (x if 'x' in locals() else False) else "Failed")
if x:
  print("Done")
```

If you find this more complicated than original or more syntax should be added to it, feel free to edit YAML files with your preference

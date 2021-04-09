# Python_Trans
Customized python syntax with [LangTrans](https://github.com/LangTrans/LangTrans)
## Customized Syntax
```py
p"Hello World"
inc = (x) => x+1
twice(x) = 2*x
add(x,y) = x+y
print(![inc => 1..6])
print|inc|inc(1)
try inc("1") Exception print("Error:",err)
test ="test"
=test.replace("test","")
print((x||True)?"Done":"Failed")
print('x is not defined') if !x
1 -> inc
|> print
print((inc+twice)(3))
#scope1#
print("Scope1")
print("Done")

#scope2#
print("scope2")
print("Done")
```
## Orginal Syntax
```python
print("Hello World")
inc = lambda x: x+1
twice = lambda x:2*x
add = lambda x,y:x+y
print(list(map(inc,range(1,6+1))))
print(inc(inc(1)))
try:
  inc("1")
except Exception as err:
  print("Error:",err)
test ="test"
test=test.replace("test","")
print("Done" if (x if 'x' in locals() else True) else "Failed")
if 'x' not in locals():
   print('x is not defined')
print(inc(3))
print(inc(3)+twice(3))
def scope1():
	print("Scope1")
	print("Done")
scope1()

def scope2():
	print("scope2")
	print("Done")
scope2()
```

If you find this more complicated than original or more syntax should be added to it, feel free to edit YAML files with your preference

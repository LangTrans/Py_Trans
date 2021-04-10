# Python_Trans
Customized python syntax with [LangTrans](https://github.com/LangTrans/LangTrans)
## Customized Syntax
```py
#Print
p"Hello World"
# Anonymous function
inc = (x) => x+1
# Lambda function
twice(x) = 2*x
# Single Line try-except
try inc("1") Exception print("Error:",err)
# Print Done if x is defined other wise Failed
print((x||True)?"Done":"Failed")
# Single Line if and check x defined or not
print('x is not defined') if !x
# Pipe Syntax
1 -> inc
|> print
# Arithmetic operations with functions 
print((inc+twice)(3))
#Scope syntax work like in javascript
#scope1#
print("Scope1")
print("Done")

#scope2#
print("scope2")
print("Done")

#PEP 359 - The "make" statement 
make type name(arg):
	x = 1
	y = 3

```

This is an example, feel free to edit the syntax in your way.
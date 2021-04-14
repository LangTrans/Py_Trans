# Python_Trans
Customized python syntax with [LangTrans](https://github.com/LangTrans/LangTrans)
## Customized Syntax
<table>

<thead>

<tr>

<th>Customized Syntax</th>

<th>Original Syntax</th>

</tr>

</thead>

<tbody>

<tr>



<td>

<pre>p"Hello World"</pre>

</td>

<td>

<pre>print("Hello World")</pre>

</td>

</tr>

<tr>



<td>

<pre>inc = (x) => x+1</pre>

</td>

<td>

<pre>inc = lambda x: x+1</pre>

</td>

</tr>

<tr>



<td>

<pre>twice(x) = 2_x
add(x,y) = x+y</pre>

</td>

<td>

<pre>twice = lambda x:2x
add = lambda x,y:x+y</pre>

</td>

</tr>

<tr>



<td>

<pre>1 -> inc 
|>print</pre>

</td>

<td>

<pre>print(inc(inc(1)))</pre>

</td>

</tr>

<tr>



<td>

<pre>try inc("1") Exception print("Error:",err)</pre>

</td>

<td>

<pre>try:
  inc("1")
except Exception as err:
  print("Error:",err)</pre>

</td>

</tr>

<tr>



<td>

<pre>print((x||True)?"Done":"Failed")</pre>

</td>

<td>

<pre>print("Done" if (x if 'x' in locals() else True) else "Failed")</pre>

</td>

</tr>

<tr>



<td>

<pre>print('x is not defined') if !x</pre>

</td>

<td>

<pre>if 'x' not in locals():
   print('x is not defined')</pre>

</td>

</tr>

<tr>



<td>

<pre>print((inc+twice)(3))</pre>

</td>

<td>

<pre>print(inc(3)+twice(3))</pre>

</td>

</tr>

<tr>



<td>

<pre>make type name:#Comment
    x = 1
    pass
    y = 3

make dict test:#Comment
    this =  "this"
    if this == "this":
        pass
    that = "that"</pre>

</td>

<td>

<pre>def name():
    x = 1
    return locals()
    y = 3
    return locals()
name = type("name", (), name())

def test():
    this =  "this"
    if this == "this":
        return locals()
    that = "that"
    return locals()

test = test()</pre>

</td>

</tr>

<tr>



<td>

<pre>#scope1#
print("Scope1")
print("Done")

#scope2#
print("scope2")
print("Done")</pre>

</td>

<td>

<pre>def scope1():
    print("Scope1")
    print("Done")
scope1()

def scope2():

    print("scope2")

    print("Done")

scope2()</pre>

</td>

</tr>

</tbody>

</table>

This is an example, feel free to edit the syntax in your way.

---
title: "Python Data Types"
datePublished: 2020-06-19T23:00:02.000Z
cuid: ckmbxgw0u06w95ns1djio7u2c
slug: python-data-types
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1615893834783/eUyPRNPe3.jpeg

---


In programming, data type is an important concept.

Variables can store data of different types, and different types can do different things.

Every value in Python has a datatype. Since everything is an object in Python programming, data types are actually classes and variables are instance (object) of these classes.

## Python Contains 12 built-in data types

* 4 Numeric Type [ int , float , complex , bool ] 
* 4 Sequence Type [ str , list , tuple , range ]
* 2 Set Type [ set, frozenset ]
* 1 Mapping Type [ dict ]
* 1 Binary Type: [ bytes ]


## Mutable VS Immutable

|                |                            |
| -------------- |:--------------------------:|
| Mutable        | Values Changed             |
| Immutable      | Values Cannot Be Changed   |


![Mutable VS Immutable](https://cdn.hashnode.com/res/hashnode/image/upload/v1615893831167/V1-44vh0m.png)

![Data Types: Mutable VS Immutable](https://cdn.hashnode.com/res/hashnode/image/upload/v1615893833000/Njceb0gCJ.png)



## Data Type In Action

<table>
<tbody>
<tr>
<th>Example</th>
<th>Data Type</th>
</tr>
<tr>
<td>x = "Hello World"</td>
<td>str</td>
</tr>
<tr>
<td>x = ["apple", "banana", "cherry"]</td>
<td>list</td>
</tr>
<tr>
<td>x = ("apple", "banana", "cherry")</td>
<td>tuple</td>
</tr>
<tr>
<td>x = range(6)</td>
<td>range</td>
</tr>
<tr>
<td>x = 20</td>
<td>int</td>
</tr>
<tr>
<td>x = 20.5</td>
<td>float</td>
</tr>
<tr>
<td>x = 1j</td>
<td>complex</td>
</tr>
<tr>
<td>x = True</td>
<td>bool</td>
</tr>
<tr>
<td>x = {"apple", "banana", "cherry"}</td>
<td>set</td>
</tr>
<tr>
<td>x = frozenset({"apple", "banana", "cherry"})</td>
<td>frozenset</td>
</tr>
<tr>
<td>x = {"name" : "John", "age" : 36}</td>
<td>dict</td>
</tr>
<tr>
<td>x = b"Hello"</td>
<td>bytes</td>
</tr>
</tbody>
</table>

Thus, Try with these snippets.

---
layout: default
title:  "Tetriminoe Rotation"
date:   14-7-2017
categories: programming
excerpt: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut nunc risus, tincidunt vel arcu id, viverra tristique est.
---

{{ page.title }}
================


**Representation**

Represent each piece in the minimum matrix where 1's represent spaces occupied by the tetriminoe and 0's represent empty space. Example:

<pre><code>originalMatrix = 
[0,   0,   <b>1</b>]
[<b>1</b>,   <b>1</b>,   <b>1</b>]
</code></pre> 
    

![enter image description here](https://i.stack.imgur.com/BfZKD.jpg)

**Rotation Formula**

    clockwise90DegreesRotatedMatrix = reverseTheOrderOfColumns(Transpose(originalMatrix))

    anticlockwise90DegreesRotatedMatrix = reverseTheOrderOfRows(Transpose(originalMatrix))


**Illustration**

<pre><code>originalMatrix = 
  x    y    z
a[0,   0,   <b>1</b>]
b[<b>1</b>,   <b>1</b>,   <b>1</b>]
</code></pre>   

<pre><code>transposed = transpose(originalMatrix)
  a   b
x[0,  <b>1</b>]
y[0,  <b>1</b>]
z[<b>1</b>,  <b>1</b>]
</pre></code>

<pre><code>counterClockwise90DegreesRotated = reverseTheOrderOfRows(transposed)
  a   b
z[<b>1</b>,  <b>1</b>]
y[0,  <b>1</b>]
x[0,  <b>1</b>]
</pre></code>

![enter image description here](https://i.stack.imgur.com/cTiEk.jpg)

<pre><code>clockwise90DegreesRotated = reverseTheOrderOfColumns(transposed)
  b   a
x[<b>1</b>,  0]
y[<b>1</b>,  0]
<[<b>1</b>,  <b>1</b>]
</pre></code>

![enter image description here](https://i.stack.imgur.com/fTvMj.jpg)

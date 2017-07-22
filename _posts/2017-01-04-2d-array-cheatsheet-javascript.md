---
id: 861
title: Cheatsheet for working with 2D arrays in JavaScript
date: 2017-01-04T23:27:25+00:00
author: Nick Ang
layout: post
guid: http://www.nickang.com/?p=861
permalink: /2d-array-cheatsheet-javascript/
categories:
  - technical
tags:
  - javascript
  - programming
---
Arrays are basic data structures present in all programming languages I've been worked with so far: JavaScript, Ruby, Python, PHP. It's easy enough to understand normal arrays but I've found that introducing an extra layer (ie. a second dimension) makes it exponentially harder to work with. This cheatsheet is a growing list of tips and tricks for using 2D arrays in JavaScript. The idea is portable to other languages, since the ideas are universal. 

### Rule #1: Always use a 1D array if you can help it 

We can represent a grid, say a tic tac toe board, using a single array:

```
var grid = [
  1, 2, 3,
  4, 5, 6,
  7, 8, 9
]
```

But I've seen people opt for a 2D array instead:

```
var grid2D = [
  [1, 2, 3],
  [4, 5, 6],
  [7, 8, 9]
]
```

I wonder, why would anyone do that, especially for a small 3x3 grid? I couldn't come up with a good, sensible answer. Accessing the 2D array is pain compared to the 1D array using iterators:

```
grid.forEach(function (element, index, array) {
  // do something
})

grid2D.forEach(function (element, index, array) {
  // here we have access to the rows 1, 2, 3
  element.forEach(function (element2d, index2d, array2d) {
    // now we have access to each individual box
  })
})
```

What about when the array is much larger? Say, 10x10? Let's also use a `for` loop to generate them so we don't have to manually generate the array (because we're lazy!):

```
// 1D array of 100 elements
var grid100 = []
for (var i = 0; i < 100; i++) {
  grid100.push(i + 1)
}

// grid100 = [
  1,2,3,4,5,6,7,8,9,10,
  11,12,13,14,15,16,17,18,19,20,
  21,22,23,24,25,26,27,28,29,30,
  31,32,33,34,35,36,37,38,39,40,
  41,42,43,44,45,46,47,48,49,50,
  51,52,53,54,55,56,57,58,59,60,
  61,62,63,64,65,66,67,68,69,70,
  71,72,73,74,75,76,77,78,79,80,
  81,82,83,84,85,86,87,88,89,90,
  91,92,93,94,95,96,97,98,99,100
]


// 2D array of 100 elements in 10x10
var grid10x10 = []
var row = []
for (var i = 0; i < 100; i++) {
  if (i.toString().indexOf('0') !== -1) {
    row.push(i)
    grid10x10.push(row)

    row = []
  } else {
    row.push(i)
  }
}

// grid10x10 = [
  [1,2,3,4,5,6,7,8,9,10],
  [11,12,13,14,15,16,17,18,19,20],
  [21,22,23,24,25,26,27,28,29,30],
  [31,32,33,34,35,36,37,38,39,40],
  [41,42,43,44,45,46,47,48,49,50],
  [51,52,53,54,55,56,57,58,59,60],
  [61,62,63,64,65,66,67,68,69,70],
  [71,72,73,74,75,76,77,78,79,80],
  [81,82,83,84,85,86,87,88,89,90],
  [91,92,93,94,95,96,97,98,99,100]
]
```

With the 2D array, we're basically splitting a grid into columns and rows. So if we were to iterate through every single element, we'd have a `for` loop nested inside another `for` loop, which means we'll go row by row, and within each row, we'll go from column 1 to the last column. To this rhythm...

R1 C1 >> R1 C2 >> R1 C3 >> ... >> R1 C10
R2 C1 >> R2 C2 >> R2 C3 >> ... >> R2 C10
...
R10 C1 >> R10 C2 >> R10 C3 >> ... >> R10 C10

Now would it make more sense to use a 2D array? Will it provide greater versatility down the road when we want to manipulate the array? 

**2D array is good for accessing an element based on a specific coordinate**

2D arrays would indeed be superior to 1D arrays if we could access an element based on a specific coordinate, like R3 C6. Do they give us that flexibility? 

Yes. R3 C6? That's as simple as calling `grid[2][5]`! We now have access to the value 26. That was much easier than using a 1D array, which would require us to first do some calculations before being able to pinpoint the value of a specific element that corresponds to the third row fifth column. 

What happens if we need to programmatically change values of the elements _surrounding_ a specific element? 

I'll explore this in tomorrow's update of this article!

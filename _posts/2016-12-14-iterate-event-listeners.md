---
id: 822
title: How to add event listeners without repeating yourself
date: 2016-12-14T21:00:59+00:00
author: Nick Ang
layout: post
guid: http://www.nickang.com/?p=822
permalink: /iterate-event-listeners/
categories:
  - technical
tags:
  - javascript
  - programming
  - technical
---
One of the key principles of good programming is DRY - Don't Repeat Yourself!

Here's one way to reduce repetition with event listeners by using an array `.forEach` iterator that I've used a number of times now. If you haven't done this before, here you go! If you have an even cleaner and easy to understand solution, please share. 

The code below uses jQuery selectors and methods to add 'mousedown' event listeners to 4 elements #up, #down, #left and #right. 

```
// NON-DRY WAY
// Add event listeners to mouse downs
$('#up').mousedown(function () {
  mouseStillDown = true
  moveBall('up')
})
$('#down').mousedown(function () {
  mouseStillDown = true
  moveBall('down')
})
$('#left').mousedown(function () {
  mouseStillDown = true
  moveBall('left')
})
$('#right').mousedown(function () {
  mouseStillDown = true
  moveBall('right')
})

// DRY WAY
// Add event listeners to mouse downs
var directions = ['up', 'down', 'left', 'right']

directions.forEach(function (direction) {
  $('#' + direction).mousedown(function () {
    mouseStillDown = true
    moveBall(direction)
  })
})
```

Code used in an [in-class lab](https://nickangtc.github.io/moving-ball/) to move a ball around the page. 
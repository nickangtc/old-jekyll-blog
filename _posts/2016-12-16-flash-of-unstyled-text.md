---
id: 827
title: The flash of unstyled text
date: 2016-12-16T07:16:26+00:00
author: Nick Ang
layout: post
guid: http://www.nickang.com/?p=827
permalink: /flash-of-unstyled-text/
categories:
  - technical
tags:
  - javascript
  - programming
  - technical
---
When I entered the web development industry-complex (is it okay to refer to it as such?) in August this year, the first thing I noticed was how fast it moved. This year EJS and HAML is hot, next year it's testing frameworks Mocha and Chai, and then Angular2 and React. In our industry, there has been a hot new thing every year. 

Recently in a bid to give a well thought out response to a student in class, the instructional team did some googling to see if some esoteric library existed to allow developers to recreate poster-esque typography on webpages. And of course we found one, called [Lettering.js](http://letteringjs.com/). It uses jQuery to transform every single letter in a sentence into a `<span>` tag, and style it accordingly. Kerning (horizontal spacing in between letters) is easy with margins and relative positioning, and alternating colours is also possible with the `:nth-child` selector. I thought it is really smart but a bit of an overkill.

But what caught my attention most was a paragraph that espoused the values of the creators of [Lettering.js](https://github.com/davatron5000/Lettering.js):

> "Web performance patterns advise that you put Javascripts at the bottom of your page before your `</body>` tag. There is an unfortunate side effect where you may experience a FOUT (Flash of Unstyled Text) when you're manipulating your text after the DOM has loaded. Unfortunately, we found the best solution to avoid/minimize the FOUT caused by this plugin is to put your scripts (jQuery, Lettering.js) in the document <head>. On the one hand, your page will load slower. On the other hand, a flash/restyling makes your site feel slow. Users might ultimately feel the site is faster if they don't see the FOUT.”

FOUT. What an acronym. To FOUT or not to FOUT is one of many design decisions that developers have to make every day. While the implementation is very simple in this case--moving the `<script>` tag between the top (at the HTML head) position or the bottom (as the last few lines within the HTML body)--what/how we decide ultimately depends on the project. 

The most interesting part about having read this is that I never scrutinised the difference between placing the `<script>` tags on top or below. I just placed it in the head all the team and used a DOMContentLoaded/jQuery.ready inside my scripts to make sure that the HTML page is fully rendered before JavaScript tries to manipulate them on the DOM. 

How fascinating... 
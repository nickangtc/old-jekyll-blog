---
id: 543
title: Always get the basics first
date: 2016-08-21T11:52:11+00:00
author: Nick Ang
layout: post
guid: http://www.nickang.com/?p=543
permalink: /always-get-the-basics-first/
categories:
  - thought of the day
tags:
  - learning
  - programming
  - startup
---
[caption id="attachment_545" align="aligncenter" width="840"]<img class="wp-image-545 size-large" src="http://www.nickang.com/wp-content/uploads/2016/08/20160819-DSCF8120-1024x683.jpg" alt="classroom of students at general assembly singapore learning programming" width="840" height="560" /> Week 1 at GA Singapore is trying to get the very basics of HTML, CSS, JavaScript[/caption]

Whenever learning something new, start with the basics. Web programming has become a mature enough industry to have its own set of community-made tools that purport to help make coding easier, but it’s a mistake to learn those before nailing down the basics, as I did.

I started learning to code on my own, in the comfort of my pyjamas at home, using <a href="http://www.freecodecamp.com">Free Code Camp</a> (my learning profile <a href="http://www.freecodecamp.com/nickangtc">here</a>). (Well, that was my first real push to learn anyway.) To be clear, Free Code Camp does not encourage students to pick up jQuery before understanding doing a lot of JavaScript exercises.

No, I decided to extend my projects by using libraries like <a href="https://jquery.com/">jQuery</a> (to supercharge JavaScript) and <a href="http://getbootstrap.com/">Bootstrap</a> (to enhance CSS) on my own. It felt nice to have to write less and still have things somehow work. I didn’t think much into it then, but now that I’m enrolled in a proper web development course, I’m beginning to see how problematic this approach can be.

I never had figured out how grids work when I used Twitter Bootstrap.

I never knew how cumbersome and difficult it is to read <code>document.getElementById(‘id’)</code> and how <code>.addClass()</code> in jQuery is actually <code>.classList.add()</code> in vanilla JavaScript.

I never even knew that web developers ought to know that there’s such a thing as ‘vanilla JavaScript’. The community is just so active in making things easier for one another—by creating libraries like jQuery and Bootstrap and hundreds or thousands more—that a newbie would think it’s natural (and the right thing to do) to use all that are necessary for their projects. As long as it makes things easier, we’d be foolish not to use them, right?

Well, you probably sensed by now that I’m going to say, “wrong!”

Without first knowing that a grid is made up of simpler blocks—like <code>div</code>s, one may run into perplexing problems using Bootstrap’s grid system, which formats things into blocks nicely straight out of the box.

Similarly, using <code>$(“idName”).on(“click”, function(){code})</code> in jQuery without first knowing its extremely lengthy but somewhat more detailed vanilla cousin, <code>document.getElementById(“idName”).addEventListener("click", function(){code}))</code>, the concept of an event listener might just fly over one’s head.

And we haven’t even touched on dependencies. What happens if you created a kick-ass web app that was built on these libraries, without knowing vanilla JavaScript, and the host servers get shut down? What happens if Twitter decides, as Facebook recently attempted by adding a <a href="https://news.ycombinator.com/item?id=12108158">sneaky clause into the React.js open-use license</a>, to revoke your startup’s license to use Bootstrap (which it developed)?

Having dependencies can create vulnerabilities for your business. Knowing the basics means being able to circumvent becoming a victim of corporate bullying by creating projects built on what is truly open-source. (Vanilla JavaScript will never be inaccessible to anyone, I don’t think, unless Mozilla wants to take down the entire world wide web!)

Boiled down, the point here is that every newbie programmer should pick up the basics of each language (HTML, CSS, JavaScript, Java, Python, etc.) before strapping booster rockets to their projects. That way you won’t ever find yourself like a penguin halfway up the stratosphere.
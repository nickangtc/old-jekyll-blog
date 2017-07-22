---
id: 611
title: Why programmers make visually ugly projects
date: 2016-09-08T22:50:45+00:00
author: Nick Ang
layout: post
guid: http://www.nickang.com/?p=611
permalink: /programmers-ugly-projects/
categories:
  - thought of the day
tags:
  - internet
  - life
---
<img src="http://www.nickang.com/wp-content/uploads/2016/09/20160907-IMG_20160907_211409-1024x578.jpg" alt="people laughing and talking with one another general assembly wdi singapore" width="840" height="474" class="aligncenter size-large wp-image-615" />

As a user, it used to be hard for a website to impress me. I see certain features here and others there, and after a while, I get a good idea of what is possible and is usually practiced, and that guides my behaviour on the web. I’d expect that hitting ‘enter’ will submit a login form. 

Now, I’m much more easily impressed. Why? Because I now know how much thinking and coding goes on behind the scenes to make simple things such as updating a user profile work. Here’s an illustration with editing a profile:

1. user clicks ‘edit profile’ button
2. client-side sends a GET request to server-side (to fetch the edit profile page with the form to edit)
3. server-side finds the exact match of GET request, gets a lot of different info from database, sends data that makes up the edit page to client-side
4. client-side continues to run…
5. client-side receives data, manipulates data, and refreshes the webpage with form (pre-populating the form with existing info)
6. user makes edits, hits ‘save’
7. client-side makes POST request to server-side with user’s data input
8. server-side receives data
9. server-side manipulates data, updates database
10. server-side redirects within itself to the GET request (a la step 3)
11. server-side sends response to client-side via GET
12. user’s browser refreshes to profile page

What used to be intuitive is not so intuitive. For the first iPhone to feel intuitive, a lot of work was put in by Steve Jobs and the Apple team behind the scenes. As internet users, things feel intuitive when they behave in ways that are consistent with how things normally behave in reality. 

But the internet is completely virtual—you can never hold it in your hands and get a feel for its texture—and that makes it a big challenge for programmers and engineers and designers to to make things feel *right*. So far though, I think they have done a great job (hat-tip to the people working on the first iPhone, which changed everything with a large, multi-touch touchscreen with gesture controls and more). 

I found myself wow-ing a lot in class today alongside my classmates. That said, I bet you would never guess what we were looking at. Steve, our instructor, showed us this:

<img src="http://www.nickang.com/wp-content/uploads/2016/09/screenshot-bestbuy-1024x504.png" alt="screenshot of simple website mockup of Best Buy" width="840" height="413" class="aligncenter size-large wp-image-613" />

Yep, an *extremely* simple rendition of Best Buy’s website with admin controls to create, edit, and delete product pages. Having only just learned how to set up a (locally-hosted) server using Node.js, this was a big leap forward in technicality for us, and I stopped to wonder just how complex some programmes out there really are. 

Here’s one last observation from today: programmers are so busy making sure that the code works (ie. doesn’t break) that styling a webpage is one of the last priorities for them. It’s true - I almost always leave CSS for last now. I think of it as a veneer that is important, yes, but my job is to ensure that the product functions as it is intended - and that is a full-time job in itself. 
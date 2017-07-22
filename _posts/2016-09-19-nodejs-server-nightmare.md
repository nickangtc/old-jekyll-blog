---
id: 652
title: The nightmare of coding a node.js server
date: 2016-09-19T23:30:04+00:00
author: Nick Ang
layout: post
guid: http://www.nickang.com/status-private/
permalink: /nodejs-server-nightmare/
categories:
  - thought of the day
tags:
  - opinion
  - programming
  - technical
---
<img src="http://www.nickang.com/wp-content/uploads/2016/09/lion-lying-down-1024x684.jpeg" alt="lion lying restlessly on the ground" width="840" height="561" class="aligncenter size-large wp-image-655" />

Setting up a <a href="https://nodejs.org/en/">node.js</a> server is not the same as writing HTML, CSS or JavaScript. It's much more complicated than that, and honestly, I think it shouldn't be. 

So, HTML handles what is displayed on the page, CSS alters the way these HTML elements look, and JavaScript manipulates these elements dynamically according to user action. While the process of writing JavaScript code, which is the only real programming language among the three, can be at times very challenging, it is almost always easy to identify the reasons you're stuck. You might be stuck because you were experimenting anyway, or because you used a string method on an array or something like that. After coding (and staring at code I've written) for a while, I'd usually recognise a pattern and be able to fix the problem. 

On the end of the spectrum as I've recently stumbled upon is node.js and its host of libraries. Ok, I didn't really stumble upon them so much as I was told to use them by my instructors at General Assembly. Anyway, Node.js is an engine that ports the JavaScript language to be used in projects other than those that run on browsers. In my case, I'm learning to use it as a server side language to build a server for my web project, and it's been a nightmare. Here's why... 

Node.js comes with a slew of external libraries that do things. In practice, these are more like essentials than addons. Express, body-parser, ejs view engine, passport.js, sequelize database handler, and much, much more are almost *requirements* for node.js to work as a server. 

If it were merely about dependencies I would just live with it, especially at this learning stage, but that is definitely not the case with this house of cards. The biggest issue I'm facing with writing code for the back-end (ie. server) using node.js is the acrobatics it requires of me. 

I'll use the example of trying to set up user authentication to bring you through the source of my recent headaches. 

## The nightmare of setting up user authentication with passport.js 

Ok, here goes. To set up a web app with user sign up and login (what we call authentication and, when it pertains to permission to view certain pages, authorisation), we need to use an external library called <a href="http://passportjs.org/">passport</a>. 

A little on what that means. Passport is a package for Node, and Node in turn is the platform on which our entire server is built. It's called node.js because it ports the JavaScript language, which was designed and built around browsers, to the server side of things. It's a big, great deal to have something like node.js exist. For one, it saves me from having to learn a server side language like PHP. 

Before I can write a line of code that defines the logic for authentication and authorisation, I need to set up my server to "require" these and various other packages. In this case, I also need the <a href="https://github.com/expressjs/session">express-session</a> package because passport needs that to work. 

After writing a bunch of "require" and "app.use" statements, I then have to create new folders to store a few other files that are absolutely necessary for it to function properly: 
1. /config/ppConfig.js to set up the behaviour of passport 
2. /controllers/auth.js to receive the signup, login and logout routes and control what happens when the user lands on the page 

After this, let me see... Oh ya, after this, I'm supposed to create a "hook" to make sure that when a new user signs up, the info passed into the form and into server are sanitised and the password is hashed (ie. encrypted) before they get stored in the database. That requires using--and thus, learning--two more node packages (bcrypt for encryption and sequelize for communicating with a SQL database using JavaScript instead of Structured Query Language), so I think I'm going to take a break first.

Ok, I'm back, and quite frankly I don't feel inclined to spell out the rest of the process. It's just mind-numbing! (If you have questions though, I'll gladly help as I can. Just post your question as a comment.) 

## What is the point? 

Yes, I have a point I'm trying to make, and it's this: it shouldn't be this hard! 

I've read in several places about a particular kind of professional whose main goal is to build systems so that life can be better, less repetitive and mundane, more colourful... 

Programmers are not supposed to have to deal with unnecessary complexity, and this is clearly what it is. It should be easier. With a community as lively as it can possibly be, there should be a project to unite these common server tasks (how many websites don't need authentication and authorisation nowadays?) into a much leaner machine. 

Until that happens, I'm afraid the only way out is through. 

(image: <a href="https://unsplash.com/@joel_herzog">Joel Herzog</a>)
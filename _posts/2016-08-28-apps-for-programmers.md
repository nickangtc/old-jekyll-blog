---
id: 571
title: Alfred and other apps for the programmer
date: 2016-08-28T21:53:41+00:00
author: Nick Ang
layout: post
guid: http://www.nickang.com/?p=571
permalink: /apps-for-programmers/
categories:
  - thought of the day
tags:
  - programming
  - tools
---
[caption id="attachment_573" align="aligncenter" width="840"]<img class="wp-image-573 size-large" src="http://www.nickang.com/wp-content/uploads/2016/08/chilling-1024x683.jpeg" alt="relaxing in a pool by snow mountains" width="840" height="560" /> Tools conserve cognitive resources for the actual tasks! Image: <a href="https://unsplash.com/@robsonhmorgan">Robson Morgan</a>[/caption]

I now recall that about a year ago, I was introduced to the productivity app called Alfred. I tried it but couldn’t understand why anyone found it useful, and swiftly proceeded to uninstall it within the week.

I learned about the Alfred app listening to Tim Ferriss interview a man named Noah Kagan on his podcast. Noah has had an illustrious career spanning the early days at Facebook and Mint.com, and he eventually founded his own tech company, SumoMe. He is now one of hundreds of interviewees on the Tim Ferriss Show podcast, one of my favourite podcasts of all time.

But I’m not going to talk about podcasts here; I want to talk about the tremendous quality and quantity of tools that are available out there on the world wide web at our disposal.

Let’s do a stock take right now. Since I began attending classes at General Assembly two weeks ago, I’ve downloaded a number of tools that purport to make my life better (as a programmer):
<ul>
 	<li><a href="https://atom.io/">Atom</a> code editor</li>
 	<li>Atom external packages: JSLinter, <a href="http://emmet.io/">Emmet</a>, highlight-selected, standard-formatter</li>
 	<li><a href="https://kapeli.com/dash">Dash</a> offline documentation dashboard</li>
 	<li><a href="https://slack.com/">Slack</a> app for team/community chats</li>
 	<li><a href="https://chrome.google.com/webstore/detail/colorzilla/bhlhnicpbhignbdhedgjhgdocnmhomnp?hl=en">ColorZilla</a> extension for Chrome</li>
 	<li><a href="https://www.alfredapp.com/">Alfred</a> app</li>
</ul>
In two weeks I’ve downloaded these and more, and they’ve been quite helpful in specific ways.

<a href="http://www.atom.io">Atom</a> code editor has integration with my command line and Git, so whenever there are “uncommitted” changes in my code files I can see them at a glance.

The various external packages are even more powerful. JSLinter constantly reads my JavaScript file for missing semicolons, undefined variables that are meant to be defined, functions defined that haven’t been used anywhere in the code, and more. <a href="http://emmet.io/">Emmet</a> is the most beautiful implementation of an open source tool I’ve come across so far, replacing this:
<pre>&lt;div id="left-pane" class="col-sm-4 img-fit"&gt;
 &lt;span class="pixel" id="pix-l-1"&gt;&lt;/span&gt;
 &lt;span class="pixel" id="pix-l-2"&gt;&lt;/span&gt;
 &lt;span class="pixel" id="pix-l-3"&gt;&lt;/span&gt;
 &lt;span class="pixel" id="pix-l-4"&gt;&lt;/span&gt;
 &lt;span class="pixel" id="pix-l-5"&gt;&lt;/span&gt;
 &lt;span class="pixel" id="pix-l-6"&gt;&lt;/span&gt;
 &lt;span class="pixel" id="pix-l-7"&gt;&lt;/span&gt;
 &lt;span class="pixel" id="pix-l-8"&gt;&lt;/span&gt;
 &lt;span class="pixel" id="pix-l-9"&gt;&lt;/span&gt;
 &lt;span class="pixel" id="pix-l-10"&gt;&lt;/span&gt;
&lt;/div&gt;</pre>
<div id="left-pane" class="col-sm-4 img-fit"></div>
With this:
<pre>div#left-pane.col-sm-4.img-fit&gt;span.pixel#pix-l-$*10

// chunk 1
div$left-pane.col-sm-4.img-fit 

// chunk 2
&gt;span.pixel#pix-l-$*10
</pre>
With Emmet, 12 lines of HTML can be generated with one sentence. A simple tab will expand the sentence into all that HTML. The time savings is enormous.

Another tool I’m already starting to fall for is Dash. It allows me to continue to code with reference to official documentation while I’m disconnected from the internet. Talk about liberating.

A guy—I think is called Jensen—who works at ThoughtWorks introduced it to us two days ago, and I’d already found a use for it yesterday. At 7am, alone at a Subway store in Marina Square that wasn’t even open, I was working on a project and needed to refer to the Emmet documentation—to generate 100 <code>span</code>s with unique IDs—but had no access to the internet. Dash came in extremely handy.

Today I’m going to bring <a href="http://www.alfredapp.com">Alfred</a> for a test drive. If I don’t feel compelled to uninstall it by the end of the day, I think it’ll join my rapidly growing repertoire of tools. It’s amazing that all these are available for free. I couldn’t be happier. Maybe one day I’ll pay my debt to the community by working on an open source tool…
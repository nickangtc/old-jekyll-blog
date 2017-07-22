---
id: 413
title: My first full month of learning code everyday
date: 2016-06-23T22:03:37+00:00
author: Nick Ang
layout: post
guid: http://www.nickang.com/?p=413
permalink: /learning-code-everyday-may-jun-2016/
categories:
  - mu
tags:
  - blog
  - learning
  - programming
---
A blink of an eye and it's been almost a month since I posted anything here.

Nope, I haven't got an epiphany to write about some big idea. I just miss logging things and having the option of a guided walk down memory lane whenever I feel like one. So I'm going to talk a little about what's been happening this past month.

I'll start with today.

We played a nice game of badminton in the morning with my university friend Ezra at NTU. Mei has only been playing with twice and I can tell she's already getting better at the game. I mean, she was kicking our asses. Part of my shoe sole came off halfway though (because she served the shuttlecock to the wrong half of the court and I stupidly ran after it by reflex), so I didn't get the chance to claim victory. Or so I tell myself.

Then our usual lunch at the Business School, and then back home.

At home I spent the remaining 3-4 hours coding. I'm currently coding a simple Wikipedia search engine webpage that works in this sequence: User enters search query --&gt; backend code sends the query to Wikipedia's server --&gt; Wiki server returns data related to search query --&gt; front-end code displays data in human-friendly results. Been working on <a href="http://codepen.io/nickang/full/VjKQEP" target="_blank">this</a> for the second day straight now. Should be done by the time this post goes online.

Before long, my parents came to pick us up for dinner. We ate some delicious Chinese food at an upmarket restaurant called Pu Tien in an upmarket shopping mall, Ion Orchard.

[caption id="attachment_418" align="aligncenter" width="840"]<img class="wp-image-418 size-large" src="http://www.nickang.com/wp-content/uploads/2016/06/DSCF0239_nickang_edited-1024x683.jpg" alt="wife banter with husband" width="840" height="560" /> Banter while waiting to be seated.[/caption]

[caption id="attachment_417" align="aligncenter" width="840"]<img class="size-large wp-image-417" src="http://www.nickang.com/wp-content/uploads/2016/06/DSCF0260_nickang_edited-1024x683.jpg" alt="women carrying mannequins" width="840" height="560" /> Caught human trafficking at Ion Orchard shopping mall. Busted![/caption]

[caption id="attachment_419" align="aligncenter" width="840"]<img class="wp-image-419 size-large" src="http://www.nickang.com/wp-content/uploads/2016/06/DSCF0253_nickang_edited-1024x683.jpg" alt="An Asian face like you've never seen" width="840" height="560" /> An Asian face like you've never seen[/caption]

That about sums up my day today.
<h5>May-June 2016: Post-US trip</h5>
Since we got back from our month-long trip around the US (from New York to Los Angeles), I've been busy coding. It's the first time I'm learning to code this furiously. My hunger to know how to code is growing by the day, and it feels great.

These are interesting times. Code is not like English, though they're both languages. Knowing code isn't exactly going to let you 'talk' to your computer. Programming language syntax is like English vocabulary, but the grammar is completely haywire. A lot of times I want my webpage to do something but it ends up doing everything else but what I intended. If it were like talking to a computer, I'd be able to tell it like in a conversation. Nope, we're not there yet with technology.

Programming also differs from talking because of the logic involved. In speech and in writing, we imply certain things, like who's saying what in a dialogue between two characters in a novel, or the fact that the car we're talking about has four wheels and runs on petrol.

To a computer, though, nothing is implied. Instead, everything is and must be spelled out. Firstly for the computer to understand what you want it to do, and then secondly for other humans who might have to read your code to understand what you were trying to accomplish when writing different lines of code.

It's not easy learning to code from scratch. But the good news is, 'scratch' is no longer below sea level. In 2016, learning from scratch is no longer starting from zero - all the free resources online that have been made by people to teach and empower others to make software have made the barrier to entry significantly lower.

That said, I must maintain that it's not easy to learn. Don't listen to the "programming is easy!" hype. Nonsense. Quincy Larson's <a href="https://medium.freecodecamp.com/one-does-not-simply-learn-to-code-f25bacdc5b62#.uzv6zmkj8" target="_blank">post</a> gives newcomers a better preview into what it's like psycho-emotionally to learn to code. (Larson is the founder of Freecodecamp, the free online course where I'm learning to code from.)

The tools and scrolls are more attainable than they've ever been in history, but becoming proficient at reading and writing code still takes a great deal of patience and time. It is, after all, a skill.

(Becoming good is also difficult because programming languages and protocols and standards continue to evolve quickly. HTML5, Ruby on Rails, etc.)

Last week I was stuck on a coding challenge where I was supposed to write a web app that tells you the weather in your city. The sequence of events that the code needed to handle was something like this:
<ol>
 	<li>Ask you for permission to get your location.</li>
 	<li>Get your location through Chrome's built-in geolocating feature (works only with Chrome users).</li>
 	<li>Send a 'get' request to a weather server with your location.</li>
 	<li>Receive location-specific weather data and display them on screen.</li>
</ol>
I worked on it everyday for close to two weeks, hitting obstacle after obstacle.

I know, I know, I'm new to the whole thing so that pace is normal! But here's where I stop you. Though you're probably right, the way that is said makes it sound too easy.

You see, I was stuck on a very specific problem. I could write out the sequence of events that needed to take place for the programme to work right from the moment I received the challenge - the structure wasn't the problem. It was <em>what</em> code to use to implement that sequence that baffled me.

For example, while asynchronous processes made sense to me (multiple things happening at the same time to reduce a user's waiting time on a webpage), actually trying to put them in a queue (so that code chunk B is able to execute using some data returned from code chunk A which operates asynchronously) wasn't at all straightforward when you have to code (not write) it out. It wasn't easy, until it become easy - when I finally figured it out.

Now it's really quite straightforward to me. When an async operation has successfully completed, you can declare a callback function whose code will then be executed, and the way you do that is to...

Okay, I'm not quite ready for technical writing yet so I'll skip the details.

Anyway, the process was gruelling. That's my point. I tried many different methods to try to achieve the result I wanted over the two weeks and I was on the verge of giving up <em>a few times</em>. But whenever I came close to quitting, I just told myself to stop coding and go do something else.(That's usually reading or watching Casey Neistat vlogs.) I'd have nothing to lose. Just put it all down and take a breather. I can come back if I felt like it later in the day. I'd close the <a href="https://www.freecodecamp.com/nickangtc" target="_blank">Free Code Camp</a> and <a href="http://codepen.io/nickang" target="_blank">Codepen</a> tabs in my browser, along with the 10-20 tabs on HTML/CSS/JavaScript tutorials and references, and just move on to something else for a couple of hours.

Then I'd come back with a fresh-enough eye and mind to tackle the problem again. Eventually I solved it. You can imagine how happy I was when I finally understood a viable method to handle async processes in JavaScript. (Okay again, maybe not. Not until you try coding yourself.) I don't think learning a new word or way of expressing myself in writing or speech in English can ever bring me that kind of euphoria that learning code does.

All's going well so far. My mind's still set on the long game of creating a company that's good for society. Coding is the means to that end, and I'm focused on getting good at it right now. The rest should fall in place bit by bit, pun proudly intended.
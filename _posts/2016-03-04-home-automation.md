---
id: 50
title: 'What We Mean When We Say &#8216;Home Automation&#8217;'
date: 2016-03-04T12:04:00+00:00
author: Nick Ang
layout: post
guid: http://www.nickang.com/?p=50
permalink: /home-automation/
categories:
  - mu
tags:
  - arduino
  - hacking
---
There are at least two kinds of home automation:
<ol>
	<li>Internet of Things</li>
	<li>Mecha-tronic Things</li>
</ol>
<h3>1. IOT! IOT! IOT!</h3>
Can you hear the crowd of geeks chanting? (In my mind I sometimes imagine a group of geeks cheering a geek supreme leader to the tune of “USA! USA!” that we all find silly [just me?] but hear all the time.)

This is what the internet is going head over heels about. The Internet of Things (IoT) is a geek’s wet dream come true, because it opens up a completely different realm of connected electronics.

At the current point in its nascent history, IoT devices are mostly connected to a master control that lives in our pockets: the smartphone. It’s the enabler at this point due to its ubiquity and tremendous computing power.

But IoT is at a really early stage in my opinion. As a result, a whole bunch of things that do not require connectivity are now connected. Worse still, their creators hardly ever admit that they’re making these things <i>just because they can</i>. Many of time, I observe, see connected things as a logical step forward. You be the judge:

<a href="https://www.quirky.com/invent/243958" target="_blank">Eggminder</a>. Egg tray + reminder. Sent to your smartphone.

[caption id="attachment_47" align="aligncenter" width="664"]<img class="wp-image-47 size-full" src="http://www.nickang.com/wp-content/uploads/2016/02/eggminderstupidiot.jpg" alt="eggminder" width="664" height="427" /> "Eggminder" smart eggtray that reminds you when you're low on... eggs[/caption]

Then, the <a href="https://www.hapi.com/product/hapifork" target="_blank">HAPIfork</a>. Don’t eat too fast or you’ll… get fat. But please don’t worry, we’ll take care of that for you with a smart fork and an app to track your every mouth.

[caption id="attachment_48" align="aligncenter" width="840"]<img class="wp-image-48 size-large" src="http://www.nickang.com/wp-content/uploads/2016/02/1_hapiforkstupidiot-1024x400.png" alt="HAPIfork" width="840" height="328" /> "HAPIfork", a smart fork that teaches you the pace to eat[/caption]

Of course, to be sure, I picked the most horrible of the lot. The senseless use of technology in making products that <em>nobody</em> <i>ever</i> said they wished existed.

I don’t doubt the potential of IoT. For now, for me, we’re just playing around. If you think about the Nest smart thermostat, which is just about the biggest IoT device (and the closest thing to actually being “smart”), it’s really not <i>that</i> game-changing.

Besides connecting everything together and slapping “smart” labels on everything, home automation is also possible without internet connectivity. How did self-stop kettles work before people started embedding internet chips into them?
<h3>2. Mechanical Electronic (Mecha-tronic) Things</h3>
My kettle has an electrical switch…

<i>Whoa, you have an IoT kettle?!</i>

Nope, just a regular electric kettle. You know, the kind you can find in pretty much every hotel room in the world? Remember those?

Ok, enough jeering. IoT has its place in our lives, and increasingly so. But it has a long way to go before the technology frameworks and protocols mature, and before the user interface for making these devices melt into the background and enable an average person to understand and use IoT stuff intuitively.

In other words when it comes to IoT, we’re still years away from the level of acceptance and intuition we’ve developed for multi-touchscreens (yes, we used to call the first iPhone’s screen a true multi-touch screen, remember?).

Back to my electric kettle. It’s a simple device that (god forbids) involves me putting water into it, plugging it into the electrical socket, and pressing a ‘boil' on-off button. It’s a simple device with a huge benefit: I don’t have to manually turn it off when it boils.

That, to me, is the most crucial part of the whole water-boiling process. I don’t want hot water spilling all over my kitchen counter top, overflowing onto the floor and accidentally scalding my feet (or my little Brownie), or short an electrical socket and cause a fire.

I can handle the rest with my limbs and a minute of time.

An electric kettle works because of a few simple but key components:
<ul>
	<li>On/off switch</li>
	<li>Heating element</li>
	<li>Bi-metallic strip (two pieces of metals with different thermal expansion coefficients bound together)</li>
</ul>
Generally speaking this is how an electric kettle works:
<ol>
	<li>User pushes on/off switch to ‘on’ position</li>
	<li>Switch closes circuit, and heating element heats up</li>
	<li>Water starts to boil, and converts to steam (100 degree celsius water)</li>
	<li>Enough steam transfers heat to the bi-metallic strip that it expands, and because of different thermal expansion of the two metals, bends until just enough to mechanically push the on/off switch to ‘off’ position (from inside, ie. not visible to the user)</li>
</ol>
That’s it. Very simple, right?

Mecha-tronic devices occupy a lower position in the technology-sophistication scale, but they can be tremendously helpful to us in our daily struggles in life.

Washing machines take 95 percent of the effort off laundry, electric thermoflasks virtually eliminates the need to re-boil a pot of water for tea and, most recently, with electronic door locks, getting in and out of the home is at least 5 times faster and arguably more secure.

What’s important to realise here is the fact that none of these devices require the internet to work. They are made with mechanical parts and electronic components. And even though that may still be daunting, learning mecha-tronics has become a lot more accessible with the advent of cheap computer platforms like the open-source <a href="http://arduino.cc" target="_blank">Arduino</a>.

I’m an environmental scientist by training. That’s as different from mechanical and electrical engineering as it gets. But the Arduino platform has given me a chance to play around with electronics (and through motors and servos, mecha-tronics) and make interesting stuff.

A recent project was a small LED light that turns on automatically when I switch off my bedroom lights, which I wanted badly because it eliminates the chance of me stumbling over stuff on the floor (including my toy poodle, Brownie) when walking from the main light switch to my bed by illuminating the way.

[caption id="attachment_49" align="aligncenter" width="840"]<img class="wp-image-49 size-large" src="http://www.nickang.com/wp-content/uploads/2016/02/arduinolowlightproject-1024x579.jpg" alt="nick arduino light project" width="840" height="475" /> My auto-on LED light project activates for 2 mins when my bedroom is dark[/caption]

I’ve got many more (logical) projects I’d like to work on to make life a little easier at home, and have already begun working on a few.

In fact, I’m thinking this might be useful to a number of people and am toying with the idea of compiling my projects in an easy to understand compendium. (If this sounds interesting to you, let me know in the comments.)

In any case, I hope more people (you) will take to learning skills that can be used to make life a little easier for yourself, and in the process, begin to see the till-then invisible middleworld of bytes and atoms.

This is part of a bigger movement, called <em>hacking</em>, and it's one that comprises more and more of electronics as we once saw it did with software. I'm feeling it. Are you?
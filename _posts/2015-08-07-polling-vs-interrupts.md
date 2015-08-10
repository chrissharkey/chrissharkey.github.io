---
layout: post
title:  "Polling vs interrupts: programmer elitism in startups and what really matters"
date: 2015-07-08 15:50:00
categories: startups programming product
author_name : Chris Sharkey
author_url : /author/chris
author_avatar: chrissharkey
show_avatar : true
read_time : 6
feature_image: feature-fire
show_related_posts: true
square_related: recommend-fire
comments: true
---

When I first started learning to program, I would use long family car trips to draw designs for computer programs. I designed a game which was meant to be like an Olympic running race: a crowd of circular people, overlooking parallel lines and two racers, also represented by circles, which would move along the track when the player alternated between pressing the 'Q' and 'P' keys on the keyboard.

I ended up making this game, and it was terrible. I didn't properly understand how to read the input values of two  simultaneous keypresses or the difference between detecting when a key is down, or when a key has been pressed and then released. Plus it looked horrible. 

I designed several successful programs too. Successful in the sense that they did what I designed them to do. They included: *Profile* - a simple database in which my Dad could store notes for his school reports, *Mr. Man* - A tile-based, side-scrolling platformer which had a longer introduction sequence than the actual game, and *Mochat* - a chat program designed to allow people to chat live over a serial or modem connection.

I wrote *Mochat* in Qbasic, like all my early work (I like how I say early work like there was a chance that Zynga would acquire *Mr. Man* or something). *Mochat* let let you connect two computers via serial link and type text on one screen which would appear on the other person's screen, and visa versa. It had unique features such as "Instant Insults" and "Instant Compliments", where you pressed a button and it would taunt or be nice to the other chatter. It worked over modem too, which was particularly exciting to test with friends.

At the time, I had been wanting to learn another programming languages and by reading every tutorial available on local BBS servers, I settled on the hardest of the lot, Assembly Language.

Cobbling together the Assembly Language examples I could find, I started working on *Mochat 2*. I got to a point, but then I needed help. I couldn’t figure out how to read in or write data to the serial connection. So I consulted my friends on "Teen Programmers Unite", a website and IRC channel that I used in the two hours of internet access I had per day from my mother's university account. 

A guy on there told me that I had two options: polling, or interrupts. He sent me code examples of both, and I implemented the polling version because it was shorter and easier to understand. He had told me that the interrupt method was "better", but I had no idea why. It seemed like it was doing a lot of unnecessary work to me, when the shorter polling version accomplished just what I wanted so I went with that.

What I should say now is that polling *is* worse than interrupts. Polling means that you're saying to the computer "is there data? Is there data? Is there data? Is there data?" and then when there is, you do something with it, and go back to saying "is there data? Is there data? Is there data? Is there data?". The problem with this is that you're chewing up CPU resources by running a bunch of instructions when there is no data at all. Interrupts avoid this by interrupting your program to let you know that new data is available, so that you don't do unnecessary work.

The purpose of Mochat 2 was to create a chat program in Assembly Language. The polling version worked. The computer was only being used for running that program. Would implementing the program with interrupts have made any difference to the efficacy of the program for the purpose I was creating it? I don't think so.

Since becoming a professional programmer and now a startup CTO, I see the polling vs. interrupts situation come up all the time. Someone will create a web app for their startup and then they will be critisized because it wasn't the best way to do it. Usually it is to do with technology choices:

You made the first version of your web app in Ruby on Rails? "Ruby is too slow."
You used MySQL? "Postgres is much better."
You're running on cloud computing? "Bare metal is the only way."
jQuery? "LOL. There's a whole website for why using jQuery is bad."

I think this kind of programmer elitism in the startup world is counter-productive and people shouldn't listen to it. I made Stayz in PHP and copped an endless barrage of criticism from people online, or in person when I met other programmers. "PHP is too easy". "PHP doesn't have consistency with order of arguments in functions". "PHP is slow".

But Stayz recently resold for $220m. They still run code that I wrote in PHP 14 years ago. Some of it was changed and improved, I did some of that myself over the 5 years we ran the company. But the point is that  the critisism I took was for naught: the purpose of the code I wrote was to help holiday property owners, and it has managed to do that for a decade and a half.

Facebook even used and uses PHP. When the time came where PHP was beyond their needs, they modified PHP and kept on going. Reddit started out using Lisp, when it got popular they rewrote it in Python. Getting things "correct" in the programmer elite sense is not always helpful in the startup world. A mantra I learned in my Teen Programmers Unite days was this: "first make it work, then make it beautiful". Sure, you should aim to use the best available tools and the best paradigms within those tools, but not at the expense of achieving your core purpose.

A favourite saying of mine is "good problems to have". If you write a system which is popular enough where programming or database efficiency becomes an issue, that is a good problem to have. Deal with it when it comes up and not before. Don't spend your time over-engineering a system that might need to be thrown out or drastically changed as you work towards product/market fit.

As your customer base grows and the prospects of your startup being a success increase, the vast importance of doing things efficiency and correctly starts to matter. The efficiency of your system matters most when you're doing well. While you're still finding your feet and exploring the market, it doesn't. While it doesn't matter, focus on working on the things that will make it so. Until then, ignore the programmer elitists, do what works, and just use polling.

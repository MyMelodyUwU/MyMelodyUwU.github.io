---
layout: post
title:  "Refactoring is fun!" 
date:   2022-12-7 12:17:27 +1100
categories: jekyll update
---


## My main goal was to:

1) two python source files. Usage monitor

2) Usage aggreator Commandline argument generator [Done]

3) Capture -> sample rate publish to MQTT [Done]

4) Aggregator, hold in memory. Web server. is the code high enough quality? 

5) Logging. See whats going on. 

6) Creater unit tests

9) Create README.md [Yes!]

10) TMUX 

## Today I learnt:

Debugging was a pain, since I did not know what my issue mainly was, I could see that my own outputs were not being placed as intended. I've learnt that with cleaner code and refactoring that I could find issues faster. I have been writing a lot of functions that were "Dead" and interfered with other components. DRY is quite important because it shows which part are genuine issues. 

## My issue:

Using click is very annoying. When i provide my final input into the program, it interprets the inputs and doesn't publish it! This will need looking at tommorrow by Andy!

![](https://i.imgur.com/is8Ol4b.png)

I also had my on_message function not working for half of the day, so messages did not come through to my aggregator, so I had to revert to an older model! 

## Writing Docs:

This is my first README file!

![](https://i.imgur.com/ade627U.png)


## Refactoring saves lives!!!

I managed to move on from my debugging issues throughout the day after i well refactored the code to suit what I actually needed. 

![](https://i.imgur.com/JDcOuea.png)


## Concepts: 

1) Learning to call a usage monitor in my program [Done]

2) Learning to call 2 aggregators with my program [Still need to master]

![](https://i.imgur.com/jyWpb4O.png)


3) Learning to have 2 Monitors in my program [Yep!]

3) AI and ML Video on Mastering Chess 

https://www.youtube.com/watch?v=0g9SlVdv1PY

4) Learnign to use CLICK for arguments in my program [Major issue]

5) have 1 function for 1 idea. and have 1 script for 1 concept [Refactored]

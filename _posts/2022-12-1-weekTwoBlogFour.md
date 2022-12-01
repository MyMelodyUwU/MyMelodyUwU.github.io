---
layout: post
title:  "Threads, Queues and Publishing!"
date:   2022-12-1 12:17:27 +1100
categories: jekyll update
---

## Refactoring

Adjustment of the code one by one to perfect the code / make more efficent / readable to avoid a big mess. Overtime, I think I have gotten better at this now that I am developing everyday. 

## Technical Debt

To prevent a big unga bunga later on, I should start taking solutions that can help me long term. 

![](https://i.imgur.com/AyhU9bF.png)

## Working on my project

Today I learnt about Locks and Queues on my threads so information cannot be overwritten by accident, and calculations are made correctly. This is called Concurrency. 

For my project, I created a Thread Lock on the the GET Request of the web server to obtain the information. 

## The Bank Account problem and the two solutions

There are two solutions Lock and Queue. Lock is generally frowned upon and only should be used when efficent and Queue is used mainly. 

Lock is advantages because its easy to implement. 

Queue is more memory efficent and easy to follow. 

Queue: Basically outsourcing the two threads (Credit and Debit) to an external thread which will set in order the threads. 

## Publishing to multiple topics:

![](https://i.imgur.com/UeTHqyv.png)

I managed to publish to multiple topics today, I altered the JSON file and created a loop to go through and individually post the temperature to a location. 

![](https://i.imgur.com/IvO4Rd2.png)

![](https://i.imgur.com/59EBPHC.png)

## The Database: 

I managed to refactor my code to have the SQL in 1 section. 

I attempted to insert the temepratures found into the databse, but there is always an error with appending to it. I assume I have initalised it incorrectly, but, I cannot tell/find where the issue is. 


## Some Ideas for Tommorrow:

1) Having a thread lock to only 1 location. 

2) I.e. I can ping for Sydney and Melbourne @ the same time. 
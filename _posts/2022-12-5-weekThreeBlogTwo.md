---
layout: post
title:  "Testing Driven Design + learning to play with inputs / outputs + finding relationships"
date:   2022-12-6 12:17:27 +1100
categories: jekyll update
---

## My main goal was to:

1) Json Output (Publish) [Yay]

2) Use click for inputs to encode my broker, topics and hosts to provide better order and searching with wildcards [Almost there but its terrible right now]

3) Create a queue for the webserver. 

4) Find meaningful relationships in my code to create a DB. 

5) Create a database to store the JSON inputs. 

6) Work fast. 

## Learning about JSON Dumps (The most successful part of today)

JSON dumps are really convinient and useful because it brings JSON strings across MQTT and can be read in a really nice way. This will ensure that factors like a dictionary can be well read. 

In my project today, I managed to create a JSON Dump to be published and decoded across the MQTT servers successfully after some tries. A noteable issue was mainly the data types, which I have managed to fix up. I aim for this JSON to be written to a database instead of appended to a CLI interface.   

![](https://i.imgur.com/q9LdBcp.png)


## The not so good stuff: I'm writing a lot of dead code. 

I realised that integrating the Python Module Click is hard since it does conflict with the JSON inputs that I have already. I used GPT3 to write a fair amount of code already. It is just the error of the pilot to put it in the publish script. 

This was my attempt of using Click with my program: 

![](https://i.imgur.com/LF5rTyw.png)

## Test Driven Design

1) Writing tests that effectively uses the computer to tell the user what is being built. 

2) Creating code that fits the test (Expectation vs reality)

3) Documentation or note of all errors to find best otucome. 

Here is a video on it: 

https://www.youtube.com/watch?v=B1j6k2j2eJg
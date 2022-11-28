---
layout: post
title:  "Clown Fiestas, Utter Confusion"
date:   2022-11-28 12:17:27 +1100
categories: jekyll update
---

## Design skills

There are 4 Stages in our mini software development cycle 

1) Requirements

2) Drawings/Diagram of Proposed material

3) Google Doc of all components

4) README

## Aim

Todays journal describes design skills that is relevant to our project, which is creating an online weather checker. Information will be passed through MQTT and printed on a webserver. Later on, there will be further analytics up. 

## In my meeting with Andy:

We followed the Diagram of the proposed application. We created a high level component flow of the program. 

![](https://i.imgur.com/QetUy71.png)

## What are Topic Wildcards, Why are they Useful?

Topic Wildcards shows generalisation of threads to show relevant data to the thread, like Reddit. 

A good example of a set of threads that is lined out by Wildcards can be seen [here](https://github.com/mqtt/mqtt.org/wiki/SYS-Topics)

## Find material on Last Will & Testament?

[Here](https://aws.amazon.com/blogs/iot/monitor-aws-iot-connections-in-near-real-time-using-mqtt-lwt/)

## What happened today:

1) I tried linking the MQTT connection to the flask web server. Failed Drastically. 

2) I managed to understand that the publish MQTT component must not run with the web server as this is going to be changed out. If the webserver also is in charge of publishing, the application will stall. 

3) I wanted to try using a last will timer on the publishing server to do only 30s worth of publishing. But it was not ideal within the scope of the program. This was also not feasible witht he way the 

## How did I manage to maintain good programming practices when writing (When it was quite hard)?

1) I clearly wrote what was going on. I made sure that the code is in adequate order

2) I marked all the imported functions provided. 

3) I looked @ the explanations of code that I did not use. 

## Where is the clown fiesta that I did today?

[Here](https://github.com/MyMelodyUwU/weather_server.git)

![](https://i.imgur.com/qcPORaU.png)









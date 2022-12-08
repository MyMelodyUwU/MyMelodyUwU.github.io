---
layout: post
title:  "Almost Finished my first card!" 
date:   2022-12-8 12:17:27 +1100
categories: jekyll update
---


## My main goal was to:

1) two python source files. Usage monitor [Done]

2) Usage aggreator Commandline argument generator [Done]

3) Capture -> sample rate publish to MQTT [Done]

4) Aggregator, hold in memory. Web server. is the code high enough quality? [Done]

5) Logging. See whats going on. [Done]

6) Creater unit tests  [Sort of Know/Dunno What to put in]

9) Create README.md [Yes!]

10) Learn TMUX 

11) Needing to fix Click [Problem] 

## Tmux: 

1) Creating a session: `Tmux new -s <session name> 
2) Closing a session: `CTRL + b, then :, then type exit`

## Logging Module with Python

The Python logging module is a built-in library that provides flexible logging capabilities for Python programs. It allows you to create loggers that emit messages with different levels of severity (such as DEBUG, INFO, WARNING, ERROR, etc.), and to specify where these messages should be sent (e.g. to the console, to a file, or to a remote logging server).

## My project today:

My First card is almost done! It is just missing the click module! This will be reviewed by Andy. 

My big sucess today is writing the dictionary with the HTML content neatly! This will help me long term when I move onto my next card, the SQLITE3 database!

I also managed to boot up a VM on my other machine and have TWO monitors and TWO aggregators on the MQTT topic / thread to be have the intended output!

![](https://i.imgur.com/m2MBrUT.png)

^ Aggregator on my Laptop

![](https://i.imgur.com/tZOwPLg.png)

^ Aggregator on my Desktop

I also am able to run multiple hosts with 1 Aggregator which was intended by my design drawing and specifications. 

## Implications from having a stronger understanding:

From understanding my code, I now managed to create a higher level diagram to document the flow of data!

![](https://i.imgur.com/nAx0i9Y.png)



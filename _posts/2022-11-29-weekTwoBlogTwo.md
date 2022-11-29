---
layout: post
title:  "Keeping code clean and consistent when writing!"
date:   2022-11-29 12:17:27 +1100
categories: jekyll update
---

## The progress so far...

Step 1,2,3 has been completed!

I managed to have a mqtt publish server and a mqtt subscribe server whichd isplays the tempereature on the computer console. 

I managed to get the informaiton in 30s and print it out in a list  sing a global variable 

I also managed to create a average function in the list of temperatures to determine the average.

Eror mangement and reversion of BIG mistakes


## The art of programming

1) By minimising literals, it is extremely helpful for me to become more efficent when I code, when I change something, only 1 thing needs to be changed before anything else. 

2) When all my functions are in order, it is easy for me to track issues. 

3) With a main function, it is easy to see the compilation of the scripts!

4) With comments, i started to have neater code and easy to udnerstand code. 

5) Functions are able to be cut and pasted to look concise and efficent!

## Errors I came into:

![](https://i.imgur.com/QIggocm.png)

Data types have become very important. I have noticed that The final output that I produce must be a string or else it would not appened. 

![](https://i.imgur.com/Lbr7ufK.png)

After a lot of debugging and thinking about it, I managed to print on the CLI

![](https://i.imgur.com/1m71oJN.png)

Later, when serving the content, I found it hard to print a list on flask. But that just because I was stupid. 

![](https://i.imgur.com/hEbTFKo.png)

This is the output. 

Finally, When I tried to debug and test my input from a text file, I accidently appended my text onto the script itself. Kaboom!

![](https://i.imgur.com/08bmRnr.png)

![](https://i.imgur.com/OLSWKSn.png)

## Where is the code?

[Here](https://github.com/MyMelodyUwU/weather_server.git)

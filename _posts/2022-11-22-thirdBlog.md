---
layout: post
title:  "Learning the basics of Py and proper development!"
date:   2022-11-24 12:17:27 +1100
categories: jekyll update
---

## What is the objective for today:

The objective is to have a clean running program that is ready to be pushed onto AWS. 

### Learning about File Types

When we use the unix command file, this determines the filetype relative to the computer.

I learnt that a Python script would need the Environment declared before it is deemed as a python file when using the file command. This is because the different permissions are being changed from Writable to Executable. 

Since Python is an *interpreted* language, the python script is being interpreted rather than like in C, where a executable has to be made. 

If I was to use Python on a C script. The Python interpreter would struggle to figure out what is going on. 

### Learning how to use VIM Properly

VIM should be used effectively by minimizing use of visual mode. This would mean starting to cut / jump lines using the distance of the lines rather than guessing. Minimize the use of characters onto the machine.  

This can be achieved by:

1) Using CW (Change word) & using .

2) Using a Number before the command


### What are the aspects of the script

#### The script must have a:

1) Environment / Library File (Stdlib.h or Python Environment File)
2) A Psudocode Goal Using Comments
3) Extra functions/plugins needed
4) Global Variables
5) Main function with all the functions being called **Inside** it. 

#### To make the code look clean:

We need to really see what the code can do now. 

This is by listing all the functions in order. Variables for the program should only be intrinsic towards the function that it is written to

I.e. a READ function should not have any variables that have had operations altered to it. (Max) 

Meaningful Version names / Variable names. **This is written in snake_case**. 

When we write our code neatly, this gives another person more time / easier to debug. Also understands the flow of the variables provided. 


## What Operations did I do:

I created a flask webserver that does 4 operations when inserting elements into the URL.

### Operations:

1) Binary

![](https://i.imgur.com/hI2wBoC.png)

2) Average

![](https://i.imgur.com/M1nFAOj.png)

3) Sum

![](https://i.imgur.com/rAAsEai.png)

4) Random Number generator

![](https://i.imgur.com/cGGgB6B.png)

### GET Request:

I could make a GET Request that could ask for the item without using the URL

![](https://i.imgur.com/LOSSxK7.png)

## Where is the code?

The code is [here](https://github.com/MyMelodyUwU/simpleOperations.git)
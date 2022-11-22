---
layout: post
title:  "Learning the basics of Py and proper development!"
date:   2022-11-22 12:17:27 +1100
categories: jekyll update
---

Started with discussion of security professionals and understanding the philosphies in why I do this work / the meaning of my decisions when doing this stuff.

This helped me in my debugging. 

### What I found: 

https://en.wikipedia.org/wiki/April_Fools%27_Day_Request_for_Comments

http://www.phrack.org/issues/70/15.html#article

I have also noticed my university material is developed versions of Bruce Schnier's book. 


### In my meeting with Andy: 


1) Aims were to learn about how to use unix tools by deviating to more powerful commands

2) With VIM, learning to use it more efficently. Learning to strategise it efficently.

3) Understanding software methdology.

In my own time, I have created a Base 10 to Binary Calculator. 

I aimed to:

1) Read a list of Numbers, 

2) Convert it to binary

3) Console output or output to a file. 

4) Use libraries and other plugins to aid the process

5) Use VIM effectively. 

### Issues I have come across:

1) Using a CSV file managed to create the wrong data type of a list I had made

2) Using recursion meant that I cannot append to a file of the desired values

### Post meeting with Andy, I have been taught:

1) How to create code in an efficent manner, which is by using vim controls to duplicate and using the find and replace methods faster. 

2) using efficent functions rather than having my own fucntions

### Further things I have tried:

1) Parsing in more than 1 argument for ther system to put into binary. It seems like the system only can recognise 1 input at the time | Failed

2) Generating random numbers | Success

From this further exercise. I have noticed that pipes in my system has issues. 

### Blogging

Lastly, I have now put everything in my blog!

Anyway, here is the code since all projects should be open source **insert Stallman noises**

```
# My aim is to:

# Take 2 forms of input
# Cut the console input 
# Perform a binary operation
# Append it to console or output

import sys
import random

#input_file = "/dev/stdin" #Console read
input_file = "z_in" #Input file

#output_file = "/dev/stdout" #Console output
output_file = "z_out" #output file

def read():
    file = open(input_file, "r")
    input = file.read()[:-1]
    return input

def operation(input):
    ans = bin(int(input))
    return ans[2:]

def write(result):
    file = open(output_file, "w")
    file.write(result)

def main():
    arguments = sys.argv[1:]
    argument_count = len(arguments)
    print(f"Command line arguments: {arguments}")
    print(f"Command line argument count: {argument_count}")
    if argument_count > 0:
        print("has command line arguments")
    #input = read()
    input = random.randint(0, 100)
    #print(input)
    #resultList = [] * len(input)
    result = operation(input)
    #resultList[i] = result
    write(result)


if __name__ == "__main__":
    main()
```
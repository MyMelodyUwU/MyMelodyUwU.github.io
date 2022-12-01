---
layout: post
title:  "Using JSON and creating my first database!"
date:   2022-11-30 12:17:27 +1100
categories: jekyll update
---

## Pre programme information:

To find out the filesystems I have:

I can look at the report file system 

![](https://i.imgur.com/7rS3K9T.png)


^Disk space 

![](https://i.imgur.com/mTT1XKN.png)


^ Each disk that has a directory on it. 


## Some philosphies when using Disks

1) Do not fill up root system

2) /home in a file system is where the users can put things on

3) i.e. if andy logs on his $home is /home/andyg

4) Data should be stored in /mnt/data

5) Clean up after yourself. 

6) Directories:

    - Bin (Where commands go)
    - Dev (Where inputs go)
    - Etc (Where admin files go)
    
![](https://i.imgur.com/phmpxBh.png)


## Making a new user: 

User has 3 files that matter

passwrd == username/userid/homedir
shadow == encrypted passwords
groupfile == groupid 


Appending to a /etc/passwd file (For user and the perms) and a /shadow file (For The passwords / ssh keys) a /Group File

![](https://i.imgur.com/aiLMix2.png)

## Working on my project

Today I managed to change the code to remove duplicates!

I also learnt to use JSON to feed my information in to avoid literals and duplicates. 

![](https://i.imgur.com/1kApWP4.png)

I also have managed to set the subscribtion to be only towards 1 location only!

Which in my case, I manged to set all the data to be in Sydney!

Right now, I am trying to get my database to load, which I managed to create the database, which we can see the binary. 

Now i need to learn to print the Data using the SELECT Statements!

![](https://i.imgur.com/bmbsDVT.png)

![](https://i.imgur.com/gMvlKrv.png)


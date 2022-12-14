---
layout: post
title:  "Starting my first TMUX run through!" 
date:   2022-12-7 12:17:27 +1100
categories: jekyll update
---

### Setting up on a machine!

Today I managed to setup my user on a machine that will be hosting my directory and the executed code on a development side. 

### Setting up my own user: 

1) I had to share my SSH key with Andy so I was able to access root of the machine. 
2) I had to append my own user id and put my 3 security permissions in a passwd/shadow/group file. 
3) I then also created my own directory with the .bashrc/SSH Key and appeneded to it. 
4) I then SSH'ed into the machine to see if everything was working just fine.

### Permission in linux files 

```
---     ---     ---
rwx     rwx     rwx
user    group   other
```

These are the big 3 To remember. 

#### Learning to change permissions 

```chmod u=rw,go=r fred.txt```

This command sets the owner's permissions to read and write (u=rw), and sets the group and other user's permissions to read only (go=r).

The first argument you give to the “chmod” command is ‘u’, ‘g’, ‘o’. We use: 
u for user / g for group / o for others, 
you can also use a combination of them (u,g,o). 

#### Learning to do EVERYTHING in that specific directory

The -R or -r flag is a common option for many Linux commands, including chmod, cp, and rm. When used, this flag causes the command to operate recursively, meaning that it applies to the specified file or directory, as well as all of its subdirectories and files.

```chmod -R u=rw,go=r fred```

On the machine, I was able to control the permissions of files on my machine by using the recursive function on the directory of the items I wanted to change. 

### Learning to use TMUX

```tmux new-session -s my-session```

^ Creating a new session 

```tmux attach-session -t my-session ```

^ Attaching a session 

### Composition over time 

Developing by combining and arranging various modular components or modules. This is a common approach to software development that allows for more flexibility and maintainability than trying to build an entire program as a single monolithic block of code.

### Maintaining flexibility when I develop: 

Inheritance is a mechanism by which an object can inherit the properties and methods of another object, allowing developers to create hierarchical relationships between classes of objects. 



### Unix vs Multrics

https://www.youtube.com/watch?v=3Ea3pkTCYx4

The major achievement of Unix is that it is effeicent, with more dymanic code and everythign could be built together like lego bricks, most commands could come together faster like building blocks. 

the famous | (Pipe) was a factor that could be used to increase the efficentcy because it serves as more paramters or combination of results together. 

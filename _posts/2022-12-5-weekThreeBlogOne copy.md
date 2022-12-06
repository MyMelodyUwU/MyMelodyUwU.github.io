---
layout: post
title:  "Data types Argh!!!!"
date:   2022-12-5 12:17:27 +1100
categories: jekyll update
---

## Learning about Click and Decorators!


Click is a Python package for creating beautiful command line interfaces in a composable way with as little code as necessary. It’s the “Command Line Interface Creation Kit”. 

Click would have decorators that will produce inputs that are tedious for us to save time!

```

import click

@click.command()
@click.option('--count', default=1, help='Number of greetings.')
@click.option('--name', prompt='Your name',
              help='The person to greet.')
def hello(count, name):
    """Simple program that greets NAME for a total of COUNT times."""
    for x in range(count):
        click.echo(f"Hello {name}!")

if __name__ == '__main__':
    hello()

```


## Flags and Sub commands:

Flags: Flags are optional parameters that modify the behavior of a command or program. They are usually preceded by a hyphen and often a single letter. For example, the -v flag for the ls command displays the contents of a directory in a verbose format.

Sub Commands: Sub commands are additional commands that modify the behavior of a program or command. They are usually preceded by a hyphen and a short name, such as -help or -h. For example, the ssh command supports sub commands such as -t (for tunneling) and -v (for verbose output).

### Software Spikes

In software development, a spike is a task that is designed to explore a problem or concept and produce a solution quickly. The goal of a spike is to quickly develop a simple prototype, prove a concept, or identify a solution to a problem. Spikes are typically used when there is uncertainty about a feature or how to implement it. They can help reduce the risk of investing too much time in a solution that may not be viable.

## Epics vs Issues: 

What is an epic and what is an issue in software development 


An epic is a large piece of work that is broken down into multiple smaller stories or tasks. Epics represent the highest level of scope in a project. In software development, an epic is a user story that encompasses a large chunk of the project. It typically covers several stories or tasks and is used to help break down a large project into more manageable pieces.

An issue in software development is a problem or bug that needs to be fixed. Issues can range from minor bugs to major system problems. Issues can be found during testing, development, or after the product has been released. Issues can be caused by a variety of factors, including coding errors, system architecture, or user errors.



### Pipelines 

Pipelines in Python are a sequence of steps or processes that take input data, process it and then return the output. They are commonly used in data engineering, machine learning and data science to streamline the data processing and analysis process. Pipelines are typically used to create a single workflow to transform raw data into some meaningful output, such as a model, report, or visualization.

## Explaning my problems. 

Don't use it as a word, because it creates lots of headaches. QED. 

## My project and data types ARGH!!!!

Data types have been quite annoying in this project, this is becasue the output of the CPU information is it own data type (PSUTIL). MQTT had only a few data types of information that is allowed to be transferred over. This is a restriction of the information that I can transfer across using MQTT. 

![](https://i.imgur.com/tUqBUrn.png)

MQTT will only take a string, bytearray, int, float or none as a data type. 

## My project and VM CPU processing

My goal for today was to take real time CPU Usage percentages and post it on my MQTT Topic for my web application to recieve. 

**Problem:** The CPU is taking in the correct CPU Usage percentages, but the problem is the CPU isn't pumping that much, since I am using a VM. So the alterantive solution is the FLOOD the CPU using a stress application to ensure the CPU is Pumping. I used an ongoing linux application called Stress. 

![](https://i.imgur.com/GPc7dZr.png)

![](https://i.imgur.com/JCixsQ7.png)

![](https://i.imgur.com/xY9AuYz.png)


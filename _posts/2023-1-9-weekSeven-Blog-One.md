---
layout: post
title:  "Last formal internship week!" 
date:   2023-1-16 12:17:27 +1100
categories: jekyll update
---

## Mailchimp Exposure of data 

1) Factors such as RBAC could have drastically reduced impact of the risk. 
2) Employees fell for a phishing attack. 
3) Security teams were able to protect a portion of their own data. 
4) Rule of Least priviledge -> Reducing attack surface
5) When Permissions are not given when provided, could end up putting data records at risk 
6) If roles are changed, there should be constant security followup on that. 

## A big achievement by myself:

Getting the timestamp and the hosts to append to the database 

![](https://i.imgur.com/ficmgsz.png)

Having multiple hosts!

![](https://i.imgur.com/VAiG6Eo.png)

Keeping the data overnight!

![](https://i.imgur.com/ymzyXpe.png)

printing the data to a web output

![](https://i.imgur.com/eGval1n.png)

Printing SQL statements nicely!

![](https://i.imgur.com/aPdoTtX.png)

![](https://i.imgur.com/X2N6UKd.png)

**I am totally doing my work**

## What is engineering

Performance in our capability. 

## Project

On the same topic, resource / hostname / cpu

Usage message + retained info type. 

How does the aggregator know which type of emessage this is. 

USage message vs info message

write to database, but written to one table, the other written o a different table. 

If the message changes, its indirect. 

ensure no mistakes (type) | value is info or usage. 

timestamp, s in epoch

field -> host

usage -> Busy

type -> Int or string (Info vs usage.)

## The next day:

![](https://i.imgur.com/wwKyXNA.png)

900KB of data here from last night! Ares has been working overnight to give me the cpu_usage of the system!

## The goal: 

The goal now is to have:

1 Monitor over the weekend taking cpu_usage data!

3 Aggregators -> Ares / Zeus / Arty

Set Gitignore on database files

Adjusting the data collection speed from 2s to 15 s 

## Whats wrong with the data:

https://www.howtogeek.com/194642/understanding-the-load-average-on-linux-and-other-unix-like-systems/

In computing, a runtime average is a measure of the performance of a program or algorithm over multiple runs or iterations. It is typically calculated by dividing the total runtime of the program by the number of iterations. This provides an overall measure of how long the program takes to execute on average for a given input size or dataset.

It's common to use runtime averages in performance analysis and optimization of software. It is also used to compare the performance of different algorithms or implementations of the same algorithm. With runtime averages, developers can determine which approach is more performant, and make decisions on which one to use based on the results.

It's worth noting that runtime averages can be affected by many factors such as the input size and data distribution, the number of runs, the specific machine and environment where the program is running, etc. So it's important to use them with care and make sure to consider these factors when interpreting the results.

## Data rolling up:

In computing, "rolling up" data typically refers to the process of aggregating data from multiple records or rows in a database into a single record or row. The process is also called "data rollup" or "data aggregation"

For example, in a database table that contains sales data, rolling up the data would involve summing up the total sales for each product across all the records, and then returning a single record for each product that contains the total sales. This process can be done across multiple levels of granularity depending on the data, for example, rolling up sales data by product, then by category, then by region, etc.

Rolling up data is often used in data analysis, reporting, and visualization, to provide summary information and insights that are easier to understand and act upon.


## Final walkthrough!

I managed to get a run through with the CEO of Silverpond to discuss about the 

![](https://i.imgur.com/1Id6FTE.png)

This is the current tentative webserver with data collected overnight!

This data has now been stored in a master copy on the repository!

![](https://i.imgur.com/R1LXXqB.png)

spent the whole day on data structure and learning how to save data into a csv

![](https://i.imgur.com/TD1Nv1n.png)

i also managed to plot my data, which tmr i will  refactor it!
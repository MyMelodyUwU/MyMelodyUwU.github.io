---
layout: post
title:  "The art of programming"
date:   2022-11-25 12:17:27 +1100
categories: jekyll update
---

## Goal for today

To understand the art of programming and to make more efficent my development skills. This included going through the current simple operations project and making it more readable and flexible so it can be used. 

## First meeting -> Understanding Git lab fundermentals

Git lab is used post deployment to help integrate merge requests onto systems on the instances. 

After code has been pushed, Gitlab would be used to do CI Tests on the code to ensure models are learning, etc. 

Increase of test cases before code is pushed for deployment

## Learning about octals

Octals work in 3. Which there are 3 numbers that abbreviate it. The 3 digits consist of Owner, Group and User. 

## Use of a lookup table / Dictioanry 

A lookup table on our operations script became fundermental because it makes code more accessible.

![](https://i.imgur.com/UVmzJbr.png)

Because of our clean code, we could make our calling functions in the Flask Web App server more dynamic.

![](https://i.imgur.com/23McYOp.png)

^ Here 

## Learning MQTT basics

In MQTT, I learnt to create a thread and publish numbers. 

I could take the numbers from a Subbed machine and process it into binary. 

![](https://i.imgur.com/oIpe456.png)

From the subbed machine, I managed to make a process to put it in binary and print it here:

![](https://i.imgur.com/C8Emtit.png)

## Next week I aim to:

1) Start my internship properly
2) Learning to host my Flask website onto a cloud instance
3) Learning to use docker
4) Learning to optimise my code so it can be used on a cloud instance
5) Sleep


## Where is the code?

The code for simple operations is [here](https://github.com/MyMelodyUwU/simpleOperations.git)

The code for the MQTT is here:

```py
#!/usr/bin/env python3

import paho.mqtt.client as mqtt 
from random import randrange, uniform
import time
import random

mqttBroker ="mqtt.eclipseprojects.io" 

client = mqtt.Client("KFC")
client.connect(mqttBroker) 

while True:
    client.publish("KFC",random.randint(0,100))
    time.sleep(1)
```

```py
#!usr/bin/env python3

import paho.mqtt.client as mqtt
import time
import operation

def on_message(client, userdata, message):
    #print("received message: " ,str(message.payload.decode("utf-8")))
    output = operation.operation_binary(str(message.payload.decode("utf-8")))
    print(output)

mqttBroker ="mqtt.eclipseprojects.io"

client = mqtt.Client("Smartphone")
client.connect(mqttBroker) 

client.loop_start()

client.subscribe("KFC")
client.on_message=on_message 

time.sleep(30)
client.loop_stop()
```

```py
#!/usr/bin/env python3

import sys
import random

def operation_binary(values):
    return bin(int(values))[2:]
```


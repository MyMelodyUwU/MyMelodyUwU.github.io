---
layout: post
title:  "Last Blog of 2022!" 
date:   2022-12-15 12:17:27 +1100
categories: jekyll update
---


## little and big Endians 

In computer science, "little endian" and "big endian" refer to the order in which bytes are stored in a multi-byte value.

In a little-endian system, the least significant byte (LSB) is stored at the lowest memory address and the most significant byte (MSB) is stored at the highest memory address. This means that if you read the memory addresses in order, you will read the value from least significant to most significant.

In a big-endian system, the opposite is true: the MSB is stored at the lowest memory address and the LSB is stored at the highest memory address. This means that if you read the memory addresses in order, you will read the value from most significant to least significant.

Endianness is important when working with multi-byte values because it determines the order in which the bytes are stored and retrieved. For example, if you have a 32-bit integer with the value 0x12345678 and you are using a little-endian system, the four bytes of the integer will be stored in memory as: 78 56 34 12. If you are using a big-endian system, the bytes will be stored as: 12 34 56 78.

The choice of endianness can have an impact on the performance of certain operations, such as data transmission over a network or reading and writing data from external storage. It is important to ensure that systems that need to communicate with each other are using the same endianness, as data may be misinterpreted if the systems have different endianness and do not properly convert the data.

## A matter of perspective 

![](https://i.imgur.com/HUp5LkW.png)

## 21/12/22

*Start 9am* 

*End 5 30pm*

## 22/12/22

*Start 9 30 am*

*Finish 4 30 pm*

### Learning further vim keybindings:

1) Mark (m) binding to alphabet to create shortcut

2) ctl e is to scroll whilst leaving in the cursor 

3) ' is Tick

4) ct (change to) 

5) What we are doing now is creating a reset function in the aggregator

### Moving code towards data | philosphy

Reduced latency: By placing the code and data on the same server, there is no need to transmit the data over a network, which can reduce the time it takes to process the data.

Improved performance: When the code and data are co-located, the data can be accessed more quickly and efficiently, which can improve the overall performance of the application.

On the other hand, if we move the data closer to the code, it means storing the data on a server or device that is separate from the server or device where the code is running. This can have the opposite effects of the ones listed above: increased latency, decreased performance, decreased security and increased complexity.

### Click Groups

Click groups are a way to group related commands together in a CLI. For example, you might have a group of commands related to managing users, and another group of commands related to managing resources. Each group can have its own set of subcommands and options!

### Python DocString

In Python, a docstring is a string literal that appears as the first statement in a module, function, class, or method definition. Docstrings are used to document the purpose and behavior of Python code, and they are accessible at runtime.

### Command line job control

![](https://i.imgur.com/hvkEBgk.png)
^ If config

![](https://i.imgur.com/QCZSNtZ.png)
^ mangeing the jobs and using shortcuts

### A bash script to remove all retained messages on MQTT 

```
def reset_MQTT_retained():
    print("checking if the remove script exists")
    if os.path.exists("remove_retained_mqtt_msgs.sh"):
        print("The file exists.")
        subprocess.run("remove_retained_mqtt_msgs.sh localhost")
    else:
        print("The file does not exist.")
```

FileNotFoundError: [Errno 2] No such file or directory: 'remove_retained_mqtt_msgs.sh localhost'


![](https://i.imgur.com/K95r1Rl.png)

^ problem solved, used another imported module to fix it 

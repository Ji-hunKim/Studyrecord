# 1. System Design for Beginners

## 1. Computer Architecture

### Disk
We will be going over the main components of a computer from the software perspective and how they work together to execute the code we write. 

Let's first start with our disk. At least that's one way to refer to it. You could also refer to it as the storage or maybe the harddrive (HDD - hard disk drive). This is going to store all of our data and it's gonna do so persistently. 

What that means is that even if our computer restart or our computer crashes while we're executing some codes or while it's running some programs, the stuff that we store inside of our disk is going to be persistent.

Now how much information can it store? Well it's usually measured in terms of 100GB or more commonly in terms of TB. 

> Remeber a byte is nothing more than eight bits. And each bit can either store 0 or 1. And we can use this bits and bytes to represent information.

### RAM
Now we also have our memory aka our RAM(Random Access Memory). And this is also used for storing information. Though it's typically a lot smaller than disk. That's because RAM is typically more expensive in terms of money. But the benefit is that it's a lot cheaper and in antoher way in terms of resources. If we're going to be writing data to our RAM, the amount of time it will take would be measured in terms of micro seconds. So in general reading and writing from RAM is measured in terms of microseconds. Reading and writing from RAM is a lot faster than reading and writing from disk. 

So while we can't store as much as information in RAM as we can in disk beacuse it's generally the case, the benefit is that RAM is a lot faster than Disk. 

Now how excactly do we write data to our disc or to our ram and how we read or retrieve data to our ram or from our disc? What if we even want to communicate between the ram and the disc? These components can't directly talk with each other. That's why we need CPU.

### CPU
CPU(Central Processing Unit) It's essentially the brain of the computer. What it's capable of doing is quite complicatecd. The main things that the CPU is capable of is writing information to RAM or Disc. And when we talked about the time that it takes to write from RAM and to write to Disc, this is what we met how much time it takes the CPU to perform this operation. The CPU is going to execute the codes, and the codes we wrote is written somewhere in memory. It's gonna be compiled down into instruction that the CPU can actually interpret. So CPU is going to be reading our code so that execute that code but it's also gonna be reading or writing from RAM for a different reason. There's a Data store in RAM. The variables we declare will be stored in the Data portion of RAM. (The codes are in code portion) So CPU is not only reading codes but also could be writing data. 

### Cache
What if we want it to be faster? CPUs have another component called 'cache'. It's smaller than Disk and RAM. It belongs to the CPU itself. And it's used to speed up read and write operation from RAM. Reading and Writing from cache is ns (ms from RAM). And the cache is mainly used as a sustitution for the RAM. What the CPU will do is it'll take a subset of the RAM some portion of RAM - that can fit in our cache. So the CPU will choose the certain portion of the RAM that we're writing or reading frequently. Even the small cache will improve the performance of the entire system. It can first check if that data is in our cache, if the data is not there then we can perform more expensive action which is actually reading from RAM. 

The downside of RAM and cache is that they are not persistent data. That means if we throw information in our cache or in our RAM, and maybe our coomputer crashes or we restart it, we are not guaranteed that the same information that we stored there is going to be persistent. 

How fast we execute our code is limited by our CPU. 

Moore's Law (intel co-founder)
Over time, the number of transistors inside of a CPU double every two years. And the cost cut in half in two years. But in reality we've seen that CPU speed is acutally beginning to plateau. Roughly in last 10 years the speed has slowed down. So we can't infinitely scale single CPU. 
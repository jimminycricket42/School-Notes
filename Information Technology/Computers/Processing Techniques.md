---
aliases: [Multitasking, multi-threading ]
tags: [GR11/Q1 computers/software ]
created: Mon 13/03 2023
---
# Processing Techniques
Software and hardware use many processing techniques to improve efficiency of the system. Common techniques are multitasking and multithreading. ^blurb

> [!note]+ :spiral_notepad: Multitasking VS. Multithreading
> Multitasking is many processes occuring on one chip, while multithreading is multiple CPU cores performing many processes at once

## Multitasking
Multitasking is used by the [[operating system]] to run multiple apps at once (despite the processor only running one process at once). This uses [[System Interrupts]] to pause tasks and resume them later. Multiple processes are stored in [[RAM]], and short burst of processing time is allotted to each. 

This requires the operating system to properly allocate CPU time to each process without leaving any suspended for too long. 

![[Pasted image 20230313092922.png]]

To give the appearance of many things happening at once, the operating system must switch processes many times each second. This is possible due to each process being stored in RAM or registers in the CPU. Each program is allotted a certain amount of CPU execution cycles, after which the CPU makes a copy of each register and notes where the process ended execution. It then loads all the registers used by the second process and allows it a number of CPU cycles before copying the registers of the second program and beginning the first one again. 

## Multi-threading
One program can have many different parts of a program running independently. This is known as multi-threading. Multi-threading must be programmed into a program to ensure that threads do not interfere with each other. 
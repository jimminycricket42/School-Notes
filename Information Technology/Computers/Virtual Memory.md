---
aliases: [ ]
tags: [GR11/Q1 computers/software ]
created: Mon 13/03 2023
---
# Virtual Memory
Virtual memory is the operating system making use of an area in [[Secondary Storage]] when the [[RAM]] is full. It extends the amount of memory addresses contained in RAM, and when information in virtual memory is called upon the RAM *pages* the secondary storage for the data it needs. Once located, the data in virtual memory swaps for data in RAM. ^blurb

Virtual memory can be seen as the opposite of [[Cache and Latency|cache]], as cache uses faster storage to accommodate for slow storage, and virtual memory uses slower memory to accommodate for not enough fast memory. 

Many graphical applications use virtual memory, as graphics files are large and often cannot all be loaded into RAM. 
---
aliases: [ random access memory, primary memory, volatile memory]
tags: [GR11/Q1 computers/hardware ]
created: Sun 12/02 2023
---
# RAM (Random Access Memory)
Ram is the main memory of a computer. It exists as modules attached to the motherboard. RAM stores *the programs and data currently in use*. RAM is volatile memory, meaning it will be lost when it loses power. ^blurb

Different types of RAM have a large impact on the system. Data must constantly be moved between caches and RAM by the system’s memory busses. If the RAM is too slow to read/write that data, then the whole system throttles. 
## Common type of RAM: DDR SDRAM
DDR SDRAM most commonly used in modern computers. 
- DDR is ‘Double Data Rate’, meaning that data is  transferred twice per [[CPU|CPU clock pulse]]. 
- The ‘S’ in SDRAM stands for Synchronous, meaning that the refresh of the RAM is synchronised to the CPU so that the CPU doesn’t have to wait for instructions. This increases the rate that instructions are fed to the CPU, reducing the wait. 
- The ‘D’ in SDRAM stands for dynamic, meaning that the type of chip used is a dynamic (therefore constantly updating) chip


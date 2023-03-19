---
aliases: [ ]
tags: [GR11/Q1 computers/software code/theory ]
created: Mon 13/03 2023
---
# High-level Languages
High level languages are meant to ‘hide’ the machine code that causes computers to work through a level of abstraction. They follow syntax and deal with things like objects, arrays, variables, methods, [[OOP Object Orientated Programming|OOP]] and loops. ^blurb

## Types of High-Level Languages
High level languages can be compiled or interpreted. 

### Interpreted Languages
*Interpreted* languages are read and directly executed, without a compilation stage. A helper program known as an interpreter converts instructions directly into machine code to be run. This means the code will run until an error is encountered, but also that interpreted languages are often slower because each line needs to be read and interpreted before it is run. 

> [!example]+ :bulb: Example
> 
> Python and Javascript are interpreted languages.

### Compiled Languages
Compiled languages are transformed into an executable before running. These executable can be machine code, or intermediate representations.

#### Machine Code Generation
With machine code generation, the compiler translates the machine code directly to machine code by creating a file known as *object code*. This is *machine-dependant*, as object code needs to be compiled for each machine that the code must run on due to the processor architecture or operating system. 

> [!example]+ :bulb: Example
> 
> Delphi compiles directly to machine code

#### Intermediate representations
Intermediate representations rely on a translation layer, called a *bytecode*, which allows it to run on different systems through a virtual machine without recompilation. This virtual machine simulates a type of CPU architecture, allowing it’s own interpreter to run without being machine dependant. The virtual machine then translates it’s own instructions to CPU instructions. 

This translation layer allows the code to be executed on any system where the virtual machine is supported, allowing the code to be portable. It also only has to be compiled once, but because of this if there are any syntax errors the code will not compile and cannot be run. 
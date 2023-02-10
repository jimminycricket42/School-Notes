---
date: [Mon 08/08 2022]
aliases: [ ]
tags: [GR10/Q3 code ]
modified: Thu 03/11 2022 08:00
---
# Loops
In code, we have 3 main types of loops:
- For … do
- While … do
- do … while

The amount of times a loop iterates can be controlled by [[Logical Operators]]. This is the *condition* that causes the loop to *terminate*. Always ensure a loop will terminate – otherwise you can create a memory-leak or have a user repeating the same action infinitely. 
## For Loops
```java
bool condition;
for (condition) {
	System.out.println("Hello world!")
}
```

For loops can be used whenever we have a set number of times we need to iterate through a loop. 

```mermaid
%% input: [/input/] %%
%% Decision: {Decision} %%
flowchart TD
id2([Start])
id2-->id3[/input/]-->id4{"for (condition)"}
id4-- false --> id6[continue program]
id4-- true --> id5[loop arguments]
id6-->id1
id5-->id4
id1([End])
```

## While Loops
```java
bool condition;
while (condition) {
	System.out.println("Hello world!")
	condition++
}
```
While loops can be used to iterate whenever we don’t know how many times the loop needs to be iterated through. 
```mermaid
%% input: [/input/] %%
%% Decision: {Decision} %%
flowchart TD
id2([Start])
id2-->id3[/input/]-->id4{"while (condition)"}
id4-- false --> id6[continue program]
id4-- true --> id5[loop arguments]
id6-->id1
id5-->id4
id1([End])
```

## Do Loops
```java
do 
loop arguments
while (condition)
```
Do loops can be used when we have to iterate through a piece of code at least once, whether or not the condition is true. 
```mermaid
flowchart TD
id2([Start])
id2 --> id3[Loop Conditions]
id3 --> id4{"while (condition)"}
id4 -- false --> id1
id4 -- true --> id3
id1([End])
```

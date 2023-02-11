---
aliases: [ ]
tags: [GR11/Q1]
created: Sun 19/02 2023
---
# OOP Object Orientated Programming
Object Orientated Programming is a philosophy that any problem can be broken into components, known as objects. Objects can be interacted with, changed, and viewed at any point. ^blurb

OOP can be broken down into a few main parts, one of which is *the class*. The class is a blueprint for an object, and defines how it will behave. If an object of a class is initialised, it takes on the components that make up that class. A class is made of *fields*, which store properties for an object of a specific class, as well as *methods*, which are actions that a class can perform. 

Each time a class is used to create an object (called initializing), a new *instance* of that class is created. This gives the object all the fields and methods within the class. The property of all information being contained within a class is called *Encapsulation*, which occurs at every initialisation of a new instance. This also means that each instance is encapsulated, and stores it’s data separately from all other instances of the same class. 

> [!example]+ :bulb: Example: The “Line” Class
> 
> Let us say we want to make a program that can draw us lines of characters within our terminal. 
> 
> We want to break that into a class, so that we can change the line type as well as the length of the line. These values will be stored in fields, and the class will have a method to draw a line. 
> 
> The code will look like:
> 
> ```java
​public class Line {
int size = 2;
char pattern = '*';
​public void draw {
  for (int i = 1; int <= size; i++)
  System.out.print(pattern);     
  System.out.println();
  }
} 
>```
>
> This creates a class which we can call in the main method. To do this, we must initialize a new Line class that further allows us to define size and pattern
> 
> Lets create an object named stripe within the main method:



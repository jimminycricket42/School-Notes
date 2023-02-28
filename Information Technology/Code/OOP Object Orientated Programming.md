---
aliases: [OOP, Java, classes]
tags: [GR11/Q1 code/theory ]
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
> ```java
public class UseLine {
  public static void main(String[] args) {
  Line stripe = new Line();
  stripe.draw();
  stripe.size = 5;
  stripe.draw();
  stripe.pattern = '&';
  stripe.draw();
  }
}
>```
>This shows what we can do with OOP: create reuseable classes that allow us to modify their code simply. However, this example does not conform to our next topic: the rules of creating good classes.

Within a class there are methods and fields. These aren’t very distinguishable without looking at a class itself, but one way to differentiate is to look at whether a component is called or accessed. Methods are called, and are always in the format `class.method(parameters)`, while fields are accessed using `class.field = "argument"`. 

Together, classes make up an application. Applications contain at least one main method, as well as lots of classes. A class cannot run without a main method, and once it has a main method, it can be considered an application. 

## The rules of Class Design
1. Use private fields
2. Do not gather user input or output in a class
3. Create at least one constructor
4. Create necessary accessor methods for private fields
5. Create necessary mutator methods for private fields
6. Create a toString method to combine values of fields. 

## Components of a class
Classes can contain many things inside of them. The components we look at are:
- Fields
- Methods
	- Constructor Methods
	- Mutator Methods
	- Accessor Methods
	- toString Methods/concatenation methods. 

### Fields
Fields store data that can be accessed using [[#Accessor Methods]]. Fields should be private to allow for [[Validation Rules]] to be implemented, or for operations to happen efficiently, such as forming other variables off of a set of inputs. 

### Methods
Methods contain actions that must be carried out when called upon. They use the data within fields to do this. Methods can carry out any action doable by code; they can manipulate data, return data, or set variables. 

There are a couple of important methods to include as part of good method creation. These are:
- Constructor Methods
- Mutator Methods
- Accessor Methods
- toString Methods/concatenation methods

#### Constructor Methods
Constructor methods set the data for fields at the creation of an object. They can be parameterized or they can contain default values. A good class has both, allowing for default values that can also be changed to be parameters. 

Default constructors contain default values, and is called without any supplied parameters. 

Parameterised constructors allow for values to be set at initialisation. They will never conflict with default constructors, as constructors can only be called at initialisation of a new object. 

> [!note]+ :spiral_notepad: Overloading Methods
> When there are multiple methods with the same name, but different parameters then they are known as overloaded methods. 

> [!example]+ :bulb: Constructors in the Line Class
> 
> In this example, there is both a default constructor `public Line()`, as well as a parameterized constructor `public Line(int s, char p)`. Either can be called without interfering with each other. 
> 
> ```java
> public class Line {
>   private int size;
>   private char pattern;
> 
>   // CONSTRUCTORS
>   public Line() {
> 	  size = 5;
> 	  pattern = '-';
>   } // Default Constructor
>   
>   public Line(int s, char p) {
> 	  size = s;
> 	  pattern = p;
>   } // Parameterized constructor
>   
>   public void draw() {
>     for (int i = 1; i <= size; i++)
>       System.out.print(pattern);
>     
>     System.out.println();
>   }
> }
>```
> > The unnecessary methods have been removed for sake of demonstration. 
> 

#### Mutator Methods
Mutator Methods are used to change private fields. They are superior to simply allowing direct access to fields as they allow you to place [[Validation Rules]] to check when a class user changes a class value, as well as allows superior control and flexibility to what happens to inputted data, such as parsing a string to an integer when it is changed. 

The naming convention for Mutator methods is: `setField(object f)`. They are always public void methods, as they have no need for a return value and must be accessible outside a class. 

> [!example]+ :bulb: Mutators in the Line Class
> 
> In this example, the mutators for `size` and `line` have been coded, as well as the declaration of size and line. We assume size and line have been initialized via the correct [[#Constructor Methods]]. 
> ```java
> public class Line {
>  private int size;
>  private char pattern;
>
>  // MUTATORS
>  public void setSize(int s) {
>	  size = s;
>  }
>  public void setPattern(char p) {
>	  pattern = p;
>  }  
>// METHODS
>  public void draw() {
>    for (int i = 1; i <= size; i++)
>      System.out.print(pattern);
>    
>    System.out.println();
>  }
> }
> ```


> [!example]+ :bulb: Validation Checks in Mutators
> 
> This example demonstrates one of the reasons we use mutator methods to access data. It  recieves scores, implements a data check to make sure they are lower than 100%, and then stores it after space for an error message. 
> ```java
> public class ScoreHolder {
>   private int score;
>   private string name;
>   
>   // Constructors go here
>
>   // Mutators
>   public void setName(string n) {
>     name = n
>   }
>   public void setScore(int s) {
>     bool scoreValid = s <= 100
>     if (scoreValid) {
>       score = s
>     } else {
>        // Error
>     }
>   }
> }
> 
> ```
#### Accessor Methods
Accessor methods allow us to access private fields within a class. They are typed methods, and return the contents of the variable being accessed. They follow the naming convention of: `getField()`, and are always typed public methods. The values they return should be used in the main method; they should be stored in a variable or they should be outputted immediately. 

> [!example]+ :bulb: Example
> 
> In this example we create the accessor methods for `size` and `pattern`. 
> ```java
> public class Line {
>  private int size;
>  private char pattern;
>  
>  // ACCESSORS
>  public int getSize() { return size; }
>  public char getPattern() { return pattern; } 
>  
>  public void draw() {
>    for (int i = 1; i <= size; i++)
>      System.out.print(pattern);
>    
>    System.out.println();
>  }
>}
>```

#### toString Methods/concatenation methods. 
A toString method is a way to summarize the data contained in an object in a human readable way. Each variable is shown, along with it’s value. 

> [!example]+ :bulb: Example
> 
> ```java
> public class Rectangle {
>	
>	private double base;
>	private double height;	
>	private double area;
>	private boolean isSquare = false;
>	
>	public Rectangle() {
>		base = 2;
>		height = 4;
>	}
>	
>	// Methods
>	public double calcArea() {
>		area = base * height;
>		return area;
>	}
>	
>	public String toString() {
>		if (isSquare) {
>			return "Square\nLength: " + (int) base + "\nWidth: " + (int) height + "\nArea: " + area;
>		} else {
>			return "Rectangle\nLength: " + (int) base + "\nWidth: " + (int) height + "\nArea: " + area;
>		}
>	}
> }
> ```
> Output if `toString()` is called with default values:
> ```output
> Rectangle
> Length: 2
> Height: 4
> Area: 8.0
>```

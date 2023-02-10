---
aliases: [ ]
tags: [GR10/Q2 maths/graphing ]
created: Sat 20/08 2022
modified: Tue 01/11 2022
---
# The Four Graphing Functions
We look at 4 functions:
- The Straight line  
- The Parabola 
- The Hyperbola 
- The Exponential Functions  ^blurb

## Straight Line
$$
\begin{gathered} 
y = mx + c \\
\textrm{where } x \in \mathbb{R}
\end{gathered}
$$
For Instance:
$$y = x$$
```desmos-graph
y = x
```

### Affect of m on the graph
“m” defines the gradient of the graph. 
$$y=2x$$
```desmos-graph
y=2x
```
an integer > 1 causes the gradient to be more steep
$$y = -\frac{1}{2}x$$
```desmos-graph
y=-(1/2)x
```
a fraction causes the gradient to be less steep

### Affect of c on the graph
“c” defines the y-intercept of the graph
$$y=x+4$$
```desmos-graph
y = 1x + 4
```
$$y=x-2$$
```desmos-graph
y=x-2
```

## Parabola
$$
\begin{gou}
y = ax^2 + q \\
\textrm{where } x \in \mathbb{R}
\end{gou}
$$
For instance:
$$
y=x^2
$$
```desmos-graph
y=x^2
```

### Affect of a on the Graph
$$y = 2x^2$$
```desmos-graph
y = 2x^2
```
“a” makes the arms of the graph steeper. 
$$y=-2x^2$$
```desmos-graph
y=-2x^2
```
“-a” makes the graph move down 

### Affect of q on the Graph
“q” changes the y-intercept of the graph
$$y = x^2 -2$$
```desmos-graph
y = 1x^2 -2
```
“q” causes the graph to move on

## Hyperbola
Hyperbolas have *asymptotes*, meaning areas that the graph does not pass through

$$
\begin{gather}
y = \frac{a}{x} + q \\
\textrm{where } x \in \mathbb{R}
\end{gather}
$$

### Affect of a on the Graph
$$
y = \frac{6}{x}
$$ 
```desmos-graph
y = 1/x
y = 6/x

y = 0|dashed
x = 0|dashed
```
“a” causes the graph to ‘expand’ outwards from the origin

$$
y = \frac{-2}{x}
$$
```desmos-graph
y = \frac{1}{x}
y = \frac{-2}{x}
```
“-a” causes the graph to go through the second and fourth quadrant instead of the first and third

### Affect of q on the Graph
$$
y=\frac{1}{x}+4
$$
```desmos-graph
y=\frac{1}{x}
y=\frac{1}{x}+4

```
“q” moves the graph up or down, and changes the y-position of the asymptote.

## Exponential Function
The exponential function has an asymptote at the “q” value
$$
\begin{gather}
y = a^x + q \\
\textrm{where } x \in \mathbb{R} \textrm{ and } x \neq 1
\end{gather}
$$

For instance:
$$
y=2^x
$$
```desmos-graph
y = 2^x
y=0|dashed
```

### Affect of “a” on the Exponential Function
$$
y=4^x
$$
```desmos-graph
y=2^x

y=4^x

y=0|dashed
```
“a” changes the y-intercept

$$
y = -4*2^x
$$
```desmos-graph
y=2^x

y = -8^x

y=0|dashed
```
“-a” causes the graph to decrease 

### Affect of “q” on the Exponential Function
$$ y=2^x+2 $$
```desmos-graph
y=2^x
y=2^x+2
y=0|dashed
y=2|dashed
```
“q” moves the graph (asymptote) up
$$ y=2^x-3 $$
```desmos-graph
y=2^x
y=2^x-3
y=0|dashed
y=-3|dashed
```
“-q” moves the graph (asymptote) down

### Affect of “-x” on the Exponential Function
$$ y=2^{-x}$$
```desmos-graph
y=2^x
y=2^{-x}

y=0|dashed
```
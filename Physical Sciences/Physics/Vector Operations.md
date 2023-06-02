---
aliases: [vector sums, decompose ]
tags: [GR11/Q1]
created: Sat 22/04 2023
---
# Vector Operations
To work out the sum of vectors, you need to know their direction and magnitude. If two vectors act in the same plane you can add/subtract them like scalars. If they work in different planes, you must decompose the vector into it’s $x$ and $y$ components. By working in one plane at a time we can then add and subtract the components like scalars, before composing the $x$ and $y$ components into the resultant vector. ^blurb

> [!summary] How to work out vector sums:
> 1. State your vectors in the form $(r:\theta)$ where $r$ is the magnitude and $\theta$ is the direction in relation to the x-axis.
> 2. Apply [[Trigonometric Reductions]] to simplify to an acute angle.
> 3. Using [[Trigonometry]], apply the ratios to find the $x$ and $y$ axes of the vector.
> 	- This is done with the formula $x = r\cos\theta$ or $y = r\sin\theta$ (but remember to think about the position of your sides and angles here, sin and cos may change which axes they are working out if the triangle is rotated)
> 4. Add all vectors acting in the same plane to get $x_{R}$ and $y_{R}$
> 5. Using the reciprocal ratios, compose the x and y back into a single vector
> 	- This is done with the formulae: $r = \sqrt{x_R^2 + y_R^2}$ ; $\theta = \cot{\frac{x_R}{y_R}}$


## Decomposing a Vector
We can use [[trigonometry]] to find the $x$ and $y$ components of a vector by using $\sin$ and $\cos$ and multiplying it by the magnitude, leaving us with just the $x$ or $y$ component of the vector

$$\begin{align}
\\ && F_x = r\cos(\theta) 
\\ && F_y = r\sin(\theta)
\\ & \textrm{Where: }
\\ & F = && \textrm{x or y Component of Force } ()
\\ & r = && \textrm{Magnitude of Force } (N)
\\ & \theta = && \textrm{Direction of Force } (\degree)
\end{align}$$

> [!extra]- Mathematical Explanation of How decomposition works
> $$\begin{align}
> \\ \cos\theta = \frac{x}{r} 
> \\ \therefore r\cdot\cos\theta = x
> \end{align}$$

We can use the diagram below to see which ration to use in what scenario, or we can apply [[Trigonometric Reductions]] to create an acute-angle in the 1st quadrant.

![[Trig Circles.jpeg]]

> [!example]+ :bulb: Example
> 
> A force is acting with $300N ; 34\degree$. Calculate it’s x and y components. 
> $$\begin{align}
 \\ && F_1 = 300N ; 34\degree
 \\ & F_{1x} = 300\cos(34\degree) = 248,71N left 
 \\ & F_{1y} = 300\sin(34\degree) = 167,75N up
 \end{align}$$



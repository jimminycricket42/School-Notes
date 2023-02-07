---
aliases: [ ]
tags: [ ]
created: Sun 06/11 2022
modified: Sun 06/11 2022
---
# Learning LaTeX
 This page is a Summary (and a sort of guide) to my personal learning of the [LaTeX document preparation system]([LaTeX - A document preparation system (latex-project.org)](https://www.latex-project.org/)) ^blurb

## Starting Equations
latex equations are started using:
```latex
$$
equation!
$$
```

equations can be put in a line using `$ equation $` → $equation$


## "Basic" Operations
### Standard Operators
use ``+, -, \times, /`` (plus, minus, times, divide) as your standard operators
```latex
+, -, \times, /
```
$$+, -, \times, /$$

### Fractions
use the ``\frac{ }{ }``


```latex
\frac{100}{50}
```

**becomes:**
$$\frac{100}{50}$$

### Exponent-related operators
#### Squares and Bases
Squares can be shown using `^x` and bases through `_x`

```latex
y = ax^2 + bx + c
```
$$
y = ax^2 + bx + c
$$
```latex
16_2 = 4
```
$$
16_2 = 4
$$

#### Square roots, cube roots, and more roots
Square roots can be made using the `\sqrt{x}` command, but this is extensible to any number. This is done by modifying the command to `\sqrt[y]{x}`

$$
\sqrt{x}
$$

$$
\sqrt[y]{x}
$$

#### Other useful symbols
`\mathbb{R}` → $\mathbb{R}$

`\pm` → $\pm$

## Trig in LaTeX
sin, cos, tan, cosec, sec, and cot all have special commands:
```latex
\sin
\cos
\tan
\csc 
\sec
\cot
```
$$
\sin
\cos
\tan
\csc
\sec
\cot
$$

Theta can also be shown as `\theta` → $\theta$

## Show Text in your equation
Use the ``\textrm{ }`` modifier 


```latex
\textrm{What you want to write in text} 
```
**becomes:**
$$\textrm{What you want to write in text}$$

## Shapes in LaTeX
```latex
\Box - \bigcirc - \triangle ⇌ \Box \bigcirc \triangle
```
$$
\Box - \bigcirc - \triangle ⇌ \Box \bigcirc \triangle
$$
## Multi-line Equations
To create multi-line equations we use LaTeX environments
they follow the syntax:
```latex
\begin{gather}
\\ create a new line
\\& the text will align to any "&" on the line
\end{gather}
```

There are a lot of different environments, but the most useful are:
- align – aligns all text to the right side, unless specified otherwise by a `&`
- gather – centre align

> [!example]+ 💡 Example
> 
> $$\begin{flalign}
& n = \frac{m}{M}
\\&
\\& n = \textrm{number of moles}
\\& m = \textrm{mass (grams) of substance}
\\& M = \textrm{molar mass} g.mol{^-1} \textrm{(use relative atomic mass)}
\end{flalign} $$
## Matrices
Matrices are another type of environment, and can be shown using the command: `\begin{matrix}`
There are multiple types of matrices, but the best one is `\begin{Bmatrix}`
```latex
\begin{Bmatrix}
a & b & c \\
d & e & f \\
\end{Bmatrix}
```
the `&` sign creates a new column, while the `\\` sign creates a new row

$$
\begin{Bmatrix}
a & b & c \\
d & e & f \\
\end{Bmatrix}
$$
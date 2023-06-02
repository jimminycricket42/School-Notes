---
aliases: [ ]
tags: [GR11/Q1]
created: Wed 15/03 2023
---
# Trigonometric Identities
Trigonometric Identities are ways to manipulate trigonometric ratio’s to prove that certain expressions involving trigonometry are equal. ^blurb

## The basic identities
### The co-function identity
$$

\sin^2\theta + \cos^2{\theta} = 1
$$
Proof:
$$

\begin{align}
\\ \textrm{Pythagoras } & x^2 + y^2 = r^2
\\ \therefore \space & \frac{x^2}{r^2} + \frac{y^2}{r^2} = \frac{r^2}{r^2}
\\ & sin^2\theta = \frac{x^2}{r^2}
\\ & cos^2\theta = \frac{y^2}{r^2}
\\ \therefore \space & sin^2\theta + cos^2\theta = 1
\end{align}
$$
### The tan Identity
$$
\tan\theta = \frac{\sin\theta}{\cos\theta}
$$
Proof:
$$
\begin{align}
\\ & \frac{\sin\theta}{\cos\theta}
\\ & = \frac{y}{r} \div \frac{x}{r}
\\ & = \frac{y}{r} \times \frac{r}{x}
\\ & = \frac{y}{x} = \tan\theta
\end{align}
$$

## Proving identities
When working with identities it is important to distinguish the two separate sides of the identity. We want to make the right hand side and the left hand side equal to each other without actually changing either expression, merely simplifying it or applying other proof’s or reductions to it. 

There are a couple of techniques we can use to manipulate the sides to prove identities, such as:
- [[Algebraic Simplification of Fractions]]
- [[Factorisation]]
- Simplification
- Other trigonometric identities
- Pythagoras’s Theorem

> [!example]+ Example: Identity using the [[Algebraic Simplification of Fractions]]
> ![[Algebraic Simplification of Fractions]]
> $$
> \begin{align*}
> \\\textrm{Prove that:} \space & \frac{1}{1-\sin\theta} + \frac{1}{1+\sin\theta} = \frac{2}{\cos^2\theta}
> \\ \textrm{RHS} \space & \frac{2}{\cos^2\theta}
> \\ \textrm{LHS} \space & \frac{1}{1-\sin\theta} + \frac{1}{1+\sin\theta}
> \\ & \frac{1 + \sin\theta + 1 - \sin\theta}{(1-\sin\theta) (1+\sin\theta)} && \space \textrm{...Multiply by LCD} 
> \\ & \frac{2}{1-\sin^2\theta} && \space \textrm{...Simplification, Diff. Squares}
> \\ & \frac{2}{\cos^2\theta} && \space \textrm{...The co-function identity} 
> \end{align*}
> $$



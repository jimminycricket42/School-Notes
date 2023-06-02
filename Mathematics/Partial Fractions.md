---
aliases: [ ]
tags: [GR11/Q1 apm]
created: Mon 27/03 2023
---
# Partial Fractions
A partial fraction is a way of expressing one fraction as the sum of other fractions. We can do this by breaking apart a factorised denominator into two fractions and then solving for the numerators. ^blurb

**Steps to solve a partial fraction:**
1. Factorize the denominator
2. Split denominator into terms, with the the highest power in the numerator being one lower than the highest power in the denominator.
3. Express numerators in standard form
4. Simplify denominators by multiplying numerators by denominators
5. Use values of X to eliminate terms to get one value of a numerator
6. Using previous numerators, use a different value of x to solve for the other numerators until values are found for all numerators

> [!example] Breaking down a partial fraction
>$$
>\begin{align}
>\\& \frac{1}{x+2} + \frac{2}{x+1} = \frac{3x+3}{x^2 + x - 2}
>\\\textrm{Factorize Denominator }& \frac{3x+3}{x^2 + x - 2} = \frac{3x+3}{(x + 2)(x-1)}
>\\\textrm{Break into addition of fractions } & \frac{3x+3}{(x+2)(x-1)} = \frac{A}{x+2} + \frac{B}{x-1}
>\\ \textrm{Simplify denominators } \space & 3x + 3 = A(x-1) + B(x+2)
>\\ & \textrm{Finding A and B:}
>\\ \textrm{let } x = 1; \space & 3(1) + 3 = A(1-1) + B(1+2) && \therefore B = 2
>\\ \textrm{let } x = -2; \space & 3(-2) + 3 = A(-2-1) + 2(-2+2) && \therefore A = 1
>\\& \therefore \frac{3x+3}{x^2 + x - 2} = \frac{A}{x+2} + \frac{B}{x-1} = \frac{1}{x+2} + \frac{2}{x+1}
>\end{align}
>$$

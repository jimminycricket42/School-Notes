
---
aliases: [surds ]
tags: [GR10/Q4 maths/algebra GR11/Q1 ]
created: Thu 19/01 2023
---
# Exponents
Powers work differently than other numbers. To ensure the correct outcome of calculations involving powers, the exponential laws were created. Exponents can also be used to describe many different types of numbers, such as surds, whole numbers, and fractions. ^blurb

![[Representation of Powers.jpeg]]

## Exponential Laws
The cases that the laws apply to are:
- The addition and subtraction of powers
- The multiplication and division of powers
- Powers applying to brackets
	- Powers applying to brackets with one term
	- Powers applying to brackets with multiple terms

### The addition and subtraction of exponents
Law: Power with the same base but different exponents cannot add or subtract

$$
x^a \pm x^b \text{…Error}
$$

### The multiplication and division of exponents
Law: Multiplication and division of powers with the same base will cause the exponents to add or subtract

$$
x^a \times x^b = x^{a + b}
$$
$$
\frac{x^a}{x^b} = x^{a - b}
$$

> [!note]+ :spiral_notepad: Breaking apart exponential numbers
> We can use this in reverse to break down some numbers, for instance:
> 
> $4 = 2^2$
> 
> $8 = 2^3$

### Powers Applying to Brackets
#### Powers applying to brackets with one term
Law: Powers applied to brackets will multiply all powers within the bracket

$$
(abc)^d = a^d b^d c^d
$$

$$ (a^b)^c = a^{bc} $$

#### Powers applying to brackets with multiple terms
Law: Powers applied to brackets with multiple terms will multiply the entire bracket by itself as many times as the power states. 

This can be simplified with methods such as [[Pascal's Triangle]] or [[FOIL]].

#### Foil
$$
(a + b)^2 = (a + b)(a + b) = a^2 + 2ab + b^2
$$
#### Pascal’s triangle
$$
(a + b)^3 = (a + b)(a + b)(a + b) = 1 a^3 + 3 a^2 b + 3 a b^2 + 1 b^3
$$

---

## Types of Exponents
### Powers where the exponent is a fraction
Rational Fraction exponents can be converted into roots. The denominator becomes the root, and the numerator is applied to the base as an exponent

$$ a^\frac{1}{2} = \sqrt{a} $$

$$ a ^\frac{2}{5} = \sqrt[5]{a^2} $$


> [!tip]- :star_struck: Extra: Using rational exponents
> Rational exponents can be used to solve sums including surds, as they adhere to the other exponential laws and can therefore be used algebraically to solve for $x$ where surds are involved

### The power of 0
Any number with the exponent of 0 is equal to one

$$
n^0 = 1
$$

### Negative Powers
Negative powers cause the base to become the denominator of a fraction, with the power applied to the denominator. Whatever the coefficient of the base is will make up the numerator, unless it also has a negative power. 

$$
n^{-1} = \frac{1}{n}
$$
$$
mn^{-3} = \frac{m}{n^3}
$$

## Solving Exponential Equations
When the unknown is in the exponent, we call the equation an exponential equation. This means that we need to apply the laws and some [[Factorisation]] to make the bases of our equations the same so we can equate the exponents and solve for x.

> [!example]+ :bulb: Exponential Equations
> 
> $$\begin{align}
\\& 2^x = 4^{x + 1}
\\& 2^x = 2^{2(x + 1)}
\\& x = 2x + 2
\\& -x = 2 \therefore x = -2
\end{align}$$

> [!example]+ :bulb: Example
> 
> $$\begin{align}
\\& 2^x + 2^{x+1} = 24
\\& 2^x + 2^x \times 2^1 = 24 &&\textrm{... exp. law } n^x \times n^y = n^{x + y}
\\& 2^x(1 + 2) = 24 &&\textrm{... Factorised through common factors}
\\& 2^x = \frac{24}{3} = 8 &&\textrm{... Simplifed by dividing the 
coefficient}
\\& 2^x = 2^3 &&\textrm{... prime factor base of 8}
\\& \therefore x = 3 &&\textrm{... Equating the exponents}
\end{align}$$

> [!example]+ :bulb: Example
> 
> $$\begin{align}
\\ & 8^x \times \frac{1}{4^{x-1}}=\frac{1}{32}
\\ & 2^{3x}\times 2^{-2x+2}=2^{-5} && \textrm{... prime factor bases \& powers applying to brackets}
\\ & 3x -2x + 2 = -5 && \textrm{... equating the exponents}
\\ & \therefore x = -7 
\end{align}$$

The basic steps are:
1. Convert terms into their prime factors
2. See if the exponents can be equated (both sides must have the same base) 
3. Separate the powers where the exponents contain the variable. Use exponential laws and factorisation. 
4. Simplify til only one side has variables
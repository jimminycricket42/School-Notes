---
date: [Mon 22/08 2022]
aliases: [factorise ]
tags: [GR10/Q1]
modified: Tue 01/11 2022 09:00
---
# Factorisation
Factorisation is the process of making an equation into a single term. ^blurb

A term is a single mathematical expression which has one output inside of it. Terms are separated by addition of numbers or variables (including the addition of negative numbers). 

## Steps to factorizing:
1. Always take out the *[[Highest Common Factor (HCF)]]* first
	1. check for any common-brackets
	2. Check if you can switch around any terms to match the signs
2. Count the terms
	- if there are *two terms*, look for a difference of squares, or a sum or difference of cubes.
	- if there are *three terms*, look for a Trinomial.
	- if there are *four or more terms*, look for a way to use Grouping.
3. Apply the factorisation method for difference of cubes, trinomial, or grouping. 
4. Repeat until fully factorized

## Factorisation Methods
We look at:
- [[Highest Common Factor (HCF)]] removal
- Difference of squares
- Sum or Difference of cubes
- Trinomial
- Grouping

### HCF Removal
If all terms in an equation share a common factor, we can factorize by removing that common factor through division. To do this we divide all terms within an equation by the common factor. 

> [!example]+ 💡 Example: 4x + 2
> 
> lets take 4x + 2 as an example
> $$\begin{gather}
4x + 2 \\
\textrm{HCF of }4 \textrm{ and } 2 = 2 \\
\therefore 2(2x + 1) = 4x + 2
\end{gather} $$

### Difference of squares
When there is a difference of squares, we can factorize by splitting the two squares into their roots. We can prove this works by multiplying the roots through [[FOIL]]. 

> [!example]+ 💡 Example 4x^2 - 16
> 
> $$ \begin{gather}
4x^2 - 16 \\
= (\sqrt{4x^2} + \sqrt{16})(\sqrt{4x^2} + \sqrt{16}) \\
= (2x + 4)(2x - 4) →
\end{gather} $$

Notice how we split the single term into two terms with opposite signs. If these signs were the same, our [[FOIL|bracket multiplication]] would result in 3 terms instead of 2. This is because square numbers are part of [[Quadratic Equations]], which have two real roots. 

### Sum or Difference of cubes
Cubes can be factorized by putting them into two separate roots – a binomial and a trinomial. This can be proven through [[polynomial division]], but is easier to do using a standard form. 

$$\begin{gather}a^3 \pm b^3 = (a \pm b) (a^2 \pm ab + b^2)\\
\textrm{if } a^3 + b^3 \textrm { then: } 
a^3 + b^3 = (a + b) (a^2 - ab + b^2)\\
\textrm{if } a^3 - b^3 \textrm { then: } 
a^3 - b^3 = (a - b) (a^2 + ab + b^2)\\
\end{gather}$$

> [!example]+ 💡 Example: 8x^3 - 27
> 
> $$\begin{gather}
a^3 - b^3 = (a - b) (a^2 + ab + b^2)\\
8x^3 - 27 = (2x + 3) (4x^2 - 6x + 9^2)
\end{gather}$$

### Trinomial
Trinomials can be factorized by applying the principles of [[FOIL]], but in reverse to create an expression where [[FOIL|bracket multiplication]] creates a trinomial. 

$$ ax^2 + bx + c $$
If we look at this equation, we want to get what common factors of ‘a’ and ‘c’ will add to create ‘b’. 

lets fill in ‘a’ ‘b’ and ‘c’ to make this simpler. 

$$ 6x^2 + 17x + 12 $$
factors of the coefficient of x<sup>2</sup> and the constant term:
$$ \begin{gather} 
6 = \begin{Bmatrix} 
1 \times 6 \\ 
2 \times 3 
\end{Bmatrix} \\
12 = \begin{Bmatrix}
1 \times 12  \\
2 \times 6  \\
3 \times 4 
\end{Bmatrix}
\end{gather} $$

Now we can look and see which factors, when multiplied and added, will give us the coefficient of x. 

$$ \begin{gather} 
6 = \begin{Bmatrix} 
1 \times 6 \\ 
\mathbf{{\color{blue}2} \times {\color{red}3}}
\end{Bmatrix} \\
12 = \begin{Bmatrix}
1 \times 12  \\
2 \times 6  \\
\mathbf{{\color{red}3} \times {\color{blue}4}}
\end{Bmatrix} \\
\therefore({\color{blue}2} \times {\color{blue}4}) + ({\color{red}3} \times {\color{red}3}) = 8 + 9 = 17 →
\end{gather}$$

now we know what factors of  the coefficient of x<sup>2</sup> and the constant term will give us 17 when multiplied and added. Now we can put them into a factorized sum:
$$ ({\color{blue}2}x + {\color{red}3})({\color{red}3}x + {\color{blue}4})
$$
Note how the factors are cross-multiplied, but in the final factorisation they are not crossed anymore. 

> [!example]+ 💡 Example: 12x<sup>2</sup> - 56x +9
> 
> $$\begin{gather} 
12x^2 - 56x + 9 \\
\textrm{Factors of 12 and 9:} \\
12; 9 = 
\begin{Bmatrix} 1 \times 12 \\ {\color{red} 2} \times {\color{blue} 6} \\ 3 \times 4 \end{Bmatrix}
;
\begin{Bmatrix} {\color{red} 1} \times {\color{blue} 9}  \\ 3 \times 3  \end{Bmatrix} \\
{\color {red} 2 \times 1} + {\color {blue} 6 \times 9} = 56\\
\therefore {\color {red} 2 \times -1} + {\color {blue} 6 \times -9} = -56 \\
\therefore 12x^2 - 56x + 9 = ({\color {red} 2}x -{\color {blue} 9})({\color {blue} 6}x - {\color {red} 2})
\end{gather}$$

### Grouping
Grouping is the most uncommon form of factorisation, because often it does not simplify into a single term, rather creating less terms that can be factorised further using other methods. 

$$ 4a - 4b + ad - bd $$

notice how we have 4 terms, but b<sup>2</sup> and c<sup>2</sup> only appear in two of them? This means we will likely have to employ grouping – especially considering there are no current common factors, differences of squares, trinomials, or cubes. This means we must break up the sum in a way that will get us one of the other methods to simplify with. 

$$ \begin{gather} 4(a-b) + d(a-b) \\ = (a-b)(4+d) \end{gather} $$

Initially, there were no common factors between each term. Through grouping we created a common factor that could then be used to further factorize. 

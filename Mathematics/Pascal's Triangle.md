---
aliases: [ ]
tags: [GR11/Q1]
created: Tue 07/02 2023
---
# Pascal's Triangle
Pascal’s Triangle is a method of *binomial expansion* that simplifies expressions like $(x + y)^5$ without simply multiplying the bracket by itself each time. ^blurb

![[Pascals triangle.png]]

Using the above series, we can use each row as a guide for the coefficients of terms, while we decrease the exponents of a from $n$ to 0, and increase the exponents of b from 0 to $n$


$$\begin{align}
\\& (a + b)^5 \textrm{ where } 5 = n
\\& \therefore \textrm{ Row 5 of Pascal's Triangle will be used. } 1;5;10;10;5;1
\\& (a + b)^5 = 1 a^5 b^0 + 5 a^4 b^1 + 10 a^3b^2 + 10 a^2 b^3 + 5 a^1 b^4 + 1 a^0 b^5
\end{align}$$


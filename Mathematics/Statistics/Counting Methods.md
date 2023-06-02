---
aliases: [permutations, combinations ]
tags: [GR11/Q1 apm/statistics]
created: Thu 20/04 2023
---
# Counting Methods
There are a lot of ways to count. Counting is very useful, as it is necessary to find the size of a sample space, or the amount of ways something can be done. To speed up counting, we use [[#the Fundamental Counting Principle]] ^blurb

## The Fundamental Counting Principle
The fundamental counting principle speeds up counting large amounts of possibility. 

>[!definition]
> If one operation can be done in $m$ ways, and a second operation can be done in $n$ ways, then the possible number of different ways in which both operations can be done is $m \times n$

> [!example]+
> Your mother lets you choose 4 CD’s from the store. The store sells 3 genres, and each genre has 10 CD’s to choose from. How many possible combinations are there of CD’s?
> $$
> 4 \times 3 \times 10 = 120 \textrm{ Possible Choices}
> $$

>[!example]+
>You have a three course meal. For starters, there are 2 options. For the main course, there are 6 options. For dessert there are 4 options. How many combinations are there?
>$$
>2 \times 6 \times 4 = 48 \textrm{ Possible Choices}
>$$
>You decide on soup for a starter, how many choices are there now?
>$$
>1 \times 6 \times 4 = 24 \textrm{ Possible Choices}
>$$

> [!example]+
> Seven students want to sit on seven chairs. Each student can only sit on one chair (no sharing!)
> $$
> 7 \times 6 \times 4 \times 3 \times 2 \times 1 = 5040 \textrm{ Possible Choices}
> $$
> This can also be written as $7!$, spoken as 7 factorial. We discuss this more [[Factorial Notation]]

## Permutations
Permutations refers to an arrangement of objects where order is important. In each case there is a total number of objects, and a total number of possible outcomes. 

If there are no limits, then the amount of permutation is how many ways the objects can be arranged. If there are limits, then the amount of permutations is how many ways the objects can be arranged, removing each invalid outcome. 

Permutations are such a common form of problem that they have their own notation:
$$\begin{align}
\\ & ^nP_r = \frac{n!}{(n-r)!}
\\ & \textrm{Where: }
\\ & n = \textrm{Total Number of Objects}
\\ & r = \textrm{Size of the arrangement}
\end{align}$$
> [[Factorial Notation]]


>[!example]+
>There are 10 people and 7 chairs. How many permutations of their arrangement can there be?
>$$\begin{align}
>\\ & ^nP_r = ^{10} P \space_7
>\\ & = \frac{10!}{(10-7)!}
>\\ & = \frac{10!}{3!} = 720
>\end{align}$$
>This means there are 720 ways to arrange 7 people from 10 people. 

> [!example]
> You have 3 maths books and 4 physics books. There are 6 spots on the bookshelf, but each subject has to remain together. 
> $$\begin{align}
> \\ & 3! \times 4! \times 2! = 288 \textrm{ Total Permutations}
> \end{align}$$
> This one looks a bit different, the size of the arrangement is big enough for each object to exist. That means $(n-r)! = 0! = 1$ 
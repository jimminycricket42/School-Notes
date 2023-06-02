---
aliases: [factorial ]
tags: [GR11/Q1 apm ]
created: Thu 20/04 2023
---
# Factorial Notation
In [[Counting Methods]], we discuss fast ways to count lots of numbers using the fundamental counting principle. In some situations, we end up with counting that looks like $6 \times 5 \times 4 \times 3 \times 2 \times 1 = 720$. We can write this as $6!$. The formula for a factorial is: $n! = n \times (n-1) \times (n-2) \times (n-3) \cdots 3 \times 2 \times 1$ ^blurb

## $0! = 1$
This statement makes little sense at first, but when looking at [[Counting Methods]] it makes a lot more sense. If you think of this as “How many ways can i arrange 0 numbers?”, you see that you can still arrange it in one way: $0$. It is the same as “How many ways can I arrange 1 number?”, there is still only one way: $1$. If I look at $2!$, I can arrange two numbers as $1;2$ or $2;1$, which is two separate [[Counting Methods#Permutations|permutations]] of 2 numbers. 
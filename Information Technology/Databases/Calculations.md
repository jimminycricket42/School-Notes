---
aliases: [ ]
tags: [GR11/Q1]
created: Sun 23/04 2023
---
# Calculations
We can perform calculations as a part of our [[SQL]] Statements. ^blurb
```SQL
SELECT <field>, <field>, [ARITHMETIC AS <alias>]
From <table>;
```

> [!example] CD_table
> ```SQL
> Select Name, Cost, AmountBought, Cost * AmountBought AS TotalPrice
> from CD_table
>```

## Possible Calculations
- Arithmetic
	- \*; /; +; -
	- MOD
- INT `INT(<value>)` – Only shows the integer portion of a number (truncates to no decimals)
- ROUND `ROUND(<value>)` – rounds the number to the nearest whole number. 
- RND `RND(<field>)`– returns a random number and inserts it into a field (note, must have a specified field otherwise all fields will fill with the first number)
	- `SELECT INT(RND(seed) * (B-A+1) + A*` gives a random number between $A$ and $B$. 

## String Manipulation
- LEFT `LEFT('<String>', <n>)` – returns $n$ of the leftmost characters of a string
- RIGHT `RIGHT('<String>', <n>)`– returns $n$ of the rightmost characters of a string
- MID `MID('<String>', <r>, <n>`– returns $n$ of the characters moving right from position $r$ within a string
- LEN – returns the length o f a string
- & – concatenates two strings
---
aliases: [ ]
tags: [GR11/Q2 code/databases ]
created: Sun 23/04 2023
---
# Selecting Data
In most [[SQL]] queries, we need to select data to update or delete. This is done using the *where* query. The where query has a lot of uses, from selecting unique data to selecting data within a range. ^blurb

The where command allows us to select records where there is specific data in certain fields. It uses [[Logical Operators]] to select this data, meaning conditions can be chained to generate information. 

The syntax of a *Where* query is:
```SQl
Where <Field> <operator> <Data>;
```
We discuss the operators more in [[#‘Where’ Operators]]

> [!example] CDDatabase
> ```SQL
> SELECT *
> From CD_table
> WHERE Genre='Alternative Rock';
> ```

## ‘Where’ Operators
The *WHERE* query has a couple of operators, namely:
- [[#Equals (=)]]
	- Equals with [[Logical Operators]]
- [[#Between… and]]
- [[#In]]
- [[#Like]]
- [[#IS NULL]]

### Equals (=)
*Equals (=)* simply checks if an entry in a field is equal to a number, string, or other data type. Using [[Logical Operators]] allows us to create more specific queries, such as “find me all the records where the artist is JayZ or Katy Perry”. 

```SQL
SELECT *
FROM <table>
WHERE <Field> = <Value> [AND/OR <Value>];
```

#### Variations:
- $=$
- $>/<$
- $>=/<=$
- $<>/!=$

### Between… and
*Between… and* is almost a shorthand syntax to find items between a range. we can use it to create queries such as “find me all records where the Release Year is between 1999 and 2010”, which would be equivalent to $$\textrm{Release year}>1999\cup\textrm{Release Year}<2010$$

```SQL
SELECT *
FROM <table>
WHERE <Field> BETWEEN <Value> and <Value>;
```

It can be used in conjunction with the NOT operator to select outside a group of values.

### In
IN lets you choose from a group of non-sequential values.

```SQL
SELECT *
FROM <table>
WHERE <Field> IN (<Value>, <Value>, ...);
```

It can be used in conjunction with the NOT operator to select outside a group of values. 

### LIKE
Like searches for text that matches a specified pattern. 

```SQL
SELECT *
FROM <table>
Where <Field> Like 'Ab*';
```

### IS NULL
Is Null searches for if something even exists in the first place. This is useful, as it can show us unknowns within a database. 

```SQL
SELECT *
FROM <table>
Where <Field> IS NULL;
```
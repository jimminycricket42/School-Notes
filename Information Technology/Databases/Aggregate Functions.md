---
aliases: [ ]
tags: [GR11/Q1]
created: Sun 23/04 2023
---
# Aggregate Functions
Aggregate functions do not deal with data in fields like other [[SQL]] functions, but rather they work with data about the table itself. This means it can look at maximums, minimums, averages, and more. ^blurb

The Aggregate Functions we look at are:
- [[#MAX()]]
- [[#MIN()]]
- [[#AVG()]]
- [[#SUM()]]
- [[#COUNT()]]


## MAX()
The MAX() Function will return the largest value within a field.

```SQL
SELECT AVG(<field>)
FROM <table>
```

## MIN()
The MIN() function will return the smallest value within a field.

```SQL
SELECT MIN(<field>)
FROM <table>
```

## AVG()
The AVG() function will average all values within a field

```SQL
SELECT AVG(<field>)
FROM <table>
```

## SUM()
The SUM() function will calculate the sum of all values within a field.

```SQL
SELECT SUM(<field>)
FROM <table>
```


## COUNT()
Count will count all the non-null entries for a chosen field. 

```SQL
SELECT COUNT(<field>)
FROM <table>;
```

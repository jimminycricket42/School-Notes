---
aliases: [ ]
tags: [GR11/Q1 code/databases ]
created: Sun 19/03 2023
---
# SQL Queries
A Query is the method used to interact with data in [[Databases]]. Queries are stated in the Structured Query Language, or SQL code. SQL allows us to select what data to show in the *query result*, which is normally shown as a table. ^blurb

## Accessing data
```SQL
SELECT [TOP <n>|DISTINCT] <field>, <field> [Calculation]
FROM <table>
ORDER BY <field> [ASC/DESC]
WHERE <field> <operator> <condition>;
```
[[Accessing Data]], [[Calculations]], [[Selecting Data]]. 
> [!note]- All queries end with a ‘;‘
> All SQL queries have a semicolon right at the end of the query to show that it has ended. 

![[Accessing Data]]
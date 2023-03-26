---
aliases: [ ]
tags: [GR11/Q1]
created: Sun 19/03 2023
---
# SQL Queries
A Query is the method used to interact with data in [[Databases]]. Queries are stated in the Structured Query Language, or SQL code. SQL allows us to select what data to show in the *query result*, which is normally shown as a table. ^blurb


```SQL
SELECT <field>
FROM <table>
ORDER BY <field> DESC /*note: can be ASC or DESC*/
WHERE <condition>;
```
> [!note]- All queries end with a ‘;‘
> All SQL queries have a semicolon right at the end of the query to show that it has ended. 

## Accessing data
There are a few commands we use to access data. We look at:
- [[#Select & From]]
- [[#Order By]]
- Where

### Select & From
Select *chooses a field* from a table. Selected fields will be shown in the *query result*, and only records with those fields will appear. A select command requires a “From” command to immediately follow in the next line that *specifies which table* to fetch the records from.

The Syntax of a *Select From* query is:
```SQL
SELECT <Field>, <Field>
From <TBL>;
```

> [!example] CDDatabase
> ```SQL
> SELECT Artist, CD_name, Genre
> FROM CD_table;
> ```
> This will select all records and display the Artist, CD_name, and Genre field flow CD_table and display them. 

### Order By
The order by command allows us to sort data, giving us information such as how many items have the same properties, or allowing us to faster access certain data. By default, the data is in Ascending order, but by specifying ASC or DESC at the end of the query we can change the order of information.

The Syntax of a *Order By* query is:
```SQL
SELECT <Field>, <Field>
FROM <TBL>
ORDER BY <Field> [ASC/DESC], <Field> [ASC/DESC];
```
>[!note]- Order by Multiple  Fields
>You can order by multiple fields by separating their field names with commas. 

> [!example]+ CDDatabase Order By Genre
> ```SQL
> SELECT Artist, CD_name, Genre
> FROM CD_table
> ORDER BY Genre desc;
> ```

>[!note] Data outside the query result. 
>You can order by data not shown in a query result. 

### Where
The where command allows us to select records where there is specific data in certain fields. It uses [[Logical Operators]] to select this data, meaning conditions can be chained to generate information. 


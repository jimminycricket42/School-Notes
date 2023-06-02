---
aliases: [ ]
tags: [GR11/Q1 code/databases]
created: Sun 23/04 2023
---
# Accessing data
There are a few commands we use to access data. We look at:
- [[#Select & From]]
- [[#Order By]]
- Where
 ^blurb

## Select & From
Select *chooses a field* from a table. Selected fields will be shown in the *query result*, and only records with those fields will appear. A select command requires a “From” command to immediately follow in the next line that *specifies which table* to fetch the records from.

The Syntax of a *Select From* query is:
```SQL
SELECT [TOP <n>|DISTINCT|] <Field>, <Field>
From <TBL>;
```

> [!example] CDDatabase
> ```SQL
> SELECT Artist, CD_name, Genre
> FROM CD_table;
> ```
> This will select all records and display the Artist, CD_name, and Genre field flow CD_table and display them. 

### TOP
You can limit how many results you get by using the `TOP <n>` condition, which will only return $n$ amount of entries, the first $n$ it finds. If you order a query then you can show the largest or the smallest amount of different things. 

### DISTINCT
Distinct means that only unique rows will be selected based on the fields they contain. It ignores duplicates of the same values, even if other fields are different. 

## Order By
The order by command allows us to sort data, giving us information such as how many items have the same properties, or allowing us to faster access certain data. By default, the data is in Ascending order, but by specifying ASC or DESC at the end of the query we can change the order of information.

The Syntax of a *Order By* query is:
```SQL
SELECT <Field>, <Field>
FROM <TBL>
ORDER BY <Field> [ASC/DESC], <Field> [ASC/DESC];
```

>[!note]+ Order by Multiple  Fields
>You can order by multiple fields by separating their field names with commas. 

> [!example]+ CDDatabase Order By Genre
> ```SQL
> SELECT Artist, CD_name, Genre
> FROM CD_table
> ORDER BY Genre desc;
> ```

>[!note] Data outside the query result. 
>You can order by data not shown in a query result, meaning that if you want to order by price but only show the artist and the CD then you can. 

---
date: [Fri 13/05 2022]
aliases: [database, SQL ]
tags: [GR10/Q2 code/data-handling]
modified: Thu 03/11 2022 08:00
---
# Databases And SQL
## Definitions
**SQL**: Structured Query Language

**Database**: a collection of related information about a subject organised in a useful manner. 

**DBMS (DataBase Management System)**: a set of programs to create a database

### Prefixes
- **tbl** – table
- **frm** – form
- **qry** – query
- **rpt** – report

## Purpose of a DBMS
a DBMS is a set of programs to create a database containing collections of related information organised in a useful manner. 

A good DBMS should:
- avoid duplication of data
- provide consistent data
- be accessible across a network for multiple users

## Database Concepts
We look at the following parts of a database:
- **Schema** – the logical structure of the database
- **Fields** – single data items with a type
- **Records** – collections of fields, represented as rows in a table
- **Primary key** – uniquely identifies a record
- **Tables** – collections of records
- **Databases** – collection of tables

### Schema
a DBMS has a *schema*, which is a ‘skeleton’ that makes up the *logical structure* of the database. it defines how data should be organised in tables, and how those tables should like to form relationships.

### Fields, Records, and tables
The simplest entity in a database is a *field*. Fields store a *single* data item. Fields exist in *columns* in a *table*. Each field has a *data type* assigned to it. When many fields are grouped, they form a *record*. For instance, all the data about one person would be stored in a single record and be stored as the *rows* of a table. 

### Primary keys
The *primary key* of a record is a type of field that *uniquely identifies each record* in the table. 

[[SQL]]
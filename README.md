# Java SQL

A student that completes this project shows that they can:

- Query data from a single table
- Query data from multiple tables
- Create a new database using PostgreSQL

## Introduction

Working with SQL

## Instructions

Reimport the Northwind database into PostgreSQL using pgAdmin. This is the same data we used during the guided project.

- [ ] **_pgAdmin data refresh_**

- Select the northwind database created during the guided project.

- Tools -> Query Tool

  - Open file northwind.sql (you used this script during the guided project)
  - Execute

- Look under

  - northwind -> Schemas -> public -> tables

- Clear query windows

### Answer the following data queries. Keep track of the SQL you write by pasting it into this document under its appropriate header below in the provided SQL code block. You will be submitting that through the regular fork, change, pull process

- [x] **_find all customers that live in London. Returns 6 records_**

  <details><summary>hint</summary>

  - This can be done with SELECT and WHERE clauses
  </details>

```SQL
{"AROUT"	"Around the Horn"	"Thomas Hardy"	"Sales Representative"	"120 Hanover Sq."	"London"		"WA1 1DP"	"UK"	"(171) 555-7788"	"(171) 555-6750"}

{"BSBEV"	"B's Beverages"	"Victoria Ashworth"	"Sales Representative"	"Fauntleroy Circus"	"London"		"EC2 5NT"	"UK"	"(171) 555-1212"}

{"CONSH"	"Consolidated Holdings"	"Elizabeth Brown"	"Sales Representative"	"Berkeley Gardens 12  Brewery"	"London"		"WX1 6LT"	"UK"	"(171) 555-2282"	"(171) 555-9199"}

{"EASTC"	"Eastern Connection"	"Ann Devon"	"Sales Agent"	"35 King George"	"London"		"WX3 6FW"	"UK"	"(171) 555-0297"	"(171) 555-3373"}

{"NORTS"	"North/South"	"Simon Crowther"	"Sales Associate"	"South House 300 Queensbridge"	"London"		"SW7 1RZ"	"UK"	"(171) 555-7733"	"(171) 555-2530"}

{"SEVES"	"Seven Seas Imports"	"Hari Kumar"	"Sales Manager"	"90 Wadhurst Rd."	"London"		"OX15 4NB"	"UK"	"(171) 555-1717"	"(171) 555-5646"}

```

- [x] **_find all customers with postal code 1010. Returns 3 customers_**

  <details><summary>hint</summary>

  - This can be done with SELECT and WHERE clauses
  </details>

```SQL
{"CACTU"	"Cactus Comidas para llevar"	"Patricio Simpson"	"Sales Agent"	"Cerrito 333"	"Buenos Aires"		"1010"	"Argentina"	"(1) 135-5555"	"(1) 135-4892"}

{"OCEAN"	"Océano Atlántico Ltda."	"Yvonne Moncada"	"Sales Agent"	"Ing. Gustavo Moncada 8585 Piso 20-A"	"Buenos Aires"		"1010"	"Argentina"	"(1) 135-5333"	"(1) 135-5535"}

{"RANCH"	"Rancho grande"	"Sergio Gutiérrez"	"Sales Representative"	"Av. del Libertador 900"	"Buenos Aires"		"1010"	"Argentina"	"(1) 123-5555"	"(1) 123-5556"}
```

- [ ] **_find the phone number for the supplier with the id 11. Should be (010) 9984510_**

  <details><summary>hint</summary>

  - This can be done with SELECT and WHERE clauses
  </details>

```SQL

```

- [ ] **_list orders descending by the order date. The order with date 1998-05-06 should be at the top_**

  <details><summary>hint</summary>

  - This can be done with SELECT, WHERE, and ORDER BY clauses
  </details>

```SQL

```

- [ ] **_find all suppliers who have names longer than 20 characters. Returns 11 records_**

  <details><summary>hint</summary>

  - This can be done with SELECT and WHERE clauses
  - You can use `length(company_name)` to get the length of the name
  </details>

```SQL

```

- [ ] **_find all customers that include the word 'MARKET' in the contact title. Should return 19 records_**

  <details><summary>hint</summary>

  - This can be done with SELECT and a WHERE clause using the LIKE keyword
  - Don't forget the wildcard '%' symbols at the beginning and end of your substring to denote it can appear anywhere in the string in question
  - Remember to convert your contact title to all upper case for case insensitive comparing so upper(contact_title)
  </details>

```SQL

```

- [ ] **_add a customer record for_**
- customer id is 'SHIRE'
- company name is 'The Shire'
- contact name is 'Bilbo Baggins'
- the address is '1 Hobbit-Hole'
- the city is 'Bag End'
- the postal code is '111'
- the country is 'Middle Earth'
  <details><summary>hint</summary>

  - This can be done with the INSERT INTO clause
  </details>

```SQL

```

- [ ] **_update *Bilbo Baggins* record so that the postal code changes to *"11122"*_**

  <details><summary>hint</summary>

  - This can be done with UPDATE and WHERE clauses
  </details>

```SQL

```

- [ ] **_list orders grouped and ordered by customer company name showing the number of orders per customer company name. *Rattlesnake Canyon Grocery* should have 18 orders_**

  <details><summary>hint</summary>

  - This can be done with SELECT, COUNT, JOIN and GROUP BY clauses. Your count should focus on a field in the Orders table, not the Customer table
  - There is more information about the COUNT clause on [W3 Schools](https://www.w3schools.com/sql/sql_count_avg_sum.asp)
  </details>

```SQL

```

- [ ] **_list customers by contact name and the number of orders per contact name. Sort the list by the number of orders in descending order. *Jose Pavarotti* should be at the top with 31 orders followed by *Roland Mendal* with 30 orders. Last should be *Francisco Chang* with 1 order_**

  <details><summary>hint</summary>

  - This can be done by adding an ORDER BY clause to the previous answer and changing the group by field
  </details>

```SQL

```

- [ ] **_list orders grouped by customer's city showing the number of orders per city. Returns 69 Records with *Aachen* showing 6 orders and *Albuquerque* showing 18 orders_**

  <details><summary>hint</summary>

  - This is very similar to the previous two queries, however, it focuses on the City rather than the Customer Names
  </details>

```SQL

```

## Data Normalization

Note: This step does not use PostgreSQL!

- [ ] **_Take the following data and normalize it into a 3NF database_**

| Person Name | Pet Name | Pet Type | Pet Name 2 | Pet Type 2 | Pet Name 3 | Pet Type 3 | Fenced Yard | City Dweller |
| ----------- | -------- | -------- | ---------- | ---------- | ---------- | ---------- | ----------- | ------------ |
| Jane        | Ellie    | Dog      | Tiger      | Cat        | Toby       | Turtle     | No          | Yes          |
| Bob         | Joe      | Horse    |            |            |            |            | No          | No           |
| Sam         | Ginger   | Dog      | Miss Kitty | Cat        | Bubble     | Fish       | Yes         | No           |

Below are some empty tables to be used to normalize the database

- Not all of the cells will contain data in the final solution
- Feel free to edit these tables as necessary

Table Name:

|     |     |     |     |     |     |     |     |     |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
|     |     |     |     |     |     |     |     |     |
|     |     |     |     |     |     |     |     |     |
|     |     |     |     |     |     |     |     |     |
|     |     |     |     |     |     |     |     |     |
|     |     |     |     |     |     |     |     |     |
|     |     |     |     |     |     |     |     |     |
|     |     |     |     |     |     |     |     |     |

Table Name:

|     |     |     |     |     |     |     |     |     |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
|     |     |     |     |     |     |     |     |     |
|     |     |     |     |     |     |     |     |     |
|     |     |     |     |     |     |     |     |     |
|     |     |     |     |     |     |     |     |     |
|     |     |     |     |     |     |     |     |     |
|     |     |     |     |     |     |     |     |     |
|     |     |     |     |     |     |     |     |     |

Table Name:

|     |     |     |     |     |     |     |     |     |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
|     |     |     |     |     |     |     |     |     |
|     |     |     |     |     |     |     |     |     |
|     |     |     |     |     |     |     |     |     |
|     |     |     |     |     |     |     |     |     |
|     |     |     |     |     |     |     |     |     |
|     |     |     |     |     |     |     |     |     |
|     |     |     |     |     |     |     |     |     |

Table Name:

|     |     |     |     |     |     |     |     |     |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
|     |     |     |     |     |     |     |     |     |
|     |     |     |     |     |     |     |     |     |
|     |     |     |     |     |     |     |     |     |
|     |     |     |     |     |     |     |     |     |
|     |     |     |     |     |     |     |     |     |
|     |     |     |     |     |     |     |     |     |
|     |     |     |     |     |     |     |     |     |

---

### Stretch Goals

- [ ] **_delete all customers that have no orders. Should delete 2 (or 3 if you haven't deleted the record added) records_**

```SQL

```

- [ ] **_Create Database and Table: After creating the database, tables, columns, and constraint, generate the script necessary to recreate the database. This script is what you will submit for review_**

- use pgAdmin to create a database, naming it `budget`.
- add an `accounts` table with the following _schema_:

  - `id`, numeric value with no decimal places that should autoincrement.
  - `name`, string, add whatever is necessary to make searching by name faster.
  - `budget` numeric value.

- constraints
  - the `id` should be the primary key for the table.
  - account `name` should be unique.
  - account `budget` is required.

```SQL

```

To see the script

- Right Click on the database name
  - Select Backup...
    - Set a filename
      - To put the file backup.sql in your home directory, you could use `backup.sql`
    - Set format to `Plain`
- The script you want is now in the text file named above.
  - Copy the script from the text file into the SQL code block above!

![Database Script](assets/jx-12-m3-script.gif)

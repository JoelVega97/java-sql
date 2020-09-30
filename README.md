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

- [x] **_find the phone number for the supplier with the id 11. Should be (010) 9984510_**

  <details><summary>hint</summary>

  - This can be done with SELECT and WHERE clauses
  </details>

```SQL
{"(010) 9984510"}
```

- [x] **_list orders descending by the order date. The order with date 1998-05-06 should be at the top_**

  <details><summary>hint</summary>

  - This can be done with SELECT, WHERE, and ORDER BY clauses
  </details>

```SQL
"1998-05-06"
"1998-05-06"
"1998-05-06"
"1998-05-06"
"1998-05-05"
"1998-05-05"
"1998-05-05"
"1998-05-05"
"1998-05-04"
"1998-05-04"
"1998-05-04"
"1998-05-01"
"1998-05-01"
"1998-05-01"
"1998-04-30"
"1998-04-30"
"1998-04-30"
"1998-04-30"
"1998-04-29"
"1998-04-29"
"1998-04-29"
"1998-04-28"
"1998-04-28"
"1998-04-28"
"1998-04-27"
"1998-04-27"
"1998-04-27"
"1998-04-27"
"1998-04-24"
"1998-04-24"
"1998-04-24"
"1998-04-23"
"1998-04-23"
"1998-04-23"
"1998-04-22"
"1998-04-22"
"1998-04-22"
"1998-04-22"
"1998-04-21"
"1998-04-21"
"1998-04-21"
"1998-04-20"
"1998-04-20"
"1998-04-20"
"1998-04-17"
"1998-04-17"
"1998-04-17"
"1998-04-17"
"1998-04-16"
"1998-04-16"
"1998-04-16"
"1998-04-15"
"1998-04-15"
"1998-04-15"
"1998-04-14"
"1998-04-14"
"1998-04-14"
"1998-04-14"
"1998-04-13"
"1998-04-13"
"1998-04-13"
"1998-04-10"
"1998-04-10"
"1998-04-10"
"1998-04-09"
"1998-04-09"
"1998-04-09"
"1998-04-09"
"1998-04-08"
"1998-04-08"
"1998-04-08"
"1998-04-07"
"1998-04-07"
"1998-04-07"
"1998-04-06"
"1998-04-06"
"1998-04-06"
"1998-04-06"
"1998-04-03"
"1998-04-03"
"1998-04-03"
"1998-04-02"
"1998-04-02"
"1998-04-02"
"1998-04-01"
"1998-04-01"
"1998-04-01"
"1998-04-01"
"1998-03-31"
"1998-03-31"
"1998-03-31"
"1998-03-30"
"1998-03-30"
"1998-03-30"
"1998-03-27"
"1998-03-27"
"1998-03-27"
"1998-03-27"
"1998-03-26"
"1998-03-26"
"1998-03-26"
"1998-03-25"
"1998-03-25"
"1998-03-25"
"1998-03-24"
"1998-03-24"
"1998-03-24"
"1998-03-24"
"1998-03-23"
"1998-03-23"
"1998-03-23"
"1998-03-20"
"1998-03-20"
"1998-03-20"
"1998-03-19"
"1998-03-19"
"1998-03-19"
"1998-03-19"
"1998-03-18"
"1998-03-18"
"1998-03-18"
"1998-03-17"
"1998-03-17"
"1998-03-17"
"1998-03-16"
"1998-03-16"
"1998-03-16"
"1998-03-16"
"1998-03-13"
"1998-03-13"
"1998-03-13"
"1998-03-12"
"1998-03-12"
"1998-03-12"
"1998-03-11"
"1998-03-11"
"1998-03-11"
"1998-03-11"
"1998-03-10"
"1998-03-10"
"1998-03-10"
"1998-03-09"
"1998-03-09"
"1998-03-09"
"1998-03-06"
"1998-03-06"
"1998-03-06"
"1998-03-06"
"1998-03-05"
"1998-03-05"
"1998-03-05"
"1998-03-04"
"1998-03-04"
"1998-03-04"
"1998-03-03"
"1998-03-03"
"1998-03-03"
"1998-03-03"
"1998-03-02"
"1998-03-02"
"1998-03-02"
"1998-02-27"
"1998-02-27"
"1998-02-27"
"1998-02-26"
"1998-02-26"
"1998-02-26"
"1998-02-26"
"1998-02-26"
"1998-02-26"
"1998-02-25"
"1998-02-25"
"1998-02-24"
"1998-02-24"
"1998-02-24"
"1998-02-23"
"1998-02-23"
"1998-02-20"
"1998-02-20"
"1998-02-20"
"1998-02-19"
"1998-02-19"
"1998-02-18"
"1998-02-18"
"1998-02-18"
"1998-02-17"
"1998-02-17"
"1998-02-16"
"1998-02-16"
"1998-02-16"
"1998-02-13"
"1998-02-13"
"1998-02-12"
"1998-02-12"
"1998-02-12"
"1998-02-11"
"1998-02-11"
"1998-02-10"
"1998-02-10"
"1998-02-10"
"1998-02-09"
"1998-02-09"
"1998-02-06"
"1998-02-06"
"1998-02-06"
"1998-02-05"
"1998-02-05"
"1998-02-04"
"1998-02-04"
"1998-02-04"
"1998-02-03"
"1998-02-03"
"1998-02-02"
"1998-02-02"
"1998-02-02"
"1998-01-30"
"1998-01-30"
"1998-01-29"
"1998-01-29"
"1998-01-29"
"1998-01-28"
"1998-01-28"
"1998-01-27"
"1998-01-27"
"1998-01-27"
"1998-01-26"
"1998-01-26"
"1998-01-23"
"1998-01-23"
"1998-01-23"
"1998-01-22"
"1998-01-22"
"1998-01-21"
"1998-01-21"
"1998-01-21"
"1998-01-20"
"1998-01-20"
"1998-01-19"
"1998-01-19"
"1998-01-19"
"1998-01-16"
"1998-01-16"
"1998-01-15"
"1998-01-15"
"1998-01-15"
"1998-01-14"
"1998-01-14"
"1998-01-13"
"1998-01-13"
"1998-01-13"
"1998-01-12"
"1998-01-12"
"1998-01-09"
"1998-01-09"
"1998-01-09"
"1998-01-08"
"1998-01-08"
"1998-01-07"
"1998-01-07"
"1998-01-07"
"1998-01-06"
"1998-01-06"
"1998-01-05"
"1998-01-05"
"1998-01-05"
"1998-01-02"
"1998-01-02"
"1998-01-01"
"1998-01-01"
"1998-01-01"
"1997-12-31"
"1997-12-31"
"1997-12-30"
"1997-12-30"
"1997-12-30"
"1997-12-29"
"1997-12-29"
"1997-12-26"
"1997-12-26"
"1997-12-26"
"1997-12-25"
"1997-12-25"
"1997-12-24"
"1997-12-24"
"1997-12-24"
"1997-12-23"
"1997-12-23"
"1997-12-22"
"1997-12-22"
"1997-12-22"
"1997-12-19"
"1997-12-19"
"1997-12-18"
"1997-12-18"
"1997-12-18"
"1997-12-17"
"1997-12-17"
"1997-12-16"
"1997-12-16"
"1997-12-16"
"1997-12-15"
"1997-12-15"
"1997-12-12"
"1997-12-11"
"1997-12-11"
"1997-12-10"
"1997-12-10"
"1997-12-09"
"1997-12-08"
"1997-12-08"
"1997-12-05"
"1997-12-05"
"1997-12-04"
"1997-12-03"
"1997-12-03"
"1997-12-02"
"1997-12-02"
"1997-12-01"
"1997-11-28"
"1997-11-28"
"1997-11-27"
"1997-11-27"
"1997-11-26"
"1997-11-25"
"1997-11-25"
"1997-11-24"
"1997-11-24"
"1997-11-21"
"1997-11-20"
"1997-11-20"
"1997-11-19"
"1997-11-19"
"1997-11-18"
"1997-11-17"
"1997-11-17"
"1997-11-14"
"1997-11-14"
"1997-11-13"
"1997-11-12"
"1997-11-12"
"1997-11-11"
"1997-11-11"
"1997-11-10"
"1997-11-07"
"1997-11-07"
"1997-11-06"
"1997-11-06"
"1997-11-05"
"1997-11-04"
"1997-11-04"
"1997-11-03"
"1997-11-03"
"1997-10-31"
"1997-10-30"
"1997-10-30"
"1997-10-29"
"1997-10-29"
"1997-10-28"
"1997-10-27"
"1997-10-27"
"1997-10-24"
"1997-10-24"
"1997-10-23"
"1997-10-22"
"1997-10-22"
"1997-10-21"
"1997-10-21"
"1997-10-20"
"1997-10-17"
"1997-10-17"
"1997-10-16"
"1997-10-16"
"1997-10-15"
"1997-10-14"
"1997-10-14"
"1997-10-13"
"1997-10-13"
"1997-10-10"
"1997-10-09"
"1997-10-09"
"1997-10-08"
"1997-10-08"
"1997-10-07"
"1997-10-06"
"1997-10-06"
"1997-10-03"
"1997-10-03"
"1997-10-02"
"1997-10-01"
"1997-10-01"
"1997-09-30"
"1997-09-30"
"1997-09-29"
"1997-09-26"
"1997-09-26"
"1997-09-25"
"1997-09-25"
"1997-09-24"
"1997-09-23"
"1997-09-23"
"1997-09-22"
"1997-09-22"
"1997-09-19"
"1997-09-18"
"1997-09-18"
"1997-09-17"
"1997-09-17"
"1997-09-16"
"1997-09-15"
"1997-09-15"
"1997-09-12"
"1997-09-12"
"1997-09-11"
"1997-09-10"
"1997-09-10"
"1997-09-09"
"1997-09-09"
"1997-09-08"
"1997-09-05"
"1997-09-05"
"1997-09-04"
"1997-09-04"
"1997-09-03"
"1997-09-02"
"1997-09-02"
"1997-09-01"
"1997-09-01"
"1997-08-29"
"1997-08-28"
"1997-08-28"
"1997-08-27"
"1997-08-27"
"1997-08-26"
"1997-08-25"
"1997-08-25"
"1997-08-22"
"1997-08-22"
"1997-08-21"
"1997-08-20"
"1997-08-20"
"1997-08-19"
"1997-08-19"
"1997-08-18"
"1997-08-15"
"1997-08-15"
"1997-08-14"
"1997-08-14"
"1997-08-13"
"1997-08-12"
"1997-08-12"
"1997-08-11"
"1997-08-11"
"1997-08-08"
"1997-08-07"
"1997-08-07"
"1997-08-06"
"1997-08-05"
"1997-08-05"
"1997-08-04"
"1997-08-01"
"1997-07-31"
"1997-07-31"
"1997-07-30"
"1997-07-29"
"1997-07-29"
"1997-07-28"
"1997-07-25"
"1997-07-25"
"1997-07-24"
"1997-07-23"
"1997-07-22"
"1997-07-22"
"1997-07-21"
"1997-07-18"
"1997-07-18"
"1997-07-17"
"1997-07-16"
"1997-07-16"
"1997-07-15"
"1997-07-14"
"1997-07-11"
"1997-07-11"
"1997-07-10"
"1997-07-09"
"1997-07-09"
"1997-07-08"
"1997-07-07"
"1997-07-07"
"1997-07-04"
"1997-07-03"
"1997-07-02"
"1997-07-02"
"1997-07-01"
"1997-06-30"
"1997-06-30"
"1997-06-27"
"1997-06-26"
"1997-06-26"
"1997-06-25"
"1997-06-24"
"1997-06-23"
"1997-06-23"
"1997-06-20"
"1997-06-19"
"1997-06-19"
"1997-06-18"
"1997-06-17"
"1997-06-17"
"1997-06-16"
"1997-06-13"
"1997-06-12"
"1997-06-12"
"1997-06-11"
"1997-06-10"
"1997-06-10"
"1997-06-09"
"1997-06-06"
"1997-06-06"
"1997-06-05"
"1997-06-04"
"1997-06-03"
"1997-06-03"
"1997-06-02"
"1997-05-30"
"1997-05-30"
"1997-05-29"
"1997-05-28"
"1997-05-28"
"1997-05-27"
"1997-05-26"
"1997-05-23"
"1997-05-23"
"1997-05-22"
"1997-05-21"
"1997-05-21"
"1997-05-20"
"1997-05-19"
"1997-05-19"
"1997-05-16"
"1997-05-15"
"1997-05-14"
"1997-05-14"
"1997-05-13"
"1997-05-12"
"1997-05-12"
"1997-05-09"
"1997-05-08"
"1997-05-08"
"1997-05-07"
"1997-05-06"
"1997-05-05"
"1997-05-05"
"1997-05-02"
"1997-05-01"
"1997-05-01"
"1997-04-30"
"1997-04-29"
"1997-04-29"
"1997-04-28"
"1997-04-25"
"1997-04-24"
"1997-04-24"
"1997-04-23"
"1997-04-22"
"1997-04-22"
"1997-04-21"
"1997-04-18"
"1997-04-18"
"1997-04-17"
"1997-04-16"
"1997-04-15"
"1997-04-15"
"1997-04-14"
"1997-04-11"
"1997-04-11"
"1997-04-10"
"1997-04-09"
"1997-04-09"
"1997-04-08"
"1997-04-07"
"1997-04-04"
"1997-04-04"
"1997-04-03"
"1997-04-02"
"1997-04-02"
"1997-04-01"
"1997-03-31"
"1997-03-31"
"1997-03-28"
"1997-03-27"
"1997-03-26"
"1997-03-26"
"1997-03-25"
"1997-03-24"
"1997-03-24"
"1997-03-21"
"1997-03-20"
"1997-03-20"
"1997-03-19"
"1997-03-18"
"1997-03-17"
"1997-03-17"
"1997-03-14"
"1997-03-13"
"1997-03-13"
"1997-03-12"
"1997-03-11"
"1997-03-11"
"1997-03-10"
"1997-03-07"
"1997-03-06"
"1997-03-06"
"1997-03-05"
"1997-03-04"
"1997-03-04"
"1997-03-03"
"1997-02-28"
"1997-02-28"
"1997-02-27"
"1997-02-26"
"1997-02-25"
"1997-02-25"
"1997-02-24"
"1997-02-21"
"1997-02-21"
"1997-02-20"
"1997-02-19"
"1997-02-19"
"1997-02-18"
"1997-02-17"
"1997-02-14"
"1997-02-14"
"1997-02-13"
"1997-02-12"
"1997-02-12"
"1997-02-11"
"1997-02-10"
"1997-02-10"
"1997-02-07"
"1997-02-06"
"1997-02-05"
"1997-02-05"
"1997-02-04"
"1997-02-03"
"1997-02-03"
"1997-01-31"
"1997-01-30"
"1997-01-30"
"1997-01-29"
"1997-01-28"
"1997-01-27"
"1997-01-27"
"1997-01-24"
"1997-01-23"
"1997-01-23"
"1997-01-22"
"1997-01-21"
"1997-01-21"
"1997-01-20"
"1997-01-17"
"1997-01-16"
"1997-01-16"
"1997-01-15"
"1997-01-14"
"1997-01-14"
"1997-01-13"
"1997-01-10"
"1997-01-10"
"1997-01-09"
"1997-01-08"
"1997-01-07"
"1997-01-07"
"1997-01-06"
"1997-01-03"
"1997-01-03"
"1997-01-02"
"1997-01-01"
"1997-01-01"
"1996-12-31"
"1996-12-30"
"1996-12-27"
"1996-12-27"
"1996-12-26"
"1996-12-25"
"1996-12-25"
"1996-12-24"
"1996-12-23"
"1996-12-23"
"1996-12-20"
"1996-12-19"
"1996-12-18"
"1996-12-18"
"1996-12-17"
"1996-12-16"
"1996-12-16"
"1996-12-13"
"1996-12-12"
"1996-12-12"
"1996-12-11"
"1996-12-10"
"1996-12-09"
"1996-12-09"
"1996-12-06"
"1996-12-05"
"1996-12-05"
"1996-12-04"
"1996-12-03"
"1996-12-03"
"1996-12-02"
"1996-11-29"
"1996-11-28"
"1996-11-28"
"1996-11-27"
"1996-11-26"
"1996-11-26"
"1996-11-25"
"1996-11-22"
"1996-11-22"
"1996-11-21"
"1996-11-20"
"1996-11-19"
"1996-11-18"
"1996-11-15"
"1996-11-14"
"1996-11-13"
"1996-11-12"
"1996-11-11"
"1996-11-11"
"1996-11-08"
"1996-11-07"
"1996-11-06"
"1996-11-05"
"1996-11-04"
"1996-11-01"
"1996-10-31"
"1996-10-30"
"1996-10-29"
"1996-10-29"
"1996-10-28"
"1996-10-25"
"1996-10-24"
"1996-10-23"
"1996-10-22"
"1996-10-21"
"1996-10-18"
"1996-10-17"
"1996-10-16"
"1996-10-16"
"1996-10-15"
"1996-10-14"
"1996-10-11"
"1996-10-10"
"1996-10-09"
"1996-10-08"
"1996-10-07"
"1996-10-04"
"1996-10-03"
"1996-10-03"
"1996-10-02"
"1996-10-01"
"1996-09-30"
"1996-09-27"
"1996-09-26"
"1996-09-25"
"1996-09-24"
"1996-09-23"
"1996-09-20"
"1996-09-20"
"1996-09-19"
"1996-09-18"
"1996-09-17"
"1996-09-16"
"1996-09-13"
"1996-09-12"
"1996-09-11"
"1996-09-10"
"1996-09-09"
"1996-09-09"
"1996-09-06"
"1996-09-05"
"1996-09-04"
"1996-09-03"
"1996-09-02"
"1996-08-30"
"1996-08-29"
"1996-08-28"
"1996-08-27"
"1996-08-27"
"1996-08-26"
"1996-08-23"
"1996-08-22"
"1996-08-21"
"1996-08-20"
"1996-08-19"
"1996-08-16"
"1996-08-15"
"1996-08-14"
"1996-08-14"
"1996-08-13"
"1996-08-12"
"1996-08-09"
"1996-08-08"
"1996-08-07"
"1996-08-06"
"1996-08-05"
"1996-08-02"
"1996-08-01"
"1996-08-01"
"1996-07-31"
"1996-07-30"
"1996-07-29"
"1996-07-26"
"1996-07-25"
"1996-07-24"
"1996-07-23"
"1996-07-22"
"1996-07-19"
"1996-07-19"
"1996-07-18"
"1996-07-17"
"1996-07-16"
"1996-07-15"
"1996-07-12"
"1996-07-11"
"1996-07-10"
"1996-07-09"
"1996-07-08"
"1996-07-08"
"1996-07-05"
"1996-07-04"
```

- [x] **_find all suppliers who have names longer than 20 characters. Returns 11 records_**

  <details><summary>hint</summary>

  - This can be done with SELECT and WHERE clauses
  - You can use `length(company_name)` to get the length of the name
  </details>

```SQL
{"New Orleans Cajun Delights"}
{"Grandma Kelly's Homestead"}
{"Cooperativa de Quesos 'Las Cabras'"}
{"Specialty Biscuits, Ltd."}
{"Refrescos Americanas LTDA"}
{"Heli Süßwaren GmbH & Co. KG"}
{"Plutzer Lebensmittelgroßmärkte AG"}
{"Nord-Ost-Fisch Handelsgesellschaft mbH"}
{"Formaggi Fortini s.r.l."}
{"Aux joyeux ecclésiastiques"}
{"New England Seafood Cannery"}
```

- [x] **_find all customers that include the word 'MARKET' in the contact title. Should return 19 records_**

  <details><summary>hint</summary>

  - This can be done with SELECT and a WHERE clause using the LIKE keyword
  - Don't forget the wildcard '%' symbols at the beginning and end of your substring to denote it can appear anywhere in the string in question
  - Remember to convert your contact title to all upper case for case insensitive comparing so upper(contact_title)
  </details>

```SQL
{"BLONP"	"Blondesddsl père et fils"	"Frédérique Citeaux"	"Marketing Manager"	"24, place Kléber"	"Strasbourg"		"67000"	"France"	"88.60.15.31"	"88.60.15.32"}

{"CENTC"	"Centro comercial Moctezuma"	"Francisco Chang"	"Marketing Manager"	"Sierras de Granada 9993"	"México D.F."		"05022"	"Mexico"	"(5) 555-3392"	"(5) 555-7293"}

{"FAMIA"	"Familia Arquibaldo"	"Aria Cruz"	"Marketing Assistant"	"Rua Orós, 92"	"Sao Paulo"	"SP"	"05442-030"	"Brazil"	"(11) 555-9857"	}

{"FRANK"	"Frankenversand"	"Peter Franken"	"Marketing Manager"	"Berliner Platz 43"	"München"		"80805"	"Germany"	"089-0877310"	"089-0877451"}

{"FRANR"	"France restauration"	"Carine Schmitt"	"Marketing Manager"	"54, rue Royale"	"Nantes"		"44000"	"France"	"40.32.21.21"	"40.32.21.20"}

{"GALED"	"Galería del gastrónomo"	"Eduardo Saavedra"	"Marketing Manager"	"Rambla de Cataluña, 23"	"Barcelona"		"08022"	"Spain"	"(93) 203 4560"	"(93) 203 4561"}

{"GREAL"	"Great Lakes Food Market"	"Howard Snyder"	"Marketing Manager"	"2732 Baker Blvd."	"Eugene"	"OR"	"97403"	"USA"	"(503) 555-7555"	}

{"ISLAT"	"Island Trading"	"Helen Bennett"	"Marketing Manager"	"Garden House Crowther Way"	"Cowes"	"Isle of Wight"	"PO31 7PJ"	"UK"	"(198) 555-8888"}

{"LAUGB"	"Laughing Bacchus Wine Cellars"	"Yoshi Tannamuri"	"Marketing Assistant"	"1900 Oak St."	"Vancouver"	"BC"	"V3F 2K1"	"Canada"	"(604) 555-3392"	"(604) 555-7293"
"LAZYK"	"Lazy K Kountry Store"	"John Steel"	"Marketing Manager"	"12 Orchestra Terrace"	"Walla Walla"	"WA"	"99362"	"USA"	"(509) 555-7969"	"(509) 555-6221"}

{"MAGAA"	"Magazzini Alimentari Riuniti"	"Giovanni Rovelli"	"Marketing Manager"	"Via Ludovico il Moro 22"	"Bergamo"		"24100"	"Italy"	"035-640230"	"035-640231"}

{"MEREP"	"Mère Paillarde"	"Jean Fresnière"	"Marketing Assistant"	"43 rue St. Laurent"	"Montréal"	"Québec"	"H1J 1C3"	"Canada"	"(514) 555-8054"	"(514) 555-8055"}

{"MORGK"	"Morgenstern Gesundkost"	"Alexander Feuer"	"Marketing Assistant"	"Heerstr. 22"	"Leipzig"		"04179"	"Germany"	"0342-023176"	}

{"QUEEN"	"Queen Cozinha"	"Lúcia Carvalho"	"Marketing Assistant"	"Alameda dos Canàrios, 891"	"Sao Paulo"	"SP"	"05487-020"	"Brazil"	"(11) 555-1189"}

{"SPECD"	"Spécialités du monde"	"Dominique Perrier"	"Marketing Manager"	"25, rue Lauriston"	"Paris"		"75016"	"France"	"(1) 47.55.60.10"	"(1) 47.55.60.20"}

{"THEBI"	"The Big Cheese"	"Liz Nixon"	"Marketing Manager"	"89 Jefferson Way Suite 2"	"Portland"	"OR"	"97201"	"USA"	"(503) 555-3612"}

{"THECR"	"The Cracker Box"	"Liu Wong"	"Marketing Assistant"	"55 Grizzly Peak Rd."	"Butte"	"MT"	"59801"	"USA"	"(406) 555-5834"	"(406) 555-8083"}

{"TOMSP"	"Toms Spezialitäten"	"Karin Josephs"	"Marketing Manager"	"Luisenstr. 48"	"Münster"		"44087"	"Germany"	"0251-031259"	"0251-035695"}

{"WILMK"	"Wilman Kala"	"Matti Karttunen"	"Owner/Marketing Assistant"	"Keskuskatu 45"	"Helsinki"		"21240"	"Finland"	"90-224 8858"	"90-224 8858"}

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
{"SHIRE"	"The Shire"	"Bilbo Baggins"		"1 Hobbit-Hole"	"Bag End"	 "111"	"Middle Earth"}
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

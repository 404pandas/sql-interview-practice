# About mySQL

mySQL is an open source relational database management system that uses Structured Query Language

Cross platform (MacOS for this project)

"Relational Model"

Uses "tables" with "columns" and "rows"
Relational using "keys"

  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#databases">Databases</a></li>
    <li><a href="#views">Views</a></li>
    <li><a href="#tables">Tables</a></li>
    <li><a href="#rows">Rows</a></li>
    <li><a href="#columns">Columns</a></li>
    <li><a href="#keys">Keys</a></li>
  </ol>

## Databases

Contains tables

Statements available:

**-CREATE DATABASE** - Creates database with given name

Example: CREATE DATABASE IF NOT EXISTS dog_data

**-ALTER DATABASE** - Changes overall characteristics of a database

Example: ALTER DATABASE dog_data

**-DROP DATABASE** - Drops all tables in the database and deletes database

Example: DROP DATABASE IF EXISTS dog_data

## Views

Views are stored queries that when invoked product a result set

Statements available:

**-CREATE VIEW** - Creates a new view

Example: CREATE VIEW test.breeds AS SELECT \* FROM breed

**-ALTER VIEW** - Alters view

Example: ALTER VIEW test.breeds AS

**-DROP VIEW** - Removes one or more views

Example: DROP VIEW IF EXISTS test.breeds CASCADE

## Tables

Table names consist of two parts- a table prefix and the specific database name.

Statements available:

**-CREATE TABLE** - Creates table with a given name

Example: CREATE TABLE IF NOT EXISTS owners

**-ALTER TABLE** - Changes structure of a table (add or delete columns, create or destroy indexes, change type of columns, or rename columns)

Example: ALTER TABLE owners DROP COLUMN owner_last_name

**-RENAME TABLE** - Renames one or more tables

Example: ALTER TABLE owners TO dog_owners

**-TRUNCATE TABLE** - Empties table completely

Example: TRUNCATE TABLE dog_owners

**-DROP TABLE** - Removes one or more tables

Example: DROP TABLE IF EXISTS dog_owners

## Rows

Rows contain the data

Statements available:

**-DELETE** - Removes rows from a table

Example: DELETE FROM dog_owners WHERE owner_first_name = 'mary'

**-EXCEPT** - Limits the result from the first query block to those rows which are not found in the second

Example: TABLE breeds EXCEPT TABLE cross_breeds

**-IMPORT TABLE** - Imports tables

Example: IMPORT TABLE FROM sdi_file

**-INSERT** - Inserts data into rows

Example: INSERT INTO breeds VALUES('labrador', 'golden retriever')

**-LOAD DATA** - Reads rows from a text file into a table

Example: LOAD DATA INFILE '/dist/owners.txt' INTO TABLE dog_owners FIELDS TERMINATED BY ','

**-REPLACE** - Inserts data into row, but if old row has same value as new row, the old row is deleted

Example: REPLACE INTO dog_owners VALUES('husky', 'boxer', 'labrador')
_old labrador value will be deleted_

**-SELECT** - Retrieves rows selected from one or more tables

Example: SELECT dog_name FROM dogs

Example: SELECT CONCAT(owner_last_name', ',owner_first_name) AS full_owner_name from owner ORDERED BY full_name

**-TABLE** - Returns rows and columns of the named table

Example: TABLE dog_name ORDER BY first_name

**-UPDATE** - Modifies rows

Example: UPDATE owners SET dog_number = dog_number + 1

**-VALUES** - Returns a set of one or more rows as a table

Example: VALUES ROW("cossette", 11, '2012-12-15'),
-> ROW("nugget", 7, '2015-09-29')

## Columns

Columns specify the type of data

Statements available:

**-SHOW COLUMNS** - Displays information about the columns in a given table

Example: SHOW COLUMNS FROM breeds

## Keys

**PRI** - Column is PRIMARY KEY or is one of the columns in a multi-column PRIMARY KEY

**UNI** - Column is the first column of a UNIQUE index (UNIQUE index permits multiple NULL vaulues)

**MUL** - Column is the first column of a nonunique index in which multiple occurences of a given value are permitted within the column

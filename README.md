MySQL Cheetsheet
================

## Contents

  - [Database Related SQL commands](database.md)
    - [SHOW DATABASES](#show-databases)
    - [CREATE DATABASE \<database\>](#create-database-database)
    - [SELECT DATABASE()](#select-database)
    - [USE \<database\>](#use-database)
    - [DROP DATABASE \<database\>](#drop-database-database)

  - [Table Related SQL commands](table.md)
    - [SHOW TABLES](#show-tables)
    - [CREATE TABLE](#create-table)
    - [DESC \<table\>](#desc-table)
    - [ALTER TABLE \<table\> ADD \<column\>\<column definition\>](#alter-table-table-add-columncolumn-definition)
    - [ALTER TABLE \<table\> ADD FOREIGN KEY (\<field\>) references \<referenced table\>(\<referenced field\>)](#alter-table-table-add-foreign-key-field-references-referenced-tablereferenced-field)
    - [DROP TABLE \<table\>](#drop-table-table)

  - [Row/Record Related SQL commands](record.md)
    - [INSERT INTO \<table\> (\<field\>, \<field\>, ...) VALUES (\<value\>,\<value\>,...)](##insert-into-table-field-field--values-valuevalue)
    - [SELECT \<field\>,\<field\>,... FROM \<table\> WHERE \<conditions\>](#select-fieldfield-from-table-where-conditions)
    - [UPDATE \<table\> SET \<field\>='\<value\>'](#update-table-set-fieldvalue)
    - [DELETE FROM \<table\> WHERE \<conditions\>](#delete-from-table-where-conditions)
    - [SELECT \* FROM \<table\> JOIN \<another table\> ON \<conditionals\>](#select--from-table-join-another-table-on-conditionals)
    - [SELECT \* FROM \<table\> GROUP BY \<field\>](#select--from-table-group-by-field)
    - [SELECT \* FROM \<table\> ORDER BY \<field\>](#select--from-table-order-by-field)

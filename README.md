MySQL Cheetsheet
================

## Contents

  - [Database Related SQL commands](database.md)
    - [SHOW DATABASES](database.md#show-databases)
    - [CREATE DATABASE \<database\>](database.md#create-database-database)
    - [SELECT DATABASE()](database.md#select-database)
    - [USE \<database\>](database.md#use-database)
    - [DROP DATABASE \<database\>](database.md#drop-database-database)

  - [Table Related SQL commands](table.md)
    - [SHOW TABLES](table.md#show-tables)
    - [CREATE TABLE](table.md#create-table)
    - [DESC \<table\>](table.md#desc-table)
    - [ALTER TABLE \<table\> ADD \<column\>\<column definition\>](table.md#alter-table-table-add-columncolumn-definition)
    - [ALTER TABLE \<table\> ADD FOREIGN KEY (\<field\>) references \<referenced table\>(\<referenced field\>)](table.md#alter-table-table-add-foreign-key-field-references-referenced-tablereferenced-field)
    - [DROP TABLE \<table\>](table.md#drop-table-table)

  - [Row/Record Related SQL commands](record.md)
    - [INSERT INTO \<table\> (\<field\>, \<field\>, ...) VALUES (\<value\>,\<value\>,...)](record.md#insert-into-table-field-field--values-valuevalue)
    - [SELECT \<field\>,\<field\>,... FROM \<table\> WHERE \<conditions\>](record.md#select-fieldfield-from-table-where-conditions)
    - [UPDATE \<table\> SET \<field\>='\<value\>'](record.md#update-table-set-fieldvalue)
    - [DELETE FROM \<table\> WHERE \<conditions\>](record.md#delete-from-table-where-conditions)
    - [SELECT \* FROM \<table\> JOIN \<another table\> ON \<conditionals\>](record.md#select--from-table-join-another-table-on-conditionals)
    - [SELECT \* FROM \<table\> GROUP BY \<field\>](record.md#select--from-table-group-by-field)
    - [SELECT \* FROM \<table\> ORDER BY \<field\>](record.md#select--from-table-order-by-field)

  - [User Related SQL commands](user.md)
    - [CREATE USER](user.md#create-user)
    - [GRANT](user.md#grant)

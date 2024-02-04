### Table Related SQL commands

**SHOW TABLES**

Show a list of available tables.

**CREATE TABLE**

Create a table with specified format.

```sql
CREATE TABLE <table>(
<field><type><specification>,
<field><type><specification>,
<field><type><specification>,
...
);
```

The following creates a table `users`.

```sql
mysql> CREATE TABLE users(
    id INT AUTO_INCREMENT,
    name VARCHAR(191),
    PRIMARY KEY(id)
);
```

**DESC <table>**

Show the definition of the specified table.
The following describes the `users` table.

```sql
mysql> DESC users;
+-------+--------------+------+-----+---------+----------------+
| Field | Type         | Null | Key | Default | Extra          |
+-------+--------------+------+-----+---------+----------------+
| id    | int          | NO   | PRI | NULL    | auto_increment |
| name  | varchar(191) | YES  |     | NULL    |                |
+-------+--------------+------+-----+---------+----------------+
```

**ALTER TABLE <table> ADD <column><column definition>**

Update the specified table and add specified column(s).

```sql
mysql> ALTER TABLE users ADD company_id INT;
```

**ALTER TABLE <table> ADD FOREIGN KEY (<field>) references <referenced table>(<referenced field>)**

Update the specified table and add a foreign key.

```sql
mysql> ALTER TABLE users ADD foreign key (company_id) REFERENCES companies(id);
```

**DROP TABLE <table>**

Delete the specified table.
The following deletes the `users` table.

```sql
mysql> DROP TABLE users;
```


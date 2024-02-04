### Row Related SQL commands

**INSERT INTO <table> (<field>, <field>, ...) VALUES (<value>,<value>,...)**

Create a record and store it in the specified table.

```sql
INSERT INTO users (name) VALUES ('Jane Doe');
```

**SELECT <field>,<field>,... FROM <table> WHERE <conditions>**

Show the values of the specified fields from the specified table which satisfies the conditions.

The following example shows values of every fields (specified by an asterisk `#`) whose `id` field is 12345 from the table `users`.

```sql
SELECT * FROM users;
```
```bash
+----+----------+
| id | name     |
+----+----------+
|  1 | Jane Doe |
+----+----------+
```

**UPDATE <table> SET <field>='<value>';**

Update the specified field value of the specified table.
The following sets the `name` field as `Jane J Doe` of a row whose `id` is 1.

```sql
UPDATE users SET name='Jane J Doe' WHERE id=1;
```

**DELETE FROM <table> WHERE <conditions>**

Delete the rows that matches the conditions.
The following deletes the row whose `id` is 1.

```sql
DELETE FROM users WHERE id=1;
```

**SELECT \* FROM <table> JOIN <another table> ON <conditionals>**

Perform join on the table with another table. By default, MySQL `JOIN` is `INNER JOIN`. For `LEFT JOIN`, `RIGHT JOIN`, or `CROSS JOIN` must be specified explicitly.
The following shows the user and the company name whose `users.company_id` matches the company `companies.id`.

```sql
SELECT users.name, companies.name FROM users JOIN companies ON users.company_id=companies.id;
```
```bash
+----------+-----------+
| name     | name      |
+----------+-----------+
| Jane Doe | Company A |
+----------+-----------+
```

**SELECT \* FROM <table> GROUP BY <field>**

Show summary rows that have the same values specified by `GROUP BY`.
The following shows the number of companies referred by the users table. The `AS` keyword creates an alias of the field.

```sql
SELECT COUNT(*) AS 'Number of Companies' FROM users GROUP BY company_id;
```
```bash
+---------------------+
| Number of Companies |
+---------------------+
|                   1 |
+---------------------+
```

**SELECT \* FROM <table> ORDER BY <field>**

Sort the rows by the specified field.
The following shows the records from the users table sorted by `id`.

```sql
SELECT * FROM users ORDER BY name;
```
```bash
+----+----------+---------+------------+
| id | name     | address | company_id |
+----+----------+---------+------------+
|  3 | Alan Doe | NULL    |       NULL |
|  2 | Jane Doe | NULL    |          1 |
|  4 | Zoe Doe  | NULL    |       NULL |
+----+----------+---------+------------+
```


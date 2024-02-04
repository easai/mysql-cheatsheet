### Database Related SQL commands

**SHOW DATABASES**

Show a list of available databases.
Example:

```sql
mysql> SHOW DATABASES;
+--------------------+
| Database           |
+--------------------+
| directory          |
+--------------------+
```

**CREATE DATABASE <database>**

Create a database.
The following creates a database named `directory`.

```sql
mysql> CREATE DATABASE directory;
```

**SELECT DATABASE()**

Show the selected database.

```sql
mysql> SELECT database();
+------------+
| database() |
+------------+
| directory  |
+------------+
```

**USE <database>**

Select database.
The following selects the `directory` database.

```sql
mysql> USE directory;
```

**DROP DATABASE <database>**

Delete the specified database.
The following deletes `directory` database.

```sql
mysql> DROP DATABASE directory;
```


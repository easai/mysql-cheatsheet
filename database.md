MySQL: Database Related commands
================================

## Contents

  - [SHOW DATABASES](#show-databases)
  - [CREATE DATABASE \<database\>](#create-database-database)
  - [SELECT DATABASE()](#select-database)
  - [USE \<database\>](#use-database)
  - [DROP DATABASE \<database\>](#drop-database-database)


## SHOW DATABASES

Show a list of available databases.<br />
Example:

```sql
SHOW DATABASES;
```
```bash
+--------------------+
| Database           |
+--------------------+
| directory          |
+--------------------+
```

## CREATE DATABASE \<database\>

Create a database.<br />
The following creates a database named `directory`.

```sql
CREATE DATABASE directory;
```

## SELECT DATABASE()

Show the selected database.

```sql
SELECT database();
```
```bash
+------------+
| database() |
+------------+
| directory  |
+------------+
```

## USE \<database\>

Select database.<br />
The following selects the `directory` database.

```sql
USE directory;
```

## DROP DATABASE \<database\>

Delete the specified database.<br />
The following deletes `directory` database.

```sql
DROP DATABASE directory;
```


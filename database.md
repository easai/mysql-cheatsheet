### Database Related SQL commands

**SHOW DATABASES**

Show a list of available databases.
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

**CREATE DATABASE <database>**

Create a database.
The following creates a database named `directory`.

```sql
CREATE DATABASE directory;
```

**SELECT DATABASE()**

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

**USE <database>**

Select database.
The following selects the `directory` database.

```sql
USE directory;
```

**DROP DATABASE <database>**

Delete the specified database.
The following deletes `directory` database.

```sql
DROP DATABASE directory;
```


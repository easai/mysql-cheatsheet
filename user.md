MySQL: User Related commands
================================

## Contents

  - [CREATE USER](#create-user)
  - [GRANT](#grant)


## CREATE USER

Create a user.<br />
Example:

```sql
create user roote@localhost identified by 'password';
```

## GRANT

Grant priviledges to a user.<br />
Example:

```sql
grant all on unguru.* to unguru@localhost;
```
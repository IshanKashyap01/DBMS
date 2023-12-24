# Transaction Control Language (TCL)

It is a subset of SQL, which is used to manage transactions in the database

## Keywords Used in TCL

### START TRANSACTION

It is used to initiate a transaction and has ```BEGIN``` as an alias

### COMMIT

- It is used to permanently store all the changes made before it in the database

- If the ```AUTOCOMMIT``` is turned on, every change will be automatically committed
to the database

```SQL
-- The value can be 0/OFF or 1/ON
SET AUTOCOMMIT = (value)
```

### SAVEPOINT

```SQL
SAVEPOINT s1;
```

It saves the current state of the database into a saving point that can be accessed
later in the transaction

### ROLLBACK

```SQL
-- To rollback to before the transaction
ROLLBACK
-- To rollback to a savepoint
ROLLBACK TO s1;
```

- It reverts all the changes made to the database during the transaction either to
the beginning or to a particular savepoint

- However, it cannot revert *committed* changes

### LOCK

- It is used to restrict access to tables during a transaction

- It requires the user to have the ```LOCK``` and ```SELECT``` privileges

- However, you can only unlock all tables at once in MySQL

```SQL
-- To prevent other sessions from writing until the lock is released
LOCK TABLE t1 READ;
-- To prevent other sessions from reading and writing the table
LOCK TABLE t1 WRITE;
-- To lock multiple tables at once
LOCK TABLES t1 READ, t2 WRITE,...;
-- To release locks
UNLOCK TABLES;
```

# Introduction to Transactions

A transaction is a logical unit of work which accesses and possibly modifies
the contents of a database

## Properties of a Transaction (ACID Properties)

### Atomicity

A transaction is an atomic unit of work that finishes completely or not at all

### Consistency

The database is consistent before and after the transaction i.e. *integrity*
*constraints* is maintained

### Isolation

- Multiple transactions can run concurrently but are isolated from each other

- The changes made during a transaction is made permanent *only after* the transaction
has completed

- Hence, a transactions will never overwrite/read changes made *during* each other's
execution

### Durability

Once, a transaction is finished, its effects are made permanent and are not lost
even in case of a system failure

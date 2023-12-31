# ACID Properties

Let's suppose there are two bank accounts A and B, both having Rs 500 in them.
A starts a transaction to send Rs 100 to B.

## Atomicity

- In case a failure occur after the amount is deducted from A but not credited to
B, the accounts should be unchanged

- That is, the transaction should be reverted/rolled back

## Consistency

- Both accounts' collective amount before and after the transaction and must remain
the same

- Hence, both accounts must still have a total of Rs 1000 after the transaction
is finished

## Isolation

- If more than one transaction concerns the same table(s), then they will affect
the database sequentially and not interfere with each other

- Suppose, A sends Rs 100 each to B and C at the same time w/o isolation

- A might end up with only Rs 100 deducted from his account as both will

## Durability

- Suppose, a system failure occurs as soon as the transaction is completed

- The transaction must persist after restoration

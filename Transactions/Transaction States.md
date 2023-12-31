# States of Transaction

## Active

When the first read/write operation of a transaction begins

## Partially Committed

When all read/write operations are finished in the main memory or local buffer

## Committed

If the **partially committed** state finishes with no errors and changes are persisted
without failure

## Failed

When any instruction like read/write operations or database persistence before
the **committed** state fails

## Aborted

If a transaction is failed, it will be aborted, i.e. it changes will be rolled back

## Terminated

End of the transaction's lifecycle after it is either aborted or committed

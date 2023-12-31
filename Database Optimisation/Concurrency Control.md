# Concurrency Control

Concurrency is when we perform two actions simultaneously or one after the other

## Lock Based Concurrency Control

- Once a request is made for a resource, it is locked for others until the current
transaction is finished with it

- However, there is a risk of deadlock in the system

## Timestamp Based Concurrency Control

- Transactions are served in a First Come First Serve basis as the timestamp at
which they enters the system is stored

- A newer transactions is not started until the previous is not completed

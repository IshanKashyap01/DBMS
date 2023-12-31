# Clustered Indexing

- A clustered index is formed on *ordered data files*

- The *search key* is not prime and may not even be unique or candidate key

- The *data reference* is a collection of all the rows grouped by the search key

- The data in the *disk itself* will be grouped w.r.t the search key

- Suppose, we have a relation ```Student (ID, course, phone, address)``` and ```course```
is used for indexing

- The table will be grouped in the disk w.r.t. ```course``` and each group will
have ```course``` as the *search key*

- This can make searching *very fast* as the database will search only in the respective
clusters rather than the whole table

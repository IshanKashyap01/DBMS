# Primary Indexing

- The **search key** in primary indexing is *always* the **primary key**

- The **data reference** will be a pointer to the *primary key*

## Dense Index

- *Each* primary key will have a corresponding search key

- This is *very fast* but will have a *heavy impact* on space

## Sparse Index

- Not all primary keys will have a corresponding search key however, table must
be sorted w.r.t. the search key

- This will save some space at the cost of speed

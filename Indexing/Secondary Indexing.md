# Secondary Indexing

- It is used to *reduce the load on primary index* when the relation grows too large
for the primary indexing to handle efficiently

- Secondary indexing adds an *extra layer* of indexing to primary indexing

- Each primary index will refer to a *range instead of a single key* and store
its *start* in data reference

- The *pointers to primary keys* will be stored by the secondary index instead

- The primary index will be in *RAM* and the secondary index will be in *ROM*

- The *secondary index* may also store its search key in *ranges*

## Example of Secondary Indexing

Suppose, we have 1000 primary keys and a request for 341 is made and the data is
divided ranges of 100 in primary and 10 in secondary index

- First, a value *just smaller* than 341 will be searched in the primary index (300)

- It will then go to 300 in the secondary index and search for the *closest* index
(340)

- Then, it will go to 340 in the *data block* and start search for 341 from 340

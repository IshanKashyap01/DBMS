# Partitioning & Sharding

## Partitioning

It is used for horizontal scaling by dividing the data into different servers

### Vertical Partitioning

It slices the tables into columns and stores them in different servers

### Horizontal Partitioning

It slices the rows and stores the table in multiple servers, each with different
set of rows

## Sharding

- A shard is just a slice of table from **horizontal partitioning**

- Large databases are partitioned into smaller, faster and more manageable shards

- These shards are all independent of each other

- Requests are sent only to the relevant shards improving performance and response
times

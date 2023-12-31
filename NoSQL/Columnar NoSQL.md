# Column Based/Columnar NoSQL Database

- Cell groups are *arranged in columns* unlike RDBMS, which stores data in rows

- All read/write operations are done in columns

- It has very fast aggregation hence, it is used for big data

- For ex. Hadoop HBase, Cassandra

- It has good compression hence, it is used for content management, blogging and
maintaining counters

- However, it is very difficult to write complex queries and extract rows by
connecting columns

- It also records the timestamp of when the records were added

- Row ID is used as a unique identifier

## How Data is Stored

Consider the following table in an RDBMS:

| S.No. |   Name    | Course |   Branch   | ID |
|-------|-----------|--------|------------|----|
| 01.   | Tanmay    | B-Tech | Computer   | 2  |
| 02.   | Abhishek  | B-Tech | Electronics| 5  |
| 03.   | Samriddha | B-Tech | IT         | 7  |
| 04.   | Aditi     | B-Tech | E & TC     | 8  |

It will be stored in a column based NoSQL database as follows:

| S.No. |   Name    | ID |
|-------|-----------|----|
| 01.   | Tanmay    | 2  |
| 02.   | Abhishek  | 5  |
| 03.   | Samriddha | 7  |
| 04.   | Aditi     | 8  |

| S.No. | Course | ID |
|-------|--------|----|
| 01.   | B-Tech | 2  |
| 02.   | B-Tech | 5  |
| 03.   | B-Tech | 7  |
| 04.   | B-Tech | 8  |

| S.No. |   Branch    | ID |
|-------|-------------|----|
| 01.   | Computer    | 2  |
| 02.   | Electronics | 5  |
| 03.   | IT          | 7  |
| 04.   | E & TC      | 8  |

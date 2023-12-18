# Inner Join

- It returns the *intersection* of the tables participating in the join

- If the common key has the same name in both the tables, it is also called a
**natural join**

```SQL
-- To retrieve some columns from both tables
SELECT 
    t1.c1 AS k1,
    ...,
    t2.c1 AS k2,
    ... 
FROM
    t1 INNER JOIN t2 ON k1 = k2
WHERE
    conditions;
-- To retrieve all columns from either tables
SELECT 
    t1.*,
    t2.c1 AS k2,
    ... 
FROM
    t1 INNER JOIN t2 ON t1.c1 = k2;
```

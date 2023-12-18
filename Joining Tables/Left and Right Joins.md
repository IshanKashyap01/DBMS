# Left & Right Joins

## Left Join

- It returns the *all* matches from the *left* table and the *intersection* of
both the tables

- It has almost same syntax as *inner join* except the join is named *left* instead
of *inner*

- Any unmatched values will be shown as *null* in the resultant join

```SQL
SELECT * FROM t1 LEFT JOIN t2 ON t1.c1 = t2.c2 WHERE conditions;
```

## Right Join

It is the same as *left* join except instead of  left table, it returns all matches
from the *right* table

```SQL
SELECT * FROM t1 RIGHT JOIN t2 ON t1.c1 = t2.c2 WHERE conditions;
```

## Using Multiple Joins

```SQL
-- inner join
SELECT * FROM t1 INNER JOIN t2 INNER JOIN t3 ON ... WHERE condtions;
--- other joins
SELECT
    ... 
FROM 
    t1 LEFT JOIN t2 ON ... 
    RIGHT JOIN t3 ON ... 
    INNER JOIN t4 ON ...
WHERE
    conditions;
```

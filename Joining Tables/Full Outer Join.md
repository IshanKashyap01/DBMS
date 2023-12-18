# Full Outer Join

- It returns the *union* of the tables participating in the join

- MySQL does not have a keyword for full outer join however, it can be emulated
via other joins

```SQL
-- removes duplicate rows
SELECT * FROM t1 LEFT JOIN t2 ON t1.c1 = t2.c2
UNION
SELECT * FROM t1 RIGHT JOIN t2 ON t1.c1 = t2.c2;
-- includes all duplicate rows
SELECT * FROM t1 LEFT JOIN t2 ON t1.c1 = t2.c2
UNION ALL
SELECT * FROM t1 RIGHT JOIN t2 ON t1.c1 = t2.c2;
```

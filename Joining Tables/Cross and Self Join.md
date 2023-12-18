# Cross & Self Join

## Cross Join

It returns the **cartesian product** of rows from the joined tables

```SQL
SELECT  * FROM t1 CROSS JOIN t2 WHERE conditions;
```

## Self Join

It joins the table with itself

```SQL
SELECT a1.c1, a2.c2 FROM t AS a1 INNER JOIN t AS a2 ON a1.c1 = a2.c1 WHERE conditions;
```

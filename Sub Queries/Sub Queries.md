# Introduction to Sub Queries

- A sub query is a query within a query and used as an alternate for joins

- It can be used with ```INSERT```, ```UPDATE```, ```DELETE``` and ```SELECT```

- However, the inner query cannot be an ```INSERT``` statement as does not return
a result set

## Types of Sub Queries

### Based on Clause

- The sub query can be placed in the ```WHERE```, ```FROM``` or ```SELECT``` clause

```SQL
SELECT (subquery1) FROM (subquery2) as t1 WHERE c1 IN (subquery3);
-- To check for existence of records
SELECT * FROM t1 WHERE EXISTS (subquery);
```

- In case of ```FROM```, the subquery's resultset will be stored as a temporary
table that must be given an alias

- This temporary table is called a **derived table**

### Result of Inner Query

Whether the inner query returns a single value or multiple values

### Dependency

- The inner query can run before or after the outer query

- It can be **nested** i.e. run *before* the outer query, which will use its output

- Or it can be **correlated** i.e. depend on the output of outer query for its
completion, i.e. run *after* the outer query

- A *correlated* subquery is performed on every row considered by the outer query

- It refers a column from the outer query making it dependent

```SQL
-- Nested Subquery
SELECT * FROM t1 WHERE (subquery);
-- Correlated Subquery
SELECT c1, c2 FROM t1 n WHERE c3 > (SELECT AVG(c3) FROM t1 WHERE c1 = n.c1);
```

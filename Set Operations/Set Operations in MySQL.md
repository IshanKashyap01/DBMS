# Set Operations in MySQL

## Union Set Operation

```SQL
-- To select all rows from both result sets without duplicates
SELECT * FROM t1
UNION
SELECT * FROM t2;
-- To select all rows from both result sets
SELECT * FROM t1
UNION ALL
SELECT * FROM t2;
```

## Intersection Set Operation

MySQL does not have the ```INTERSECT``` keyword, however, we can emulate it

```SQL
SELECT 
    DISTINCT c1
FROM
    t1 INNER JOIN t2 USING(c1);
```

## Minus Set Operation

MySQL does not have the ```MINUS``` keyword, however, it can be emulated

```SQL
SELECT id FROM t1 LEFT JOIN t2 USING(id) WHERE t2.id IS NULL;
```

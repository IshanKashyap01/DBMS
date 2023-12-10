# Filtering Data in MySQL

- Multiple conditions separated with **AND** and/or **OR** like:

    SELECT * FROM tb_1 WHERE c1 = 'x' AND c2 = 1 OR c3 = '1990-11-30'

- To find data between a range:

    SELECT * FROM tb_1 WHERE c2 BETWEEN 0 AND 1000;

- To find data with a set of values:

    SELECT * FROM tb_1 WHERE c1 IN ('x', 'y', 'z');

- To find all data not in a particular range or set:

    SELECT * FROM tb_1 WHERE c2 NOT BETWEEN 0 AND 1000;

    SELECT * FROM tb_1 WHERE c1 NOT IN ('x', 'y', 'z');

- To filter w.r.t. null values:

    SELECT * FROM tb_1 WHERE c1 IS NULL;

    SELECT * FROM tb_1 WHERE c2 IS NOT NULL;

- To filter data w.r.t. to likeness (**wildcard**):

    SELECT * FROM tb_1 WHERE c1 LIKE "x%" AND c2 LIKE "_y%"

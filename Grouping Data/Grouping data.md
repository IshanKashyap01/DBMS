# Grouping Data in MySQL

- The **GROUP BY** clause is used after the *WHERE* clause to group similar data
together like:

    SELECT * FROM tb_1 WHERE c1 = 'xyz' GROUP BY c1;

- However, the columns selected must be relevant to the *grouping*

- It can be used with *aggregate functions* such as:
  - SUM()
  - AVG()
  - COUNT()
  - MAX()
  - MIN()

    SELECT c1, AVG(c4) FROM tb_1 WHERE c1 = 'xyz' GROUP BY c1;

    SELECT c1, c2, AVG(c4) FROM tb_1 WHERE c1 = 'xyz' GROUP BY c1, c2;

- We can use *aliases* for columns by using the **AS** keyword such as:

    SELECT c1, AVG(c4) AS average_salary FROM tb_1 WHERE c1 = 'xyz' GROUP BY c1;

    SELECT c1, AVG(c4) AS 'Average Salary' FROM tb_1 WHERE c1 = 'xyz' GROUP BY c1;

- We can filter the *groups* by using the **HAVING** clause such as:

    SELECT c1, AVG(c4) FROM tb_1 GROUP BY c1 HAVING sum(c3) > 4000;

- We can also use **ORDER BY** with grouping, however, it must always come *after*
*GROUP BY* such as:

    SELECT c1, AVG(c4) FROM tb_1 WHERE c1 = 'xyz' GROUP BY c1 ORDER BY sum(c4);

- However, the column used in *ordering* must be a part of the *groups*

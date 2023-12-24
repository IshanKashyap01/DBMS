# Export Data from MySQL

```SQL
SELECT
    *
FROM
    table_name
INTO OUTFILE
    '<file_location>'
FIELDS
    ENCLOSED BY
        '"'
    TERMINATED BY
        ','
LINES
    TERMINATED BY
        '\n'
```

- The file is directly created by the MySQL server and must not already exist

- You must have the MYSQL FILE privilege to execute the above statement

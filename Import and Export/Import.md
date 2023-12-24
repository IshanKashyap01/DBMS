# Import External Data

```SQL
-- To import data from a .csv file
LOAD DATA [LOCAL] INFILE
    '<file_location/name>'
INTO TABLE
    table_name
FIELDS 
    TERMINATED BY
        ','
    -- Optional
    ENCLOSED BY
        '"'
LINES 
    TERMINATED BY
        '\n'
IGNORE 1 ROWS;
```

- In order to import data, the table schema must already be present in the database

- The columns and their order must be the same in the import file

- Use local if the file is present outside the server's folder otherwise, it will
not have the permission to access it

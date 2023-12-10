# Data Query Language

## Basic Select statement

- To select records from selected columns of a table:

    **SELECT** (column name), (column name)... (column name) **FROM** (table name);

- To select all records from a table:

    **SELECT * FROM** (table name);

- To filter records:

    **SELECT * FROM** (table name) **WHERE** (conditions)

- SELECT without the FROM clause:

    1. SELECT 100 - 1;
    2. SELECT UCASE("string");
    3. SELECT NOW();
    4. SELECT CURRENT_TIMESTAMP()
    5. SELECT CURRENT_TIMESTAMP(5)

**NOTE**: *the current_timestamp() function takes a parameter to specify precision*
*in milliseconds hence, the 5 above denotes the digits in millisecond*

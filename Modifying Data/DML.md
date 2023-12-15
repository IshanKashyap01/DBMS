# Data Manipulation Language (DML)

## Insert Command

    -- insert only in selected columns
    INSERT INTO table_name(column names) VALUES (row1), (row2)..., (rown);
    -- insert in all columns
    INSERT INTO table_name VALUES (row1), (row2),..., (rown);

## Update Command

    UPDATE table_name SET column_name = value WHERE conditions;
    UPDATE table_name SET column_name = value,..., column_name = value WHERE conditions;

## Delete Command

    DELETE FROM table_name WHERE conditions;
    -- Delete all records
    DELETE FROM table_name;
    -- Disable safe update mode
    SET SQL_SAFE_UPDATES = 0;
    -- Enable safe update mode
    SET SQL_SAFE_UPDATES = 1;

## Replace Command

    REPLACE INTO table_name(column_names) VALUES (row1),..., (rown);
    REPLACE INTO table_name SET column = value,... column = value WHERE conditions;

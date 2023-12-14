# Alter Operations

It is used to change the structure of the data

## Add

    ALTER TABLE table_name ADD 
        FIRST column_name data_type constraint,
        ...
        ...
        column_name data_type constraint AFTER column_name;

## Modify

    ALTER TABLE table_name MODIFY column_name data_type;

## Change Column

    ALTER TABLE table_name CHANGE COLUMN column_name new_name data_type;

## Drop

    ALTER TABLE table_name DROP COLUMN column_name, ..., column_name;

## Rename

    ALTER TABLE table_name RENAME TO new_name;

# Cascade

    CREATE TABLE table_name
    (
        ...
        FOREIGN KEY(key) REFERENCES table(column)
        ON DELETE CASCADE
        ON UPDATE CASCADE
    )
    CREATE TABLE table_name
    (
        ...
        FOREIGN KEY(key) REFERENCES table(column)
        ON DELETE SET NULL
    )

It defines what should be done to a child table, if a corresponding parent table
record is deleted or updated

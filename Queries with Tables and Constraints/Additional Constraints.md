# Additional Constraints

## Unique Key

    CREATE TABLE person
    (
        name VARCHAR(40),
        email VARCHAR(100) UNIQUE
    );
    CREATE TABLE person
    (
        name VARCHAR(40),
        email VARCHAR(100),
        UNIQUE(name, email)
    );

Its value must be unique for each row and can only have a **null value once**

## Check

    CREATE TABLE Persons 
    (
        Name VARCHAR(60), 
        Age INT,
        City VARCHAR(60),
        CONSTRAINT CHK_Person CHECK (Age>=18 AND City='Sandnes')
    );
    CREATE TABLE Persons 
    (
        Name VARCHAR(60),
        City VARCHAR(60)
        Age INT,
        CHECK (Age>=18)
    );

It is used to limit values of an attribute, however, MySQL does not enforce
check constraints for versions **8.0** or older

## Default

    CREATE TABLE loan
    (
        loan_id INT PRIMARY KEY,
        interest INT DEFAULT 10
    );

It provides a default value to for an attribute if none is provided

## Not Null

    CREATE TABLE loan
    (
        loan_id INT PRIMARY KEY,
        interest INT NOT NULL
    );

It enforces that an attribute cannot have a null value

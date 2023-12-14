# Primary and Foreign Key

## Primary Key

- It is the used to uniquely identify each and every row of a table
- It must be **unique**, **not null** and **immutable** and **only one** per table
- MySQL is much faster dealing with **integer** primary keys than other data types

        CREATE TABLE student
        (
            id INT PRIMARY KEY,
            fname VARCHAR(20),
            lname VARCHAR(20)
        );
        CREATE TABLE student
        (
            fname VARCHAR(20),
            lname VARCHAR(20),
            PRIMARY KEY(fname, lname)
        );

## Foreign Key

- It is used to connect two tables via *primary key(s)*
- Its value can either be null or must be present in the related table
- It must be the primary key of the related table

        CREATE TABLE employee
        (
            id INT PRIMARY KEY,
            fname VARCHAR(20),
            lname VARCHAR(20),
            dept_ID int,
            FOREIGN KEY(dept_ID) REFERENCES Department(ID)
        );
        CREATE TABLE class
        (
            id INT PRIMARY KEY,
            stud_fname VARCHAR(20),
            stud_lname VARCHAR(20),
            FOREIGN KEY(stud_fname, stud_lname) REFERENCES Student(fname, lname)
        );

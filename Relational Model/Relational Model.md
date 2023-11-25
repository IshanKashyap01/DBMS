# Relational Model

- Proposed by E.F. Codd in 1970, it is based on modelling the data as **relation**

- We follow the following steps to create a database:
  - Define the problem statement
  - Create an ER model
  - Create a Relational model
  - Implement the relational model using an RDBMS

## Terminologies in Relational Model

- In the context of Relational Model:
  - **Relation** means *table*
  - **Attribute/Field** means *column*
  - **Tuple** means a *row*

- **Degree** is the total number of *attributes* in a relation

- **Cardinality** is the total number of *tuples* in a relation

- **Relational Instance** is the identity of a relation at any given time
  - It will only have unique tuples i.e, no duplicates are allowed
  - It keeps changing as we add/delete tuples

- **Relational keys** are the various *attributes* of a tuple

- **Attribute domain** is the pre-defined range of values for an attribute

- **Relational schema** defines design and structure of the relation

## Properties of a Relation

- Values must be atomic i.e. cannot be broken down further
- Each value in a column must be of the same data type
- Each row has to be unique as redundancy is against the concepts of RDBMS
- Sequence of rows and columns are insignificant
- The value of each attribute has to be unique

**Note**: CRUD operations are performed via API to the database

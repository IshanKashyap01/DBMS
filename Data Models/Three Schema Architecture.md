# Architecture of Schema

We use a 3 schema architecture also known as ANSI, or SPARC architecture. It has
three schemas, each representing a different layer/level. These levels, in
increasing order of abstraction are:

1. Internal/Physical layer schema
2. Conceptual layer schema
3. External/View layer schemas

## Layers in 3 Schema Architecture

### Internal/Physical Layer Schema

- It explains the storage of data
- It contains the internal schema that tells us about how data is actually stored
via a physical data model
- It specifies the access path of all data

### Conceptual Layer Schema

- It defines the meaning of data
- It describes the structure of schema for the community or a set of users
- It hides the physical structure/schema
- Example: representational data model

### External/View Layer Schema

- It defines how to use/view the data
- It is used as a view for a number of users, that's why there are multiple
external levels
- It provides access control by providing different schemas depending on the user

## Important Features

- Every user can access same data but with a different view
- Hides the physical storage
- Provides data independence i.e. we can change one level without affecting the
other

## Logical Data Independence

- It refers to changing conceptual level w/o changing the physical level
- It is hard to achieve

## Physical Data Independence

- It refers to changing the physical level w/o changing the logical level
- It is easy to achieve

# Normal Forms

## First Normal Form (1 NF)

It states that a relation must not contain multi-valued attributes

## Second Normal Form (2 NF)

1. The relation must be satisfy the *first normal form*

2. There should be *no partial dependencies*

## Third Normal Form (3 NF)

1. The relation must be in the *second normal form*

2. There should be *no transitive dependencies*

## Boyce Codd Normal Form (BCNF or 3.5 NF)

1. The relation must be in the *third normal form*

2. For every non trivial functional dependency **A → B**, A must be a super key

    - i.e., a prime key should not depend on a non-prime key

# Functional Dependency

## Types for Functional Dependency

### Trivial

An attribute **A** and **B** have a *trivial functional dependency* if **B is a**
**subset of A**

### Non-Trivial

- When **B is not a subset of A** but its value *can be determined* using A

- Moreover, **A ⋂ B** must be **null**

## Rules for Functional Dependency (Armstrong's Axioms)

### Reflexive Rule

If A is a set of attributes and B is a subset of A, then A *determines* B

### Augmentation Rule

- If B can be determined from A, then adding an attribute to this dependency won't
change anything

- **A → B** holds then, **AM → BM** also holds true

### Transitive Rule

If A determines B, which determines C, then A also determines C

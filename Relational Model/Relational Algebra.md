# Relational Algebra

It is a **Procedural Query Language** that gives us a step-by-step way to arrive
at a definite result

## Selection (small sigma)

- It is used to select attributes and tuples from tables
- It does not display the selected items
Syntax:
    sign attribute_names conditions (table_name)

## Projection (pie)

- It is used to display/project the attributes and tuples from tables
- It can be used in conjunction with selection
Syntax:
    sign attribute_names/selection_statement (table_name/selection_statement)

## Union (⋃)

It returns all the values from the two operands
Syntax:
    operand ⋃ operand

## Intersection (⋂)

It returns only the common values b/w the two operands
Syntax:
    operand ⋂ operand

## Set Difference (-)

It returns the all the values from the first set except the ones present in the
second set
Syntax:
    A - B

## Cartesian Product (X)

It adds the attributes and returns the combination of all the tuples from both
the relations
Syntax:
    A X B

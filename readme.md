###SQL day 2 (aka sqewl, aka skl, .)

- Student can add foreign key to new table
- Student can add foreign key to existing table
- Student can use join
- Student can use sub-selects/nested queries
- Student can set null values
- Student can Group by
- Student can update rows
- Student can delete rows
- Student can use distinct
- Student can describe one-to-one relationships
- Student can describe one-to-many relationships
- Student can describe many-to-many relationships

* 1st normal form:
    - data in each column is indivisible

    - recommended:

        - string 
        - number 
        - boolean
        - float 
        - null

    - not recommended:

        - objects
        - arrays

* 2nd normal form:
    - first normal form
    - all non-key columns are fully functionally dependant on tables primary key

* 3rd normal form:
    - sencond normal form
    - contains only columns that are non transitively-dependent on a primary key

transitive: if A is greater than B, and B is greater than C then A must be greater than C 

A, B, PK, if the value of A relies on the Primary Key(PK) and B relies on the PK and A also relies on B then you
can say A relies on the PK through B 

```sql
personId, firstName, lastName => nontransitively dependant

personId, bodyMassIndex, isObese => transitively dependant
```

**one to one relationship**

- relationship between two tables where both tables match based on one matching column

<img width='500px' src='https://upload.wikimedia.org/wikipedia/commons/thumb/f/f7/CPT-Databases-OnetoOne.svg/500px-CPT-Databases-OnetoOne.svg.png'>

**one to many relationship**

- relationship between two tables where a column from one table can have multiple matching column in another tables

<img width='500px' src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d7/CPT-Databases-OnetoMany2.svg/500px-CPT-Databases-OnetoMany2.svg.png">

**many to many**

- occurs when multiple records in a table are associated with multiple records from another table 

<img width='500px' src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/c4/CPT-Databases-ManytoMany.svg/500px-CPT-Databases-ManytoMany.svg.png">


<img width='500px' src="https://upload.wikimedia.org/wikipedia/commons/0/02/Databases-ManyToManyWJunction.jpg">

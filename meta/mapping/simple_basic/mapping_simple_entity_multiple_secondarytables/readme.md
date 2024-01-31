see Jakarta Persistence Spec. (V 3.0)
chapter "11.1.46. SecondaryTable Annotation"

"The SecondaryTable annotation is used to specify a secondary table for the annotated entity class.
If no SecondaryTable annotation is specified, it is assumed that all persistent fields or properties of the
entity are mapped to the primary table. Specifying one or more secondary tables indicates that the
data for the entity class is stored across multiple tables.

[...]

If no primary key join columns are specified, the join columns are assumed to reference the primary
key columns of the primary table, and have the same names and types as the referenced primary key
columns of the primary table."
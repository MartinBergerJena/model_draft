see Jakarta Persistence Spec. (V 3.0)
chapter 11.1.44. "PrimaryKeyJoinColumn Annotation"

"The PrimaryKeyJoinColumn annotation specifies a primary key column that is used as a foreign key to
join to another table.
The PrimaryKeyJoinColumn annotation is used to join the primary table of an entity subclass in the
JOINED mapping strategy to the primary table of its superclass; it is used within a SecondaryTable
annotation to join a secondary table to a primary table; and it may be used in a OneToOne mapping in
which the primary key of the referencing entity is used as a foreign key[118] to the referenced entity[119]."

Excerpt from table 41 PrimaryKeyJoinColumn Annotation Elements:

"
Type: String
Name: name
Description: (Optional) The name of the primary key column of the current table.
Default: [...] the same name as the primary key column of the primary table (SecondaryTable mapping);[...]

Type: String
Name: referencedColumnName
Description: (Optional) The name of the primary key column of the table being joined to.
Default: [...] the same name as the primary key column of the primary table (SecondaryTable mapping);[...]
"
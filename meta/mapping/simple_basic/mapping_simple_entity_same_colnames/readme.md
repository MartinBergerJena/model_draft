see Jakarta Persistence Spec. (V 3.0)
chapter "10.1. Entity

The Entity annotation specifies that the class is an entity. This annotation is applied to the entity class.

The name annotation element specifies the entity name. If the name element is not specified, the entity
name defaults to the unqualified name of the entity class. This name is used to refer to the entity in
queries"


chapter "11.1.50. Table Annotation

The Table annotation specifies the primary table for the annotated entity. Additional tables may be
specified by using the SecondaryTable or SecondaryTables annotation.[121]
Table 47 lists the annotation elements that may be specified for the Table annotation and their default
values.
If no Table annotation is specified for an entity class, the default values defined in Table 47 apply."

excerpt from table 47 Table Annotation Elements:

"
Type: String
Name: name
Description: (Optional) The name of the table.
Default: Entity name
[...]
"

chapter "11.1.9. Column Annotation

The Column annotation is used to specify a mapped column for a persistent property or field.
Table 12 lists the annotation elements that may be specified for the Column annotation and their
default values.

If no Column annotation is specified, the default values in Table 12 apply."Entity

excerpt from table 12 Column Annotation Elements:

"
Type: String
Name: name
Description: (Optional) The name of the column.
Default: The property or field name.
[...]
"

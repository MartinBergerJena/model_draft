see Jakarta Persistence Spec. (V 3.0)

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
see Jakarta Persistence Spec. (V 3.0)

chapter "11.1.41. OneToOne Annotation

The OneToOne annotation defines a single-valued association to another entity that has one-to-one
multiplicity. It is not normally necessary to specify the associated target entity explicitly since it can
usually be inferred from the type of the object being referenced.
[...]"

chapter "11.2.4. Foreign Key Column Mappings

11.2.4.1. JoinColumn

The JoinColumn annotation is typically used in specifying a foreign key mapping. In general, the
foreign key definitions created will be provider-dependent and database-dependent. Applications that
are sensitive to the exact mapping that is used should use the foreignKey element of the JoinColumn
annotation or include DDL files that specify how the database schemas are to be generated.
The following elements of the JoinColumn annotation are used in schema generation:
• name
• referencedColumnName
• unique
• nullable
• columnDefinition
• table
• foreignKey
See Section 11.1.25 for rules that apply to these elements and join column creation, and sections
Section 2.10 and Section 11.1.8 for the rules that apply for the default mappings of foreign keys for
relationships and element collections.
[...]"

chapter "11.1.25. JoinColumn Annotation

The JoinColumn annotation is used to specify a column for joining an entity association or element
collection.

Table 24 lists the annotation elements that may be specified for the JoinColumn annotation and their
default values.

If the JoinColumn annotation itself is defaulted, a single join column is assumed and the default values
described in Table 24 apply.

The name annotation element defines the name of the foreign key column. The remaining annotation
elements (other than referencedColumnName) refer to this column and have the same semantics as for
the Column annotation.

If the referencedColumnName element is missing, the foreign key is assumed to refer to the primary
key of the referenced table.
[...]"
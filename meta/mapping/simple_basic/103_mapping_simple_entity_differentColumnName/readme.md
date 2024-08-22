see Jakarta Persistence Spec. (V 3.0)

chapter "11.1.6. Basic Annotation

The Basic annotation is the simplest type of mapping to a database column. The Basic annotation can
be applied to a persistent property or instance variable of any of the following types: Java primitive
types, wrappers of the primitive types, java.lang.String, java.math.BigInteger, java.math.BigDecimal,
java.util.Date, java.util.Calendar, java.sql.Date, java.sql.Time, java.sql.Timestamp, java.time.LocalDate,
java.time.LocalTime, java.time.LocalDateTime, java.time.OffsetTime, java.time.OffsetDateTime, byte[],
Byte[], char[], Character[], enums, and any other type that implements Serializable.[99] As described in
Section 2.8, the use of the Basic annotation is optional for persistent fields and properties of these
types. If the Basic annotation is not specified for such a field or property, the default values of the Basic
annotation will apply.

chapter "12.2.3.26. attributes

The attributes element groups the mapping subelements for the fields and properties of the entity. It
may be sparsely populated to include only a subset of the fields and properties. If the value of
metadata-complete is true, the remainder of the attributes will be defaulted according to the default
rules. If metadata-complete is not specified, or is false, the mappings for only those properties and
fields that are explicitly specified will be overridden."

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

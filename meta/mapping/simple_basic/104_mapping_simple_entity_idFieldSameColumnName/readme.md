see Jakarta Persistence Spec. (V 3.0)

chapter "11.1.21. Id Annotation
The Id annotation specifies the primary key property or field of an entity. The Id annotation may be
applied in an entity or mapped superclass.

The field or property to which the Id annotation is applied should be one of the following types: any
Java primitive type; any primitive wrapper type; java.lang.String; java.util.Date; java.sql.Date;
java.math.BigDecimal; _java.math.BigInteger_[109]. See Section 2.4.
The mapped column for the primary key of the entity is assumed to be the primary key of the primary
table. If no Column annotation is specified, the primary key column name is assumed to be the name of
the primary key property or field."

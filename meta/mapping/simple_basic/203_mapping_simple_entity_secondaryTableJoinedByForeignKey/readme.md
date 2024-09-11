This mapping example may possibly not work. It is an attempt to use PrimaryKeyJoinColumn to join an primary table
to a secondary table using a foreign key in the primary table that references the primary key in the secondary
table.

see https://en.wikibooks.org/wiki/Java_Persistence/Tables#Multiple_tables_with_foreign_keys:

"Sometimes you may have a secondary table that is referenced through a foreign key from the primary table to the 
secondary table instead of a foreign key from the secondary table to the primary table. You may even have a foreign 
key between two of the secondary tables. Consider having an EMPLOYEE and ADDRESS table where EMPLOYEE refers to 
ADDRESS through an ADDRESS_ID foreign key, and (for some strange reason) you only want a single Employee class that 
has the data from both tables. The JPA spec does not cover this directly, so if you have this scenario the first thing
to consider, if you have the flexibility, is to change your data model to stay within the confines of the spec. You
could also change your object model to define a class for each table, in this case an Employee class and an Address
class, which is typically the best solution. You should also check with you JPA implementation to see what extensions 
it supports in this area.

[...]

Another option is to just use the foreign key column in the @PrimaryKeyJoinColumn, this will technically be backward,
and perhaps not supported by the spec, but may work for some JPA implementations. However this will result in the table
insert order not matching the foreign key constraints, so the constraints will need to be removed, or deferred.

[...]"
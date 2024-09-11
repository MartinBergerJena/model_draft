This mapping example will probably not work. The attributes of a single entity are spread over a primary and a secondary
table, while the secondary table does not contain a row for each primary table element and the affected entity 
attributes are optional. In SQL an outer left join would be used to join the two tables.

see also https://en.wikibooks.org/wiki/Java_Persistence/Tables#Multiple_table_outer_joins:

"Another perversion of multiple table mapping is to desire to outer join the secondary table. This may be desired if
the secondary may or may not have a row defined for the object. Typically the object should be read-only if this is
to be attempted, as writing to a row that may or may not be there can be tricky.

This is not directly supported by JPA, and it is best to reconsider the data model or object model design if faced with
this scenario. Again it is possible to map this through a database view, where an outer join is used to join the tables
in the view. [...]"


- In the Northwind database, what is the type of relationship between the
  `Employee` and `Territory` tables?

#Andrea's answer
The relationship between Employee and Territory is many to many. A territory
can have many employees assigned to it. A single employee may be assigned
to many territories. An intermediary table is needed for joins.

- What is a situation where a document store (like MongoDB) is appropriate, and
  what is a situation where it is not appropriate?

  MongoDB is a NoSQL database. It is appropriate for a document store, 
  or any collection of heterogenous data. A situation where this might
  be appropriate is a large news archive. The disadvantage of using a NoSQL
  database is that it is not ACID (Atomicity, Consistency, Isolation, Durability) compliant.
  Some people like these for prototyping because you don't have to specify the schema
  up front. However, not having a schema has turned out to cause problems for many
  in the long run.  

- What is "NewSQL", and what is it trying to achieve?  
NewSQL aims to combine the key advantages of SQL and NoSQL. Ideally it will handle 
the volume and variety of datatypes that NoSQL supports, while adding the SQL features of 
being relational providing ACID guarantees. NewSQL solutions have been explored since 2011,
and are still under development. Amazon Auora is a NewSQL project.

NewSQL wants to give us "the best of both worlds" - the scalability of
non-relational approaches with the guarantees and standard querying language 
of relational approaches. It is the next generation of database systems, and there
are a variety of approaches being tried. Some try to add relational niceties
to non-relational systems (like transactions to MongoDB), and some try to scale a 
relational system up more (like Postgres SQL sharding or columnar data stores.)

SQL has been around since 1970and was adopted as an ANSI standard in 1986.
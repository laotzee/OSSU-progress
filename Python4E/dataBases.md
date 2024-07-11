**What is an attribute?** One of the values within a tuple. More commonly called a 'column' or a 'field'.
**What is a constraint?** When we tell the database to enforce a rule on a field or a row in a table. A common constraint is to insist that three can be no duplicate values in a particular field (i.e, all the tuples must be unique)
**What is a cursor?** A cursor allows you to execute SQL commands in a database and retrieve data from the database. A cursos is similar to a socket or a file handle for network connections and files respectively
**What is a database browser?** A piece of software that allows you to directly connect to a data base and manipulate the database directly without writing a program.
**What is a foreign key?** A numeric key that points to the primary key of a row in another table. Foreign keys establish relationships between rows stored in different tables
**What is an index?** An index in the context of databases is additional data that the database software maintains as rows and inserts into a table to make lookups very fast.
**What is a logical key?** A key that the 'outside world' uses to look up a particular row. For example, in a table of user accounts, a person's email address might be a good candidate as the logical key for the user's data.
**What does the term normalization mean?** Normalization means to design a data model so that no data is replicated. We store each item of data at one place in the database and reference it elsewhere using a foreign key.
**What is a primary key?** A numeric key assigned to each row that is used to refer to one row in a table from another table. Often the database is configured to automatically assign primary keys as rows are inserted.
**What is a relation?** An area within a database that contains tuples and attributes. More typically called a 'table'
**What is a tuple?** A single entry in a database table that is a set of attributes. More typically called 'row'

--- 

- A relation is defined as a set of *tuples* that have the same *attributes*. A tuple usually represents an object and information about that object.
- Objects are typically physical objects or concepts.
- A relation is usually describe as a table, which is organized into rows and columns.
- All the data reference by an attribute are in the same domain and conform to the same constrains. 
- SQL != Sequencial language but imperative
-  **Database Administrator**: Person responsible for for the design, implementation, maintenance, and repair or an organization's database. The role includes the development and design of a database strategies, monitoring and improving database performance and capacity, and planning for future expansions requirements. They also plan coordinate, and implement security measures to safeguard the database
- **Database Model**: A database model, or a database schema, is the structure of format of a database, describe in a formal language supported by the database management system. In other words, a "database model" is  the application of a data model when used in conjunction with a database management system.

**Database**: file that is organized to store data, which implements insertion and access of data very fast. 
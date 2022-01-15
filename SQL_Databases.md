# SQL & DATABASES CONCEPTS & QUESTIONS
### :dvd: <span style="color: aqua">What is a database?</span>
A database is an organized collection of data, stored and retrieved digitally from a remote or local computer system. Regardless of programming language, databases are vital. They help facilitate problem-solving through implementing structure and rules. They ensure scalability, accessibility, accuracy, security, consistency, permanence. Databases can be vast and complex, and such databases are developed using fixed design and modeling approaches.
### :dvd: <span style="color: aqua">What is a relational database?</span>
- A type of database that stores and provides access to data points that are related to one another.
- Based on a relational model: an intuitive / straightforward way of representing data in tables.
- Other types: Hierarchical, network, object-oriented, NoSQL

### :dvd: <span style="color: aqua">What is a database management system (DBMS)?</span>
DBMS stands for Database Management System. DBMS is a system software responsible for the creation, retrieval, updating, and management of the database. It ensures that our data is consistent, organized, and is easily accessible by serving as an interface between the database and its end-users or application software and allows a user to interact with and manipulate information within a DB. (Examples: Oracle - MySQL - PostgreSQL).  

### :dvd: <span style="color: aqua">What is SQL?</span>
***Structured Query Language***  
SQL stands for Structured Query Language. It is the standard language for relational database management systems. It is especially useful in handling organized data comprised of entities (variables) and relations between different entities of the data.
- It operates declaritively, you describe the outcome but are not concerned with how it occurs.
- CRUD Functions - Create, read, update, delete
    - Its good practice to use a SELECT statement prior to a DELETE query execution.
    
### :dvd: <span style="color: aqua">What are aggregate functions in SQL?</span>
An aggregate function performs operations on a collection of values to return a single scalar value to produce more meaningful information. Aggregate functions are often used with the GROUP BY and HAVING clauses of the SELECT statement. Examples of SQL aggregate functions:

- AVG() - Calculates the mean of a collection of values.
- COUNT() - Counts the total number of records in a specific table or view.
- MIN() - Calculates the minimum of a collection of values.
- MAX() - Calculates the maximum of a collection of values.
- SUM() - Calculates the sum of a collection of values.
- FIRST() - Fetches the first element in a collection of values.
- LAST() - Fetches the last element in a collection of values.

### :dvd: <span style="color: aqua">What are scalar functions in SQL?</span>
A scalar function returns a single value based on the input value. Following are the widely used SQL scalar functions:

- LEN() - Calculates the total length of the given field (column).
- UCASE() - Converts a collection of string values to uppercase characters.
- LCASE() - Converts a collection of string values to lowercase characters.
- MID() - Extracts substrings from a collection of string values in a table.
- CONCAT() - Concatenates two or more strings.
- RAND() - Generates a random collection of numbers of a given length.
- ROUND() - Calculates the round-off integer value for a numeric field (or decimal point values).
- NOW() - Returns the current date & time.
- FORMAT() - Sets the format to display a collection of values


### :dvd: <span style="color: aqua">Discuss Normalization</span>
- Normalization aims to improve the quality of the data. It represents the way of organizing structured data in the database efficiently. It includes the creation of tables, establishing relationships between them, and defining rules for those relationships. Inconsistency and redundancy can be kept in check based on these rules, hence, adding flexibility to the database. 
- Typically, in most business contexts 1st, 2nd, 3rd normal form is sufficient, but other normal forms exist and are more practical in a scientific setting. Additionally, denormalization may be warranted if there is a need to improve performance.

    - 1st NF – each cell in the col. / table must have only 1 value and no repeating groups
        - A relation is in first normal form if every attribute in that relation is a single-valued attribute. If a relation contains a composite or multi-valued attribute, it violates the first normal form. 
    - 2nd NF – (already in 1stNF), any non-key should be dependent on the entire primary key.
        - A relation is in second normal form if it satisfies the conditions for the first normal form and does not contain any partial dependency. A relation in 2NF has no partial dependency, i.e., it has no non-prime attribute that depends on any proper subset of any candidate key of the table. Often, specifying a single column Primary Key is the solution to the problem.
    - 3rd NF – (In 1st&2nd NF) No non-key field is dependent on any other key field.
        - A relation is said to be in the third normal form, if it satisfies the conditions for the second normal form and there is no transitive dependency between the non-prime attributes, i.e., all non-prime attributes are determined only by the candidate keys of the relation and not by any other non-prime attributeA relation is said to be in the third normal form, if it satisfies the conditions for the second normal form and there is no transitive dependency between the non-prime attributes, i.e., all non-prime attributes are determined only by the candidate keys of the relation and not by any other non-prime attribute.
    - Boyce-Codd Normal Form
        - A relation is in Boyce-Codd Normal Form if satisfies the conditions for third normal form and for every functional dependency, Left-Hand-Side is super key. In other words, a relation in BCNF has non-trivial functional dependencies in form X –> Y, such that X is always a super key. 


### :dvd: <span style="color: aqua">What do we need to do to decrease the retrieval time?</span>
Depending on the situation, denormalization might be appropriate. You could create an index (which operates like an index in the back of a book). It's basically a pointer to data in a table. Speeds up select and where queries but might slow down update and insert statements.

### :dvd: <span style="color: aqua">What are the different types of joins in SQL?</span>
The SQL Join clause is used to combine records (rows) from two or more tables in a SQL database based on a related column between the two.
* INNER JOINS:
    - Return rows only with matches from both tables. The most used / popular join.
* LEFT / RIGHT OUTER JOINS
    - Returns all the rows for that precedence and matches from the opposing side where possible. (i.e. Left outer join returns all left rows regardless if they have a match).
* FULL OUTER JOINS
    - Returns all rows no matter if they are matches or not.

### :dvd: <span style="color: aqua">Tables vs. Views in SQL</span>
A table contains data as seen in the database, a view is just a SELECT statement which has been saved in the database. The advantage of a view is that it can join data from several tables thus creating a new view of it. Say you have a database with salaries and you need to do some complex statistical queries on it. Instead of sending the complex query to the database all the time, you can save the query as a view and then SELECT * FROM view. Additionally it provides an element of security as users can access data through the view rather than needing permissions to interact with a table directly.
### :dvd: <span style="color: aqua">What is group by, order by in SQL?</span>
- Order by: sorts data into ascending or descending order. Ascending is default, to set descending use ```DESC``` keyword.
- Group by: used to arrange similar data (rows with the same value) into a group. Typically, follows the WHERE clause and before ORDER BY.

### :dvd: <span style="color: aqua">What is the having clause?</span>
The HAVING clause was added to SQL because the WHERE keyword cannot be used with aggregate functions. It allows one to perform queries based on specific conditions.

### :dvd: <span style="color: aqua">Types of keys in SQL</span>
A key is used to uniquely identify a particular row.
- Primary Keys - are unique and cannot occur more than once in a particular column
- A Unique Key – similar to primary key in that they provide uniqueness to a record but unlike a primary key it can accept a NULL value and be used on more than one column
- Foreign Keys - Creates a relationship with another table
- Composite Keys - When no natural keys exist, 2 fields are combined to create a primary key.
    - Used when creating many-to-many relationships

### :dvd: <span style="color: aqua">What is a foreign key?</span>
A foreign key creates a relationship with another table and is only used in one to one relationships.
It is comprised of a single or a collection of fields in a table that essentially refers to the PRIMARY KEY in another table. The foreign key constraint ensures referential integrity in the relation between two tables.
The table with the foreign key constraint is labeled as the child table, and the table containing the candidate key is labeled as the referenced or parent table

### :dvd: <span style="color: aqua">What is an index?</span>
An index acts as a special lookup table that can improve the speed of data retrieval in the database. Essentially it is a pointer to data in a table the same way an index in the back of a book points you to the related topic or information you’re looking for. It enhances the speed of operations accessing data from a database table at the cost of additional writes and memory to maintain the index data structure.

### :dvd: <span style="color: aqua">What are clustered / non-clustered indexes?</span>
- Clustered indexes are indexes whose order of the rows in the database corresponds to the order of the rows in the index. This is why only one clustered index can exist in a given table, whereas, multiple non-clustered indexes can exist in the table. 
- A CLUSTERED index – a table that is stored in a sorted order based on key value. Can only have 1 at a time (only sort in 1 order). Data and index are stored together similar to a phone book. If you don’t have a clustered index it’s referred to as a heap.
- A NON-CLUSTERED index – also called secondary indexes: stores only key values with a pointer to the row that contains the value.

### :dvd: <span style="color: aqua">Discuss how to build relationships?</span>
- One-to-One
    - This can be defined as the relationship between two tables where each record in one table is associated with the maximum of one record in the other table.
    - Relies on the use of a ***foreign key***.

- One-To-Many / Many-To-One: ***Most common***
    - This is the most commonly used relationship where a record in a table is associated with multiple records in the other table.
    - Uses ***references keyword*** to build relationships.

- Many-To-Many: Cannot create directly, not as obvious to identify
    - This is used in cases when multiple instances on both sides are needed for defining a relationship.
    - Created by using a junction or linking table
        - Only exists to join the table.

 - Self-Referencing Relationships - This is used when a table needs to define a relationship with itself

### :dvd: <span style="color: aqua">ACID Test</span>
- ***Atomic***: all or nothing transactions. Either all parts of the transaction occurs or none of them do.
- ***Consistency***: guarantees committed transaction state. The database must be consistent before & after a transaction occurs. If a transaction cannot be completed fully all at once, it rolls back to the original version.
- ***Isolation***: Transactions are independent and must occur without interference while still maintaining consistency. Transactions must also occur concurrently.
- ***Durability***: Committed data is never lost. All changes must be permanently stored in the databases' memory.

### :dvd: <span style="color: aqua">What is Referential Integrity?</span>
Referential integrity refers to the accuracy and consistency of data within a relationship. It is a subset of data integrity, which is concerned with the accuracy and consistency of all data. Data on both sides of a relationship must remain intact. A lack of referential integrity in a database can lead to incomplete data being returned, usually with no indication of an error. You cannot:
- Delete part of a record that relies on another.
- You cannot refer to data that doesn't exist.


### :dvd: <span style="color: aqua">What is an ERD?</span>
An ***entity relationship diagram*** or ***ER diagram*** is a type of structural diagram for use in database design. An ERD contains different symbols and connectors that visualize two important pieces information: The major entities within the system scope, and the inter-relationships among these entities. Simply put, it models the entities within a database and the relationships between them.

### :dvd: <span style="color: aqua">What is a primary key?</span>
A primary key is one or more columns that have been configured as the unique identifier field for the table. This means that they uniquely ID each row in the table, contain unique values (or combine to a unique identifier) and has an implicitly _not null_ constraint. Some examples of what would be an appropriate primary key:  
- An automatically generated number
- Social Security Number
- Drivers License Number
- E-mail address (so long as no users share the same one)

### :dvd: <span style="color: aqua">How can you get a list of all your databases?</span>
(PostgreSQL) On the command line:  
- psql  
- ```\l``` ***or*** ```\list```
### :dvd: <span style="color: aqua">How can you get the list of all the tables in a database?</span>
(PostgreSQL) On the command line:  
- psql 
- Connect to a DB using ```\c <database_name>```  
    - You can list databases available using ```\l``` ***or*** ```\list``` 
- ```\dt``` ***or*** ```\dtables```

### :dvd: <span style="color: aqua">How do you delete a table?</span>
(PostgreSQL) On the command line:  
- psql 
- Connect to a DB using ```\c <database_name>```  
    - You can list databases available using ```\l``` ***or*** ```\list```
- ```DROP TABLE <table_name>;```

### :dvd: <span style="color: aqua">What is NoSQL?</span>
NoSQL databases (also referred to as 'non-relational' or 'non-SQL') maintains unstructured data stored in JSON files. They're best for:  
- Handling large, unrelated, indeterminate, or rapidly changing data.
- Schema-Agnostic data or schema dictated by an application.
- Applications where performance and availability are more important than strong consistency.  
Some common scenarios involving NoSQL databases might be:  
- Mobile Apps
- Real-time Analytics
- Content Management
- Personalization
- IoT Apps
- Database Migration  

NoSQL databases scale data horizontally by sharding across servers. This differs from Relational databases which scale vertically by increasing server load.

### :dvd: <span style="color: aqua">What is a candidate key?</span>
Any column that can guarantee uniqueness is called a candidate key. But just because it’s a candidate key it doesn’t necessarily follow that it’s a primary key. Any candidate key would need to be specified as the primary key first. So it is possible that more than one column in a table can guarantee uniqueness, but only one of them is defined as the primary key.

### :dvd: <span style="color: aqua">What is a composite key?</span>
A composite key is a candidate key defined by more than one column. Therefore, a primary key can consist of more than one column. Two or more columns can be specified as being the primary key. In this case, the value of these columns is combined to create a unique identifier. Each column on its own doesn’t necessarily guarantee uniqueness but when the columns are combined, they must guarantee uniqueness if they are to be used as a primary key.

### :dvd: <span style="color: aqua">What is RDBMS? How is it different from DBMS?</span>
RDBMS stands for Relational Database Management System. The key difference here, compared to DBMS, is that RDBMS stores data in the form of a collection of tables, and relations can be defined between the common fields of these tables. DBMS involves storing data as a file and data elements are accessed individually and no normalization is present. Most modern database management systems like MySQL, Microsoft SQL Server, Oracle, IBM DB2, and Amazon Redshift are based on RDBMS.  

### :dvd: <span style="color: aqua">What are Tables and Fields?</span>
A table is an organized collection of data stored in the form of rows and columns. Columns can be categorized as vertical and rows as horizontal. The columns in a table are called fields and represent individual attributes while the rows are referred to as records and a single record displays the collection of attributes.
### :dvd: <span style="color: aqua">What are Constraints in SQL?</span>
Constraints are used to specify the rules concerning data in the table. It can be applied for single or multiple fields in an SQL table during the creation of the table or after creating using the ALTER TABLE command. The constraints are:
- ```NOT NULL```: Restricts NULL value from being inserted into a column.
- ```CHECK```: Verifies that all values in a field satisfy a condition.
- ```DEFAULT```: Automatically assigns a default value if no value has been specified for the field.
- ```UNIQUE```: Ensures unique values to be inserted into the field.
- ```INDEX```: Indexes a field providing faster retrieval of records.
- ```PRIMARY KEY```: Uniquely identifies each record in a table.
- ```FOREIGN KEY```: Ensures referential integrity for a record in another table
### :dvd: <span style="color: aqua">What is a UNIQUE constraint?</span>
A UNIQUE constraint ensures that all values in a column are different. This provides uniqueness for the column(s) and helps identify each row uniquely. Unlike primary key, there can be multiple unique constraints defined per table. The code syntax for UNIQUE is quite similar to that of PRIMARY KEY and can be used interchangeably.
### :dvd: <span style="color: aqua">What is a Self-Join?</span>
A self JOIN is a case of regular join where a table is joined to itself based on some relation between its own column(s). Self-join uses the INNER JOIN or LEFT JOIN clause and a table alias is used to assign different names to the table within the query.

### :dvd: <span style="color: aqua">What is a Cross-Join?</span>
Cross join can be defined as a cartesian product of the two tables included in the join. The table after join contains the same number of rows as in the cross-product of the number of rows in the two tables. If a WHERE clause is used in cross join then the query will work like an INNER JOIN.
### :dvd: <span style="color: aqua">What is Data Integrity?</span>
Data Integrity is the assurance of accuracy and consistency of data over its entire life-cycle and is a critical aspect of the design, implementation, and usage of any system which stores, processes, or retrieves data. It also defines integrity constraints to enforce business rules on the data when it is entered into an application or a database.
### :dvd: <span style="color: aqua">What is a Query?</span>
A query is a request for data or information from a database table or combination of tables. A database query can be either a select query or an action query.
### :dvd: <span style="color: aqua">What is a Sub-query / Nested Query?</span>
A sub-query is a query within another query, also known as a nested query or inner query. It is used to restrict or enhance the data to be queried by the main query, thus restricting or enhancing the output of the main query respectively.
### :dvd: <span style="color: aqua">What is the SELECT statement?</span>
SELECT operator in SQL is used to select data from a database. The data returned is stored in a result table, called the result-set
### :dvd: <span style="color: aqua">What are some common clauses used with SELECT query in SQL?</span>
- WHERE clause in SQL is used to filter records that are necessary, based on specific conditions.
- ORDER BY clause in SQL is used to sort the records based on some field(s) in ascending (ASC) or descending order (DESC).
- GROUP BY clause in SQL is used to group records with identical data and can be used in conjunction with some aggregation functions to produce summarized results from the database.
- HAVING clause in SQL is used to filter records in combination with the GROUP BY clause. It is different from WHERE, since the WHERE clause cannot filter aggregated records.


### :dvd: <span style="color: aqua"> What are UNION, MINUS and INTERSECT commands?</span>
The UNION operator combines and returns the result-set retrieved by two or more SELECT statements.
The MINUS operator in SQL is used to remove duplicates from the result-set obtained by the second SELECT query from the result-set obtained by the first SELECT query and then return the filtered results from the first.
The INTERSECT clause in SQL combines the result-set fetched by the two SELECT statements where records from one match the other and then returns this intersection of result-sets.
### :dvd: <span style="color: aqua">What are Entities and Relationships?</span>
- ```Entity```: An entity can be a real-world object, either tangible or intangible, that can be easily identifiable. For example, in a college database, students, professors, workers, departments, and projects can be referred to as entities. Each entity has some associated properties that provide it an identity.
- ```Relationships```: Relations or links between entities that have something to do with each other. For example - The employee's table in a company's database can be associated with the salary table in the same database.
### :dvd: <span style="color: aqua">What is an Alias in SQL?</span>
An alias is a feature of SQL that is supported by most, if not all, RDBMSs. It is a temporary name assigned to the table or table column for the purpose of a particular SQL query. In addition, aliasing can be employed as an obfuscation technique to secure the real names of database fields. A table alias is also called a correlation name.

An alias is represented explicitly by the ```AS``` keyword but in some cases, the same can be performed without it as well. Nevertheless, using the AS keyword is always a good practice.
### :dvd: <span style="color: aqua">What is Denormalization?</span>
Denormalization is the inverse process of normalization, where the normalized schema is converted into a schema that has redundant information. The performance is improved by using redundancy and keeping the redundant data consistent. The reason for performing denormalization is the overheads produced in the query processor by an over-normalized structure.
### :dvd: <span style="color: aqua">What are the TRUNCATE, DELETE and DROP statements?</span>
DELETE statement is used to delete rows from a table.
TRUNCATE command is used to delete all the rows from the table and free the space containing the table.
DROP command is used to remove an object from the database. If you drop a table, all the rows in the table are deleted and the table structure is removed from the database.

### :dvd: <span style="color: aqua">What is the difference between DROP and TRUNCATE statements?</span>
If a table is dropped, all things associated with the tables are dropped as well. This includes - the relationships defined on the table with other tables, the integrity checks and constraints, access privileges and other grants that the table has. To create and use the table again in its original form, all these relations, checks, constraints, privileges and relationships need to be redefined. However, if a table is truncated, none of the above problems exist and the table retains its original structure
### :dvd: <span style="color: aqua">What is the difference between DELETE and TRUNCATE statements?</span>
The TRUNCATE command is used to delete all the rows from the table and free the space containing the table.
The DELETE command deletes only the rows from the table based on the condition given in the where clause or deletes all the rows from the table if no condition is specified. But it does not free the space containing the table
### :dvd: <span style="color: aqua">What is OLTP?</span>
OLTP stands for Online Transaction Processing, is a class of software applications capable of supporting transaction-oriented programs. An essential attribute of an OLTP system is its ability to maintain concurrency. To avoid single points of failure, OLTP systems are often decentralized. These systems are usually designed for a large number of users who conduct short transactions. Database queries are usually simple, require sub-second response times, and return relatively few records.
### :dvd: <span style="color: aqua">What are the differences between OLTP and OLAP?</span>
OLTP stands for Online Transaction Processing, is a class of software applications capable of supporting transaction-oriented programs. An important attribute of an OLTP system is its ability to maintain concurrency. OLTP systems often follow a decentralized architecture to avoid single points of failure. These systems are generally designed for a large audience of end-users who conduct short transactions. Queries involved in such databases are generally simple, need fast response times, and return relatively few records. A number of transactions per second acts as an effective measure for such systems.

OLAP stands for Online Analytical Processing, a class of software programs that are characterized by the relatively low frequency of online transactions. Queries are often too complex and involve a bunch of aggregations. For OLAP systems, the effectiveness measure relies highly on response time. Such systems are widely used for data mining or maintaining aggregated, historical data, usually in multi-dimensional schemas
### :dvd: <span style="color: aqua">How to create empty tables with the same structure as another table?</span>
Creating empty tables with the same structure can be done smartly by fetching the records of one table into a new table using the INTO operator while fixing a WHERE clause to be false for all records. Hence, SQL prepares the new table with a duplicate structure to accept the fetched records but since no records get fetched due to the WHERE clause in action, nothing is inserted into the new table.
### :dvd: <span style="color: aqua">What is Pattern Matching in SQL?</span>
SQL pattern matching provides for pattern search in data if you have no clue as to what that word should be. This kind of SQL query uses wildcards to match a string pattern, rather than writing the exact word. The LIKE operator is used in conjunction with SQL Wildcards to fetch the required information.

- The % wildcard matches zero or more characters of any type and can be used to define wildcards both before and after the pattern. Search a student in your database with first name beginning with the letter K:
- Use the NOT keyword to select records that don't match the pattern. This query returns all students whose first name does not begin with K.
- Search for a student in the database where he/she has a K in his/her first name.
- The _ wildcard matches exactly one character of any type. It can be used in conjunction with % wildcard. This query fetches all students with letter K at the third position in their first name.
- The _ wildcard plays an important role as a limitation when it matches exactly one character. It limits the length and position of the matched results.
### :dvd: <span style="color: aqua">What is PostgreSQL?</span>
PostgreSQL was first called Postgres and was developed by a team led by Computer Science Professor Michael Stonebraker in 1986. It was developed to help developers build enterprise-level applications by upholding data integrity by making systems fault-tolerant. PostgreSQL is therefore an enterprise-level, flexible, robust, open-source, and object-relational DBMS that supports flexible workloads along with handling concurrent users. It has been consistently supported by the global developer community. Due to its fault-tolerant nature, PostgreSQL has gained widespread popularity among developers.

### :dvd: <span style="color: aqua">What is Stored Procedure?</span>
A stored procedure is a named group of SQL statements that have been previously created and stored in the server database. Stored procedures accept input parameters so that a single procedure can be used over the network by several clients using different input data. And when the procedure is modified, all clients automatically get the new version. Stored procedures reduce network traffic and improve performance. Stored procedures can be used to help ensure the integrity of the database.
### :dvd: <span style="color: aqua">What is Trigger?</span>
A trigger is a SQL procedure that initiates an action when an event (INSERT, DELETE or UPDATE) occurs. Triggers are stored in and managed by the DBMS. Triggers are used to maintain the referential integrity of data by changing the data in a systematic fashion. A trigger cannot be called or executed; DBMS automatically fires the trigger as a result of a data modification to the associated table. Triggers can be viewed as similar to stored procedures in that both consist of procedural logic that is stored at the database level. Stored procedures, however, are not event-driven and are not attached to a specific table as triggers are. Stored procedures are explicitly executed by invoking a CALL to the procedure while triggers are implicitly executed. In addition, triggers can also execute stored procedures.
### :dvd: <span style="color: aqua">What is Cursor?</span>
Cursor is a database object used by applications to manipulate data in a set on a row-by- row basis, instead of the typical SQL commands that operate on all the rows in the set at one time.

In order to work with a cursor we need to perform some steps in the following order:
1. Declare cursor
2. Open cursor
3. Fetch row from the cursor
4. Process fetched row
5. Close cursor
6. De-allocate cursor

### :dvd: <span style="color: aqua">What is Identity?</span>
Identity (or AutoNumber) is a column that automatically generates numeric values. A start and increment value can be set, but most DBA leave these at 1. A GUID column also generates numbers; the value of this cannot be controlled. Identity/GUID columns do not need to be indexed.

### :dvd: <span style="color: aqua">What is Data Warehousing?</span>
Data warehousing is a technology that aggregates structured data from one or more sources so that it can be compared and analyzed for greater business intelligence. 

### :dvd: <span style="color: aqua">What is Data Mining?</span>
Data Mining is a subcategory of Computer Science which aims at extraction of information from set of data and transform it into Human Readable structure, to be used later.
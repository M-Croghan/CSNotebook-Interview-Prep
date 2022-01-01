# SQL & DATABASES CONCEPTS & QUESTIONS
### <span style="color: aqua">What is a database?</span>
Regardless of programming language, databases are vital. Databases help facilitate problem-solving through implementing structure and rules. They ensure scalability, accessibility, accuracy, security, consistency, permanence.
### <span style="color: aqua">What is a relational database?</span>
- A type of database that stores and provides access to data points that are related to one another.
- Other types: Hierarchical, network, object-oriented, NoSQL

### <span style="color: aqua">What is a database management system?</span>
DBMS represents the software that allows of user to interact with and manipulate information within a DB.  
Database Management Systems (DBMS) -> Oracle - MySQL - Postgres  
- Create and manages databases
- Organization can maintain multiple databases   
Multiple DBMS can be used within a single organization  
Relational DBMS (RDBMS)  
Features:  
	- 1 or more tables (tables are the fundamental building block)  
		- Composed of columns and rows  
			- Columns: Name & Datatype   
Rows: Represent a record

### <span style="color: aqua">What is SQL?</span>
***Structured Query Language***  
- It operates declaritively, you describe the outcome but are not concerned with how it occurs.
- CRUD Functions - Create, read, update, delete
    - Its good practice to use a SELECT statement prior to a DELETE query execution.
    
### <span style="color: aqua">What are aggregate functions in SQL?</span>
- Is a function that returns certain value on the selected rows to produce more meaningful information.
    - Count(), Sum(), Avg(), Min(), Max()

### <span style="color: aqua">What are scalar functions in SQL?</span>
- Similar to aggregate, performs operation on the data
    - UCASE(), LCASE(), ROUND(), NOW(), MID()

### <span style="color: aqua">Discuss Normalization</span>
- Normalization aims to improve the quality of the data. Typically, in most business contexts 1st, 2nd, 3rd normal form is sufficient, but other normal forms exist and are more practical in a scientific setting. Additionally, denormalization may be warranted if there is a need to improve performance.
    - 1st NF – each cell in the col. / table must have only 1 value and no repeating groups
    - 2nd NF – (already in 1stNF), any non-key should be dependent on the entire primary key.
    - 3rd NF – (In 1st&2nd NF) No non-key field is dependent on any other key field.

### <span style="color: aqua">What do we need to do to decrease the retrieval time?</span>
Depending on the situation, denormalization might be appropriate. You could create an index (which operates like an index in the back of a book). It's basically a pointer to data in a table. Speeds up select and where queries but might slow update and insert statements.

### <span style="color: aqua">What are the different types of joins in SQL?</span>
* INNER JOINS:
    - Return rows only with matches from both tables. The most used / popular join.
* LEFT / RIGHT OUTER JOINS
    - Returns all the rows for that precedence and matches from the opposing side where possible. (i.e. Left outer join returns all left rows regardless if they have a match).
* FULL OUTER JOINS
    - Returns all rows no matter if they are matches or not.

### <span style="color: aqua">Tables vs. Views in SQL</span>
Virtual table. A view is a specific query made and saved from a table. Instead of having to reproduce a specific / complex query repeatedly, you could create a view to save that information. You can also join other tables using the view, additionally it provides an element of security as users can access data through the view rather than needing permissions to interact with a table directly.

### <span style="color: aqua">What is group by, order by in SQL?</span>
- Order by: sorts data into ascending or descending order. Ascending by default, DESC keyword.
- Group by: used to arrange similar data into a group. Typically, follows the WHERE clause and before ORDER BY.

### <span style="color: aqua">What is the having clause?</span>
WHERE keyword doesn't apply to aggregate functions and the having clause allows one to perform queries based on specific conditions.

### <span style="color: aqua">Types of keys in SQL</span>
- A key is used to uniquely identify a particular row
- Primary Keys - are unique and cannot occur more than once in a particular column
- A Unique Key – similar to primary key in that they provide uniqueness to a record but unlike a primary key it can accept a NULL value and be used on more than one column
- Foreign Keys - Creates a relationship with another table
- Composite Keys - When no natural keys exist, 2 fields are combined to create a primary key.
    - Used when creating many-to-many relationships

### <span style="color: aqua">What is a foreign key?</span>
A foreign key creates a relationship with another table and is only used in one to one relationships.

### <span style="color: aqua">What are two different types of indexes for a table? [??]</span>
Clustered & Non-Clustered

### <span style="color: aqua">What is an index?</span>
Act as a special lookup table that can improve the speed of data retrieval. Essentially a pointer to data in a table the same way an index in the back of a book points you to the related topic or information you’re looking for.

### <span style="color: aqua">What are clustered / non-clustered indexes?</span>
- A CLUSTERED index – a table that is stored in a sorted order based on key value. Can only have 1 at a time (only sort in 1 order). Data and index are stored together similar to a phonebook. If you don’t have a clustered index it’s referred to as a heap.
- A NON-CLUSTERED index – also called secondary indexes: stores only key values with a pointer to the row that contains the value.

### <span style="color: aqua">Discuss how to build relationships?</span>
- One-to-One
  - Relies on the use of a ***foreign key***.
- One-To-Many: Most common
  - Uses ***references keyword*** to build relationships.
- Many-To-Many: Cannot create directly, not as obvious to identify
    - Created by using a junction or linking table
        - Only exists to join the table.

### <span style="color: aqua">ACID Test</span>
- Atomic – all or nothing transactions. Either all parts of the transaction occurs or none of them do.
- Consistency – guarantees committed transaction state. The database must be consistent before & after a transaction occurs.
If a transaction cannot be completed fully all at once, it rolls back to the original version.
- Isolation – Transactions are independent and must occur without interference while still maintaining consistency. Transactions must 
also occur concurrently.
- Durability – Committed data is never lost. All changes must be permanently stored in the databases' memory.

### <span style="color: aqua">What is Referential Integrity?</span>
- You cannot delete part of data
- You cannot refer to data that doesn't exist


### <span style="color: aqua">What is an ERD?</span>
An ***entity relationship diagram*** or ***ER diagram*** is a type of structural diagram for use in database design. An ERD contains different symbols and connectors that visualize two important pieces information: The major entities within the system scope, and the inter-relationships among these entities. Simply put, it models the entities within a database and the relationships between them.

### <span style="color: aqua">What is a primary key?</span>
A primary key is one or more columns that have been configured as the unique identifier field for the table. Most primary keys are comprised of a single column, but they can also be comprised of multiple columns. Any value stored in a primary key field is unique to that record. No other record contains that value. The value is a unique identifier. Some examples of what would be an appropriate primary key:  
- An automatically generated number
- Social Secuity Number
- Drivers License Number
- E-mail address (so long as no users share the same one)


### <span style="color: aqua">How can you get a list of all your databases?</span>
On the command line:  
- psql  
- ```\l``` ***or*** ```\list```
### <span style="color: aqua">How can you get the list of all the tables in a database?</span>
On the command line:  
- psql 
- Connect to a DB using ```\c <database_name>```  
    - You can list databases available using ```\l``` ***or*** ```\list``` 
- ```\dt``` ***or*** ```\dtables```

### <span style="color: aqua">How do you delete a table?</span>
On the command line:  
- psql 
- Connect to a DB using ```\c <database_name>```  
    - You can list databases available using ```\l``` ***or*** ```\list```
- ```DROP TABLE <table_name>;```

### <span style="color: aqua">What is NoSQL?</span>
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

NoSQL databses scale data horizontally by sharding across servers. This differs from Relational databases which scale vertically by increasing server load.

### <span style="color: aqua">What is a candidate key?</span>
Any column that can guarantee uniqueness is called a candidate key. But just because it’s a candidate key it doesn’t necessarily follow that it’s a primary key. Any candidate key would need to be specified as the primary key first. So it is possible that more than one column in a table can guarantee uniqueness, but only one of them is defined as the primary key.

### <span style="color: aqua">What is a composite key?</span>
A composite key is a candidate key defined by more than one column. Therefore, a primary key can consist of more than one column. Two or more columns can be specified as being the primary key. In this case, the value of these columns is combined to create a unique identifier. Each column on its own doesn’t necessarily guarantee uniqueness but when the columns are combined, they must guarantee uniqueness if they are to be used as a primary key.
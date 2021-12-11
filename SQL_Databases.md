# SQL & DATABASES
### <span style="color: aqua">What is a relational database?</span>
- A type of database that stores and provides access to data points that are related to one another.
- Other types: Hierarchical, network, object-oriented, NoSQL

### <span style="color: aqua">What is a database management system?</span>
DBMS represents the software that allows of user to interact with and manipulate information within a DB.

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
Depending on the situation, denormalization might be appropriate. You could create an index (which operates like an index in the back of a book). Its basically a pointer to data in a table. Speeds up select and where queries but might slow update and insert statements.

### <span style="color: aqua">What are the different types of joins in SQL?</span>
* INNER JOINS:
    - Returns rows only with matches from both tables.
* LEFT / RIGHT OUTER JOINS
    - Returns all of the rows for that precedence and matches from the opposing side where possible. (i.e. Left outer join returns all left rows regardless if they have a match).
* FULL OUTER JOINS
    - Returns all rows no matter if they are matches or not.

### <span style="color: aqua">Tables vs. Views in SQL</span>
Virtual table. A view is a specific query made and saved from a table. Instead of having to reproduce a specific / complex query repeatedly, you could create a view to save that information. You can also join other tables using the view, additionally it provides an element of security as users can access data through the view rather than needing permissions to interact with a table directly.

### <span style="color: aqua">What is group by, order by in SQL?</span>
- Order by: sorts data into ascending or descending order. Ascending by default, DESC keyword.
- Group by: used to arrange similar data into a group. Typically follows the WHERE clause and before ORDER BY.

### <span style="color: aqua">What is the having clause?</span>
WHERE keyword doesn’t apply to aggregate functions and the having clause allows to perform queries based on specific conditions.

### <span style="color: aqua">Types of keys in SQL</span>
- A key is used to uniquely identify a particular row
- Primary Keys - are unique and cannot occur more than once in a particular column
- A Unique Key – similar to primary key in that they provide uniqueness to a record but unlike a primary key it can accept a NULL value and be used on more than one column
- Foreign Keys - Creates a relationship with another table
- Composite Keys - When no natural keys exist, 2 fields are combined to create a primary key.
    - Used when creating many-to-many relationships

### <span style="color: aqua">What is a foreign key?</span>
A foreign key creates a relationship with another table

### <span style="color: aqua">What are two different types of indexes for a table? [??]</span>
Clustered & Non-Clustered

### <span style="color: aqua">What is an index?</span>
Act as a special lookup table that can improve the speed of data retrieval. Essentially a pointer to data in a table the same way an index in the back of a book points you to the related topic or information you’re looking for.

### <span style="color: aqua">What are clustered / non-clustered indexes?</span>
- A CLUSTERED index – a table that is stored in a sorted order based on key value. Can only have 1 at a time (only sort in 1 order). Data and index are stored together similar to a phonebook. If you don’t have a clustered index it’s referred to as a heap.
- A NON-CLUSTERED index – also called secondary indexes: stores only key values with a pointer to the row that contains the value.

### <span style="color: aqua">Discuss how to build relationships?</span>
- One-to-One
- One-To-Many: Most common
- Many-To-Many: Cannot create directly, not as obvious to identify
    - Created by using a junction or linking table
        - Only exists to join the table.

### <span style="color: aqua">ACID Test</span>
- Atomic – all or nothing transactions
- Consistency – guarantees committed transaction state
- Isolation – Transactions are independent
- Durability – Committed data is never lost.

### <span style="color: aqua">What is Referential Integrity?</span>
- You cannot delete part of data
- You cannot refer to data that doesn't exist


### <span style="color: aqua"></span>

### <span style="color: aqua"></span>
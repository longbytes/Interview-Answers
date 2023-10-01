# Interview-Answers
Answers to the Data Interview Questions

## SQL & DB Interview Questions & Answers 

### What is the primary key, and why is it important?
A primary key is a special relational database table column (or combination of columns) designated to uniquely identify all table records. It’s important for several reasons:
* Uniqueness: A primary key ensures that each record in the table is unique. This means that no two rows in the table can have the same primary key value.
* Data Integrity: By enforcing uniqueness, primary keys prevent duplicate entries and help to maintain data integrity.
* Relationships: Primary keys are often used to create relationships between tables. For example, a foreign key in one table could reference the primary key in another table, creating a link between the data in both tables.
* Efficient Data Retrieval: Databases are often optimized to search and sort by primary key, making data retrieval operations faster and more efficient.

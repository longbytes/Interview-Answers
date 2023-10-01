# Interview-Answers
This list is the collection of answers to the interview questions in those repositories for [Data Science](https://github.com/longnguyendata/Data-Science-Interview-Questions-Answers) and [Data Engineering](https://github.com/longnguyendata/Data-Engineering-Interview-Questions-Answers).

## SQL & DB Interview Questions & Answers 

### What is the primary key, and why is it important?
A primary key is a special relational database table column (or combination of columns) designated to uniquely identify all table records. It’s important for several reasons:
* Uniqueness: A primary key ensures that each record in the table is unique. This means that no two rows in the table can have the same primary key value.
* Data Integrity: By enforcing uniqueness, primary keys prevent duplicate entries and help to maintain data integrity.
* Relationships: Primary keys are often used to create relationships between tables. For example, a foreign key in one table could reference the primary key in another table, creating a link between the data in both tables.
* Efficient Data Retrieval: Databases are often optimized to search and sort by primary key, making data retrieval operations faster and more efficient.

### How do I choose the right primary key for my table?
Choosing the right primary key for your table is a critical step in database design. Here are some guidelines to help you make the right choice:
* Uniqueness: The primary key field must be unique for each record. It should not contain null values.
* Stability: Choose a primary key that doesn’t change. Updating primary keys can be problematic, especially if they’re used in foreign key relationships.
* Non-sensitive: Primary keys often appear in logs or other external systems, so they shouldn’t be sensitive or private data.
* Relevance: Although it’s tempting to use a field like ‘email’ or ‘username’ as a primary key for a Users table, it’s generally better to use an auto-incrementing ID or similar. This is because fields like ‘email’ or ‘username’ might change, breaking the Stability rule.

### What is the foreign key, and why is it important?
A foreign key is a column or group of columns in a relational database table that provides a link between data in two tables. It acts as a cross-reference between tables because it references the primary key of another table, thereby establishing a link between them. Foreign keys play an essential role in database relationships, particularly in relation to maintaining the integrity of the data:
* Referential Integrity: Foreign keys help to ensure referential integrity in the relationship between two tables. This means that the foreign key in any referencing table must always refer to a valid row in the referenced table.
* Relationships Between Tables: Foreign keys enable the creation of relationships between tables (or relations). They can be used to establish various types of data relationships, such as one-to-one, one-to-many, and many-to-many relationships.
* Data Consistency: By enforcing relationships between tables, foreign keys ensure consistency and accuracy of the data within the database.
* Query Versatility: They allow you to perform complex queries and obtain meaningful results by joining tables on the foreign key.

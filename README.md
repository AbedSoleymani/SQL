# SQL
SQL, or Structured Query Language, is a specialized programming language used for managing and manipulating **relational databases**. It is the standard language for interacting with and managing data in a relational database management system (RDBMS). SQL provides a set of commands and syntax for performing tasks such as data retrieval, insertion, updating, and deletion, as well as defining and modifying the structure of a database.

Here are some key aspects of SQL:

1. Data Querying: SQL is used to retrieve data from a database. You can specify which columns and rows of data you want to retrieve using SQL SELECT statements.
2. Data Modification: SQL allows you to insert, update, and delete data in a database. You can use SQL INSERT, UPDATE, and DELETE statements for these purposes.
3. Schema Definition: SQL is used to define the structure of a database, including tables, columns, constraints, and relationships. The CREATE TABLE statement is an example of SQL used for schema definition.
4. Data Manipulation: SQL provides functions and operators for manipulating data within the database. You can perform calculations, string manipulations, and other operations on data using SQL.
5. Data Integrity: SQL supports the definition of integrity constraints to ensure data accuracy and consistency. These constraints include primary keys, foreign keys, unique constraints, and check constraints.
6. Transaction Control: SQL provides commands for managing transactions, such as COMMIT (to save changes) and ROLLBACK (to undo changes) to maintain data integrity.

SQL is used in various database management systems, including MySQL, PostgreSQL, SQLite, Microsoft SQL Server, Oracle, and many others. While the core SQL syntax is standardized, each database system may have its own extensions and specific features.

So, what is **relational database**? Relational databases are a type of database management system (DBMS) that organizes and stores data in a structured manner using a relational model. This model represents data as tables or relations, where each table contains rows and columns. Relational databases are designed to efficiently manage and manipulate structured data while maintaining the integrity of the relationships between different data elements. Here are some key characteristics and components of relational databases:

1. Tables: In a relational database, data is organized into tables, also referred to as relations. Each table is made up of rows (tuples) and columns (attributes or fields). Rows represent individual records, while columns represent specific attributes of the data.
2. Schemas: Relational databases have a schema that defines the structure of the database, including the tables, their columns, data types, and constraints. The schema enforces data integrity and provides a blueprint for the database's structure.
3. Relationships: Relational databases are known for their ability to establish relationships between tables. This is achieved through the use of keys, such as primary keys and foreign keys, to link records in one table to records in another. These relationships enable data consistency and integrity.
4. SQL: Structured Query Language (SQL) is the standard language for interacting with relational databases. SQL provides a set of commands for querying, inserting, updating, and deleting data, as well as defining and modifying the database schema.

Now, what is **database schema**? Database schema is a blueprint or structural framework that defines the organization and structure of a database. It specifies how data is stored, how tables are related to each other, and the constraints that govern the data. The database schema defines the logical design of the database and provides a way to understand its structure without necessarily looking at the actual data.

# Database Management System (DBMS)
A **Database Management System (DBMS)** is a software system that provides an organized and efficient means of managing and storing data (i.e., CRUD: Read, Update, and Delete). DBMSs are designed to interact with users, applications, and the database itself to capture and analyze data. They offer a structured and secure way to store, retrieve, and manipulate data, making it easier to manage large amounts of information.

Key Characteristics and Functions of a DBMS

- **Data Storage:** DBMSs store data in structured formats, often using tables (in the case of relational databases) or other data structures.
- **Data Retrieval:** They provide mechanisms to retrieve data from the database using query languages like SQL (Structured Query Language).
- **Data Manipulation:** DBMSs enable the addition, modification, and deletion of data through commands like INSERT, UPDATE, and DELETE.
- **Data Security:** They implement security measures to protect data from unauthorized access, including user authentication, access control, and encryption.
- **Data Integrity:** DBMSs enforce data integrity rules and constraints to maintain the accuracy and consistency of data.
- **Data Concurrency:** They manage concurrent access to data by multiple users or applications to ensure consistency and prevent conflicts.
- **Data Recovery:** DBMSs often include mechanisms for backup, restore, and recovery in case of system failures or data corruption.
- **Data Independence:** DBMSs provide data independence by separating the physical storage of data from the way data is presented to users or applications. This allows changes to the data structure without affecting how data is accessed.
- **Query Optimization:** They optimize queries to improve performance, often using techniques like indexing and query planning.
- **Interacting with software applications:** DBMSs facilitate interactions with software applications, allowing them to read, write, and manipulate data stored in the database.

# Relational vs. Non-Relational Databases

Relational databases and non-relational databases, often referred to as NoSQL databases, are two distinct types of database management systems. They have different characteristics, advantages, and use cases. This comparison outlines their key differences.

## Relational Databases

- **Data Model:** Relational databases use a structured data model based on tables with rows and columns, organizing data in a tabular format.

- **Schema:** They have a fixed schema, which means data structure is defined in advance. Schema changes can be complex and may require data migration.

- **ACID Properties:** Relational databases support ACID (Atomicity, Consistency, Isolation, Durability) properties, ensuring data consistency and reliability, even in the presence of system failures.

- **SQL:** SQL (Structured Query Language) is the standard query language for relational databases, providing a powerful and standardized way to query and manipulate data.

- **Use Cases:** Well-suited for applications with structured and well-defined data requirements, such as financial systems, e-commerce platforms, and systems where data consistency and transactions are critical.

- **Examples:** MySQL, PostgreSQL, Oracle Database, Microsoft SQL Server.

## Non-Relational Databases (NoSQL)

- **Data Model:** NoSQL databases use a variety of data models, including document-oriented (JSON, XML, etc), key-value, column-family, graph, and flexible table. They are more flexible in handling unstructured or semi-structured data.

- **Schema:** They are often schema-less or have a flexible schema, allowing changes in data structure without extensive schema alterations.

- **ACID vs. BASE:** NoSQL databases often prioritize availability and partition tolerance over strict consistency (ACID). This is sometimes summarized as the BASE (Basically Available, Soft state, Eventually consistent) model.

- **Query Languages:** While some NoSQL databases offer query languages (e.g., MongoDB's query language for document databases), they may not be as standardized or as feature-rich as SQL.

- **Use Cases:** Suitable for applications where data is unstructured, rapidly changing, or distributed across multiple servers. Commonly used in big data, real-time applications, content management systems, and systems requiring horizontal scalability.

- **Examples:** MongoDB (document store), Redis (key-value store), Cassandra (column-family store), Neo4j (graph database).

- Please note that Any non-relational database falls under this category, so there's no set language standard.
Most NRDBMS will implement their own language for performing CRUD and administrative operations on the database.

The choice between a relational and a non-relational database depends on your specific project requirements. If your data is structured and consistency is paramount, a relational database may be a better choice. If you need flexibility, scalability, and can tolerate eventual consistency, a NoSQL database may be more appropriate. Some projects even use a combination of both types of databases to address different aspects of their data management needs.


SQL is often categorized into four main types of language, each serving distinct purposes:

* Data Query Language (DQL)

DQL is used for querying a database to retrieve information. The primary statement used in DQL is the `SELECT` statement, which allows users to extract data from one or more tables in a structured manner.

* Data Definition Language (DDL)

DDL is responsible for defining and managing the structure and schema of the database. DDL statements include `CREATE`, `ALTER`, and `DROP`. These statements are used to create tables, modify their structure, or remove tables and other database objects.

* Data Control Language (DCL)

DCL is used for controlling access to the data stored in the database. It includes statements such as `GRANT` (to give privileges) and `REVOKE` (to revoke privileges). DCL is essential for managing user permissions and access rights to various database objects.

* Data Manipulation Language (DML)

DML is used for adding, updating, and deleting data within the database. Key DML statements include `INSERT` (to add new data), `UPDATE` (to modify existing data), and `DELETE` (to remove data). DML statements are used to manage the content of the database.

These language categories form the foundation of SQL and are essential for effectively managing and interacting with relational databases.


# Various Points
A **surrogate key**, in the context of databases, is a system-generated unique identifier assigned to each record or row in a table. Surrogate keys are typically used as the primary key of a table to ensure that each row has a unique and stable reference, regardless of the data values in the other columns. Surrogate keys are not derived from any inherent characteristics of the data but are instead generated by the database management system (DBMS) or the application.

In contrast, a **natural key**, in the context of databases, is a primary key that is based on one or more attributes or columns that have inherent meaning within the domain of the data. Natural keys are derived from the actual data values of the records and provide a way to uniquely identify each record based on properties or attributes that are relevant to the data's real-world context (e.g., SIN number, employee number, etc.).

A **foreign key** in a relational database is a column or a set of columns that establishes a link or relationship between two tables. It enforces referential integrity by ensuring that the values in the foreign key column(s) of one table match the values in the primary key column(s) of another table. In other words, it creates a connection between records in different tables, typically to represent relationships between data entities.

A **composite key**, in the context of a relational database, is a key that consists of two or more columns used together to uniquely identify a record or row within a table. Unlike a single-column primary key, which uses a single attribute to uniquely identify records, a composite key relies on the combination of multiple attributes (columns) to achieve uniqueness.
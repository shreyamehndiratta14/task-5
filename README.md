 Objective:
To design and implement a relational database for a Library Management System using SQL. The project involves creating schema, inserting and manipulating data, and writing queries involving filtering, aggregation, and various types of joins.

 Tools Used:
MySQL Workbench / DB Browser for SQLite

SQL (Structured Query Language)

 Database Structure:
Table Name	Description
Authors	Stores author details
Books	Stores book details
Borrowers	Stores borrower details
BorrowRecords	Records book borrow transactions

 Schema Overview:
Authors(AuthorID, Name, Country)

Books(BookID, Title, AuthorID, Year)

Borrowers(BorrowerID, Name, Email, Age)

BorrowRecords(RecordID, BookID, BorrowerID, BorrowDate, ReturnDate)

 Tasks Completed:
 Task 1: Database Setup & Schema Design
Created tables with appropriate constraints and foreign keys.

 Task 2: Data Insertion and Handling NULLs
Inserted data into all tables, including cases with NULL values (e.g., unknown author or missing age).

 Task 3: SELECT Queries
Basic retrieval queries using SELECT, WHERE, and filters on Year and NULL conditions.

 Task 4: Aggregates and Grouping
Used COUNT(), AVG(), and GROUP BY to derive insights such as:

Number of books per author

Number of books borrowed by each user

Average age of borrowers

 Task 5: SQL Joins (Inner, Left, Right, Full)
Used various joins to combine data across multiple tables:

INNER JOIN: Books and Authors

LEFT JOIN: All Books with Authors (even if author is missing)

RIGHT JOIN: All Authors with their Books (MySQL only)

FULL OUTER JOIN: All books and authors, using UNION (MySQL only)

Multi-table join on Borrowers, Books, and BorrowRecords


To re-run script: Use DROP TABLE IF EXISTS at the top to reset the database.

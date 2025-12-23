# Library Management Database System

## Project Overview
This project is a relational database design for a Library Management System. It aims to manage books, authors, members, and the borrowing process efficiently. The database ensures data integrity through the use of primary keys, foreign keys, and unique constraints.

## Features
* Authors Management: Stores information about book authors.
* Book Tracking: Maintains a record of available books, their ISBN numbers, and links them to their respective authors.
* Member Records: Keeps track of registered library members and their contact information.
* Borrowing System: Manages the relationship between members and books, tracking borrowing and return dates.

## Database Schema
The database consists of the following tables:
1. Authors: Contains author_id, author_name, and nationality.
2. Books: Contains book_id, title, isbn (Unique), published_year, and author_id (Foreign Key).
3. Members: Contains member_id, first_name, last_name, email (Unique), and join_date.
4. Borrowing: Contains borrow_id, book_id (Foreign Key), member_id (Foreign Key), borrow_date, and return_date.



## How to Use
1. Clone this repository to your local machine.
2. Ensure you have MySQL installed.
3. Open your MySQL terminal or a tool like MySQL Workbench.
4. Run the following command to set up the database:
   `sql
   SOURCE library_management.sql;
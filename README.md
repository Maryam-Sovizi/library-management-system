markdown
# Library Management System

A simple Library Management System built with PostgreSQL.

## Features

- Manage books, authors, and categories
- Member management
- Borrow and return books
- Automatic stock update using Triggers
- Useful views for reports
- Stored functions for borrow and return operations

## How to Run

1. Create a database:


sql
CREATE DATABASE library_db;


2. Run the SQL files in order:


bash
psql -U postgres -d library_db -f schema/01_tables.sql
psql -U postgres -d library_db -f schema/02_triggers.sql
psql -U postgres -d library_db -f schema/03_functions.sql
psql -U postgres -d library_db -f schema/04_views.sql
psql -U postgres -d library_db -f schema/05_indexes.sql


## Author

Maryam Sovizi
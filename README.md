
# Phone Book Records Management System

## Overview
This Python-based system manages phone book records stored in a CSV file. It provides functionalities to read, write, query, insert, and delete records using a SQL-like interface.

The system offers an interface similar to SQL queries to interact with phone book records, allowing users to perform operations like fetching all records, retrieving records by name, adding new entries, and deleting existing records.

## Features

- **CSV File Handling:** Reads and writes phone book records to a CSV file, providing persistent storage.
- **CRUD Operations:** Implements CRUD functionalities - Create, Read, Update, Delete - through SQL-like queries.
- **SQL-like Query Parser:** Interprets queries to perform specific operations on the phone book records.
- **Error Handling:** Addresses potential file handling errors and invalid query inputs.

## Problem Statements

The system addresses the following problem statements:

### Problem 1: Reading and Writing Phone Book Records
- Reads phone book records from a CSV file.
- Writes phone book records to a CSV file.

### Problem 2: Implementing SQL-like Parser for CRUD Operations
- Fetches all records using ***SELECT * FROM phone_records;***.
- Retrieves records based on the name using ***SELECT * FROM phone_records WHERE name='doe';***.
- Inserts new entries using ***INSERT INTO phone_records(...) VALUES(...);***.
- Deletes records based on the name using ***DELETE FROM phone_records WHERE name='John';***.

## Usage

To use this system:

1) Ensure you have Python 3.x installed on your machine.
2) Modify the *file_name* variable in the code to point to your CSV file.
3) Run the program in a Python environment.

## Functions

**Reading and Writing Records**

- **read_phone_records():** Reads phone book records from the specified CSV file.
- **write_phone_records(records):** Writes phone book records to the specified CSV file.

**CRUD Operations**
- **select_all():** Retrieves all phone records.
- **select_by_name(name):** Retrieves records based on a given name.
- **insert_record(record):** Inserts a new record into the dataset.
- **delete_by_name(name):** Deletes records based on a given name.

**Query Parsing**
- **parse_select(query):** Implements SELECT queries as specified in the problem statement.
- **parse_insert(query):** Implements INSERT queries as specified.
- **parse_delete(query):** Implements DELETE queries as specified.
- **execute_query(query):** Executes queries based on their types (SELECT, INSERT, DELETE).

## Guidelines Adherence
The code follows the following guidelines:

- Clean and documented code.
- Mostly adheres to PEP 8 style guidelines.
- Implements appropriate error handling for file not found errors.
## Testing
Thorough testing was conducted to ensure correct functionality. However, it's advisable to test with various inputs and edge cases for robustness.

## Contributing
Contributions are welcomed! Fork this repository, make changes, and create a pull request. Please ensure adherence to coding standards and provide clear commit messages.
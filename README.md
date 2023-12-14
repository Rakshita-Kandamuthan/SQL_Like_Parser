
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

To use this system, follow these steps:

### Setup
1. **Python Installation:** Ensure you have Python 3.x installed on your machine. If not, download and install Python from https://www.python.org/

2. **Clone the Repository:** Clone this repository to your local machine using the command:

       git clone https://github.com/Rakshita-Kandamuthan/SQL_Like_Parser

3. **Navigate to Directory:** Access the project directory:

       cd phone-book-management

4. **Modify File Path:** Open the **main.py file** and update the file_name variable to point to your specific CSV file containing phone book records:

       file_name = r"path/to/your/phone_records.csv"

### Running the Code
Once you've set up the project:

1. **Run the Program:** Execute the program in a Python environment by running:

       python main.py

2. **Interacting with the System:** After running the program, you can interact with the system by directly modifying the queries within the main.py file or by using the provided query examples in the code.

    
       query_1 = "SELECT * FROM phone_records;"  # Fetch all records
       query_2 = "SELECT * FROM phone_records WHERE name='Matthew Peters';"  # Fetch records by name
       query_3 = "INSERT INTO phone_records(name, email, phone_number1, phone_number2) VALUES('Test', 'test@test.xtyz', '1234456', '1233233');"  # Insert a new record
       query_4 = "DELETE FROM phone_records WHERE name='John';"  # Delete a record

3. **Executing Queries:** Modify or use the provided query examples within the main.py file. Uncomment or modify these queries as needed to perform CRUD operations on the phone book records.

4. **Review Output:** The system will display outputs based on the queries executed, such as fetched records, insertion success, or deletion confirmation.

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
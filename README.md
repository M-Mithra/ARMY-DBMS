# Army Database Management System (DBMS)

This project is a **Database Management System for Army personnel and logistics**. It provides SQL-based commands to manage soldiers, weapons, dependents, and zones efficiently. The system supports **CRUD operations**, inventory management, and analytical queries such as finding zones needing protection or calculating average weapon ranges.  

## Features
- SQL queries to manage **soldiers, dependents, weapons, and zones**.  
- Update operations (e.g., rank, room ID, weapon inventory).  
- Analytical queries (average weapon range, soldiers below a certain age, least protected zones).  
- Insertion of new data (new soldiers, dependents, and weapons).  
- Deletion operations (retirement, death, or age-based removal).  
- Support for authentication (logout command).  

## Requirements
- MySQL / PostgreSQL / SQLite (any SQL-compatible RDBMS).  
- Python 3.x (if integrating with a Python frontend).  
- Install required dependencies (if Python-based):  
  ```bash
  pip install mysql-connector-python psycopg2 sqlite3

## How to Run

1. Clone this repository and set up the database.

2. Import the provided SQL schema and sample data:

   ```bash
   mysql -u <username> -p < database_name < Data_SQL.sql
   ```

3. Run the Python interface (if provided):

   ```bash
   python PythonCode.py
   ```

4. Use the command menu to:

   * Update or delete soldiers
   * Insert weapons or zones
   * Run analysis queries (e.g., average weapon range, married soldiers)

## Project Structure

```
├── PythonCode.py       # Main script for interacting with DB
├── Data_SQL.sql        # SQL schema and dataset
├── Project_Report.pdf  # Detailed project report
└── README.md           # Project documentation
```

## Notes

* Each command is mapped to an SQL query (see README for full list).
* Supports **15+ commands**, including CRUD operations and analytical queries.
* Extendable: New queries and tables can be added for more features (e.g., missions, training).

Name : Gauri Hanumant Rasal
Company : CODTECH IT SOLUTIONS
ID : CTO8EHQ
Domain : SQL
Duration : DEC 2024 to JAN 2025
Mentor : Harish Neelam
# Employee Database Management System

## Overview
The **Employee Database Management System** is a SQL-based project designed to manage and organize employee data efficiently. It includes features for creating databases, managing employee records, performing queries, and modifying the database schema.

## Features
- **Database Creation**: Ensures the database is created only if it does not already exist.
- **Table Schema**: Creates an employee table with predefined fields and constraints.
- **Data Insertion**: Populates sample employee records.
- **Data Retrieval**: Queries for filtering and displaying employee data.
- **Data Manipulation**:
  - Update employee details.
  - Delete specific employee records.
- **Aggregation Queries**: Includes calculations like count, sum, average, min, and max.
- **Sorting and Filtering**: Retrieves ordered and filtered records based on specific conditions.
- **Schema Modification**: Demonstrates altering tables by dropping columns.

## Technologies Used
- **SQL**: Structured Query Language.
- **Database Server**: MySQL or MariaDB.

## Database Schema
```
EMPLOYEE(
    EMP_ID INT PRIMARY KEY,
    NAME VARCHAR(40) NOT NULL,
    EMAIL VARCHAR(40) NOT NULL,
    DEPT VARCHAR(20),
    JOB_POSITION VARCHAR(20) NOT NULL,
    SALARY DECIMAL(10,2) DEFAULT 30000.00,
    HIRED_DATE DATE NOT NULL DEFAULT CURRENT_DATE
)
```

## Setup Instructions
1. Install MySQL or MariaDB on your system.
2. Open a MySQL client or command-line interface.
3. Execute the script using:
   ```
   source employee_db_queries.sql;
   ```
4. Verify database creation with:
   ```sql
   SHOW DATABASES;
   USE EMP;
   SHOW TABLES;
   ```
5. Run queries provided in the script to test functionality.

## Usage Examples
1. Retrieve all employee records:
   ```sql
   SELECT * FROM EMPLOYEE;
   ```
2. Employees with salary above 55000:
   ```sql
   SELECT * FROM EMPLOYEE WHERE SALARY > 55000;
   ```
3. Count total employees:
   ```sql
   SELECT COUNT(*) FROM EMPLOYEE;
   ```
4. Retrieve employees whose name starts with 'U':
   ```sql
   SELECT * FROM EMPLOYEE WHERE NAME LIKE 'U%';
   ```

## Notes
- The database is set to create only if it does not already exist.
- Modify the sample data to meet your specific requirements.
- Ensure the database server is running before executing the script.

## Contributing
Contributions are welcome! Feel free to fork this repository, submit issues, or create pull requests.

## License
This project is licensed under the MIT License.

---
For questions or suggestions, please contact [gaurirasal2919@gmail.com].

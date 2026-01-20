<p align="center">
  <img src="https://content.presspage.com/uploads/2543/1920_purple-seal-unstoppable-bkg-1800x1200.png?10000" alt="Purple Seal Unstoppable" width="400"/>
</p>

# Module 6 – Database Initialization & Connectivity
*CSD 310 Database Development and Use*  
<sub>Bellevue University · Course Module Assignment</sub>

---

## Introduction
This module focuses on **initial database setup and basic database connectivity** using MySQL and Python. The assignment establishes the foundation for later database-driven applications by demonstrating how to create a database schema, populate initial data, and verify successful connections from an application layer.

The project emphasizes the **first step of any database-backed system**: ensuring that the database environment is correctly structured and accessible before performing queries or data manipulation.

---

## Key Features
- **Database Initialization Script** – Creates tables and initial data using SQL.
- **Schema Definition** – Establishes table structure and relationships.
- **Python Database Connectivity** – Verifies MySQL connection from Python.
- **Environment Validation** – Confirms credentials, host access, and database availability.

---

## Technologies Used
- **Language:** Python 3  
- **Database:** MySQL  
- **Scripts:**  
  - SQL schema initialization  
  - Python connection test  
- **Concepts:**  
  - Database creation  
  - Table initialization  
  - Client/server connectivity  
  - Environment verification  

---

## Getting Started (set up for local development)

Follow the steps below to set up and run this module locally.

### Prerequisites
- Python 3.x
- MySQL Server (running locally)
- Git

---

### 1. Clone the Repository
git clone https://github.com/WobbuWoop13/csd-310.git
cd csd-310

### 2. Initialize the Database

Use the SQL initialization script to create the database and tables:

mysql -u root -p < db_init_2022.sql

### 3. Install Required Python Package
pip install mysql-connector-python

### 4. Verify Database Connectivity

Run the Python test script:

python mysql_test.py

If successful, the script will connect to MySQL without errors, confirming that:

Credentials are valid

The database exists

Python can communicate with MySQL

### What the Scripts Do
db_init_2022.sql

Creates the database (if not already present)

Defines required tables and fields

Prepares the database for application use

mysql_test.py

Attempts a connection to the MySQL server

Confirms database accessibility from Python

Serves as a diagnostic tool before running more advanced scripts

### What I Learned

This module strengthened my understanding of:

How to initialize a database environment from scratch

The importance of validating database connectivity early

How Python applications communicate with MySQL

Preparing a clean database foundation for future development

### Known Limitations

Credentials are hardcoded for coursework purposes

No data querying or modification is performed

Output is limited to connection success or failure

### Future Improvements

Move credentials to environment variables (.env)

Add error handling and detailed logging

Add validation queries to confirm table creation

Expand initialization scripts to support versioning

### Author

Kyle Marlia-Conner
B.S. Software Development · Bellevue University
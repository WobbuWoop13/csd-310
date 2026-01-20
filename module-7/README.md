<p align="center">
  <img src="https://content.presspage.com/uploads/2543/1920_purple-seal-unstoppable-bkg-1800x1200.png?10000" alt="Purple Seal Unstoppable" width="400"/>
</p>

# Module 7 – Database Querying & Data Retrieval
*CSD 310 Database Development and Use*  
<sub>Bellevue University · Course Module Assignment</sub>

---

## Introduction
This module focuses on **querying and retrieving data from a relational MySQL database** using Python. The assignment works with a fictional **movies database** and demonstrates how structured SQL queries can be used to extract meaningful information from multiple tables.

The project emphasizes **read-only database operations**, preparing the foundation for more advanced CRUD workflows implemented in later modules.

---

## Key Features
- **Table Data Retrieval** – Queries full records from studio and genre tables.
- **Conditional Filtering** – Retrieves films with a runtime under two hours.
- **Sorting & Ordering** – Displays films grouped and ordered by director.
- **Structured Output** – Formats query results for clear, readable console display.
- **Error Handling** – Uses MySQL error codes to detect connection issues.

---

## Technologies Used
- **Language:** Python 3  
- **Database:** MySQL  
- **Library:** mysql-connector-python  
- **Concepts:**  
  - SELECT queries  
  - WHERE clauses  
  - ORDER BY sorting  
  - Relational table access  
  - Database connection handling  

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

### 2. Install Required Python Package
pip install mysql-connector-python

### 3. Verify Database Configuration

This script connects to an existing MySQL database named movies and expects the following tables:

studio

genre

film

Update the database connection settings in the script if needed:

config = {
    "user": "movies_user",
    "password": "YOUR_PASSWORD",
    "host": "127.0.0.1",
    "database": "movies"
}

### 4. Run the Script

From the module directory, run:

python Assignment_7_2.py

### What the Script Does

When executed, the script performs the following actions:

Connects to the MySQL movies database

Displays all records from the studio table

Displays all records from the genre table

Retrieves films with a runtime under 120 minutes

Displays film names and directors ordered alphabetically by director

The script pauses at the end, allowing users to review the output before exiting.

### What I Learned

This module strengthened my understanding of:

Writing effective SELECT queries

Filtering results using WHERE clauses

Sorting query results with ORDER BY

Structuring Python scripts for clean database access

Handling database connection errors gracefully

### Known Limitations

Database credentials are hardcoded

No data modification (read-only operations only)

Output is console-based with no user interface

### Future Improvements

Move credentials to environment variables (.env)

Add JOIN queries to combine related tables

Add pagination or result limits

Refactor repeated query logic into reusable functions

### Author

Kyle Marlia-Conner
B.S. Software Development · Bellevue University
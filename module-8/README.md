<p align="center">
  <img src="https://content.presspage.com/uploads/2543/1920_purple-seal-unstoppable-bkg-1800x1200.png?10000" alt="Purple Seal Unstoppable" width="400"/>
</p>

# Module 8 – Database CRUD Operations & JOIN Queries
*CSD 310 Database Development and Use*  
<sub>Bellevue University · Course Module Assignment</sub>

---

## Introduction
This module focuses on **core database CRUD operations** (Create, Read, Update, Delete) using Python and MySQL. The project works with a fictional **movies database** and demonstrates how to retrieve, insert, update, and delete records while maintaining relationships across multiple tables.

The assignment reinforces foundational database interaction patterns commonly used in real-world applications, including the use of **JOIN queries** to combine related data from multiple tables.

---

## Key Features
- **Read Operations** – Retrieves and displays movie data using INNER JOINs.
- **Create Operation** – Inserts a new film record into the database.
- **Update Operation** – Modifies an existing film’s genre.
- **Delete Operation** – Removes a film record from the database.
- **Formatted Output** – Displays query results in a structured, readable format.

---

## Technologies Used
- **Language:** Python 3  
- **Database:** MySQL  
- **Library:** mysql-connector-python  
- **Concepts:**  
  - CRUD operations  
  - SQL INNER JOINs  
  - Relational table design  
  - Transaction commits  

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
This script connects to an existing MySQL database named movies and assumes the following tables exist:

film

genre

studio

Update the database connection settings in the script if needed:

db = mysql.connector.connect(
    host="localhost",
    user="movies_user",
    password="YOUR_PASSWORD",
    database="movies"
)

### 4. Run the Script
From the module directory, run:
python Assignment_8_2.py

### What the Script Does
When executed, the script performs the following steps:

Displays all films using JOINs across film, genre, and studio tables

Inserts a new film record (Titan A.E.)

Displays films after insertion

Updates the genre of the film Alien

Displays films after the update

Deletes the film Gladiator

Displays films after deletion

Each step prints results to the console to verify successful database operations.

### What I Learned
This module strengthened my understanding of:

Performing full CRUD workflows against a relational database

Writing SQL JOIN queries to combine related data

Managing database transactions using commits

Structuring Python scripts to clearly demonstrate database state changes

### Known Limitations
Database credentials are hardcoded

No user interface is included

Error handling is minimal and focused on instructional outcomes

### Future Improvements
Move credentials to environment variables (.env)

Add input validation and error handling

Separate CRUD operations into reusable functions

Add logging instead of console print statements

### Author
Kyle Marlia-Conner
B.S. Software Development · Bellevue University
<p align="center">
  <img src="https://content.presspage.com/uploads/2543/1920_purple-seal-unstoppable-bkg-1800x1200.png?10000" alt="Purple Seal Unstoppable" width="400"/>
</p>

# Module 10 – Relational Database Design & Implementation
*CSD 310 Database Development and Use*  
<sub>Bellevue University · Course Module Assignment</sub>

---

## Introduction
This module focuses on the **design and implementation of a relational MySQL database** using Python. The assignment simulates a small business environment for a wine production and distribution company, requiring the creation of multiple related tables, enforcement of foreign key constraints, and population of realistic sample data.

The project demonstrates how database schemas can be programmatically created and managed using Python, reinforcing database-first design principles and proper handling of relational dependencies.

---

## Key Features
- **Programmatic Database Creation** – Automatically creates a MySQL database from Python.
- **Relational Schema Design** – Eight interconnected tables modeling employees, inventory, products, and sales.
- **Foreign Key Constraints** – Enforces data integrity between related entities.
- **Automated Data Population** – Inserts realistic sample data into each table.
- **Verification Output** – Displays tables, columns, and records to confirm successful execution.

---

## Technologies Used
- **Language:** Python 3  
- **Database:** MySQL  
- **Connector:** mysql-connector-python  
- **Concepts:**  
  - Relational database design  
  - Primary and foreign keys  
  - ENUM constraints  
  - Data integrity enforcement  

---

## Getting Started (set up for local development)

Follow the steps below to set up and run this module locally.

### Prerequisites
- Python 3.x
- Git
- MySQL Server (running locally)

---

### 1. Clone the Repository
git clone https://github.com/WobbuWoop13/csd-310.git
cd csd-310

### 2. Install Required Python Package
pip install mysql-connector-python


Note: This only needs to be done once per environment.

### 3. Update MySQL Credentials

Open the Python script for this module and update the MySQL connection configuration:

config = {
    'user': 'root',
    'password': 'YOUR_PASSWORD_HERE',
    'host': 'localhost',
}

### 4. Run the Script

From the module directory, run:

python FinalTest\ 2.py

### 5. What Happens When the Script Runs

When executed, the script will:

Create a MySQL database

Drop existing tables (if present)

Create all tables with defined schemas

Apply foreign key constraints

Insert sample data into each table

Display:

All tables in the database

Column definitions

All records in each table

This output confirms both schema correctness and successful data insertion.

### Database Schema Overview

The database models a simplified winery operation using the following entities:

Employee – Staff members and assigned roles

Department – Organizational structure

GrapeVariety – Grape types used in wine production

Wine – Finished wine products

Supplier – Vendors providing materials

Inventory – Raw materials and finished goods

Distributor – External sales partners

Sales – Sales transactions

Foreign key relationships ensure logical connections between employees, inventory, wines, distributors, and sales records.

### What I Learned

This module strengthened my understanding of:

Translating ERD diagrams into executable SQL

Managing foreign key dependencies during schema creation

Automating database setup and validation using Python

Designing relational schemas that reflect real-world business logic

### Known Limitations

Database credentials are hardcoded for coursework purposes

No graphical interface; interaction is via console output

Error handling is minimal and focused on learning outcomes

### Future Improvements

Move credentials to environment variables (.env)

Separate schema creation and data population into different scripts

Add reporting queries (sales totals, inventory summaries)

Include an ERD image in the README

### Author

Kyle Marlia-Conner
B.S. Software Development · Bellevue University
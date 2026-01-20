<p align="center">
  <img src="https://content.presspage.com/uploads/2543/1920_purple-seal-unstoppable-bkg-1800x1200.png?10000" alt="Purple Seal Unstoppable" width="400"/>
</p>

# Module 11 – Database Reporting & Analysis System
*CSD 310 Database Development and Use*  
<sub>Bellevue University · Course Module Assignment</sub>

---

## Introduction
This module focuses on **database-driven reporting and analysis** using Python and MySQL. The project is based on a fictional **Bacchus Winery** production and distribution business and demonstrates how structured database queries can be transformed into meaningful business reports.

The system generates multiple reports that support decision-making related to **sales performance**, **inventory levels**, and **employee work hours**, reinforcing real-world database usage patterns commonly found in enterprise environments.

---

## Key Features
- **Relational Database Setup** – Programmatic creation of the Bacchus Winery MySQL database.
- **Sales Performance Reporting** – Aggregates sales data by wine type.
- **Inventory Status Reporting** – Displays current raw material and finished product levels.
- **Employee Work Hours Reporting** – Summarizes employee work hour data.
- **Data Analysis Tools** – Uses Pandas for query results and Matplotlib for visualization.

---

## Technologies Used
- **Language:** Python 3  
- **Database:** MySQL  
- **Libraries:**  
  - mysql-connector-python  
  - pandas  
  - matplotlib  
- **Concepts:**  
  - SQL joins and aggregation  
  - Database reporting  
  - Data analysis and visualization  
  - Business intelligence fundamentals  

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

### 2. Install Required Python Packages
pip install mysql-connector-python pandas matplotlib

### 3. Create the Database

Run the database setup script to create and populate the Bacchus Winery database:

python Bacchus_Winery.py


This script:

Creates the bacchus_winery database

Builds all required tables

Inserts sample business data

### 4. Run the Reports
Sales Performance Report
python sales_perforamce.py


Displays total quantity sold and sales amount per wine type

Generates a bar chart visualization

Inventory Status Report
python Inventory_status.py


Displays current inventory levels for raw materials and finished products

Employee Work Hours Report
python Work_Hour.py


Displays employee work hour summaries

### Reports Overview
Sales Performance Report

Provides insight into which wine products generate the most revenue and sales volume, helping guide production and marketing strategies.

Inventory Status Report

Displays inventory quantities to ensure production readiness and assist with supply planning.

Employee Work Hours Report

Summarizes employee work hours to support productivity tracking and workforce management.

### What I Learned

This module strengthened my understanding of:

Writing SQL queries that support business reporting

Using Python to transform raw database data into readable reports

Applying data analysis libraries (Pandas, Matplotlib) to database results

Structuring reporting systems similar to real-world business intelligence tools

### Known Limitations

Database credentials are hardcoded for coursework purposes

Reports are generated via console output and static charts

No user interface or authentication layer is implemented

### Future Improvements

Move credentials to environment variables (.env)

Add a menu-driven or GUI interface for report selection

Export reports to CSV or PDF formats

Add automated database validation checks

Improve error handling and logging

### Contributors
Role	Name
Developer	Kyle Marlia-Conner
Developer	Steve Stylin
Developer	Ean Masoner
Developer	Cuitlahuac Hernandez
Developer	Mirajo Tesora
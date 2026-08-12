# Lab: Database SQL Basics

**Role:** Pre-Security Student / Data Security Trainee

## 🎯 Objective
To understand the foundational architecture of relational databases (tables, columns, rows) and master fundamental Structured Query Language (SQL) commands to securely retrieve, filter, and sort data without altering the underlying database structure.

## 🚀 Execution Steps
1. **Relational Database Architecture Analysis:** 
   * Analyzed how databases systematically store data within structured formats known as **Tables**, which are organized into distinct columns and rows.
2. **Data Retrieval & Filtering (SELECT & WHERE):** 
   * Formulated and executed SQL queries using the `SELECT` statement to target and retrieve specific data points from the database.
   * Applied the `WHERE` clause to filter the extracted data based on precise conditional logic, narrowing down the results to match specific investigation criteria.
3. **Data Sorting & Presentation (ORDER BY):** 
   * Utilized the `ORDER BY` command to logically sort the queried results (e.g., sorting items incrementally from cheapest to most expensive).
   * Verified that the executed queries performed read-only operations, successfully extracting information without making unauthorized modifications to the database records.

## 📊 Results & Evidence
* Successfully queried a simulated relational database, applied logical filters to locate specific records, and sorted the output for efficient analysis using standard SQL commands.

> 📸 <br><img width="1081" height="809" alt="image" src="https://github.com/user-attachments/assets/bfc66347-a5fc-48b9-b436-fded2a38d293" />

> 📸 <br><img width="1051" height="770" alt="image" src="https://github.com/user-attachments/assets/64432bc5-2ce1-4f66-a776-06274e29f8a2" />

## 🧠 Key Takeaways
* **SQL as an Investigation Tool:** Learned that SQL is not just for database administrators; it is a critical tool for security analysts to quickly search through massive datasets and logs stored in relational databases.
* **Tables are the Core:** Understood the fundamental concept that all data within a relational database is stored systematically inside Tables, making it highly organized and searchable.
* **Read-Only Queries:** Recognized that utilizing standard `SELECT` statements allows an analyst to safely pull and analyze data (such as finding the cheapest items) without the risk of accidentally altering or deleting the actual database records.

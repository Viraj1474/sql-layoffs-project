# SQL Data Cleaning Project - Layoffs Dataset

## 📌 Project Overview
This project focuses on **data cleaning using SQL**.  
The dataset contains information about company layoffs, and the goal of this project was to transform messy, inconsistent data into a clean, analysis-ready format.  

All steps were executed in **MySQL Workbench**.

---

## 🔧 Key Data Cleaning Steps
1. **Removed Duplicates**  
   - Used `ROW_NUMBER()` to identify duplicate rows.  
   - Kept only one record per duplicate group.

2. **Standardized Data**  
   - Trimmed extra spaces in text columns.  
   - Standardized company names and industry categories.  

3. **Handled Null / Missing Values**  
   - Replaced `NULL` values with appropriate defaults where possible.  
   - Dropped rows where critical fields were missing.

4. **Corrected Data Types**  
   - Converted text-based numeric fields into integers/floats.  
   - Ensured dates were in proper `DATE` format.  

5. **Created Clean Final Table**  
   - Stored the cleaned data into a new table for future analysis.  

---

## 📂 Files in this Repository
- **`laysoff_project.sql`** → SQL script containing all queries used for cleaning the dataset.  
- **`README.md`** → Project documentation.  

---

## ▶️ How to Run
1. Open **MySQL Workbench** (or any MySQL client).  
2. Import the SQL script:
   ```sql
   SOURCE laysoff_project.sql;

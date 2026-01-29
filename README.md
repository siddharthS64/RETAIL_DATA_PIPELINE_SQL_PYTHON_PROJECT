# 🛒 Retail Orders Data Analysis & ETL Pipeline

## 📌 Project Overview

This project demonstrates an end-to-end data engineering and analytics workflow, covering the complete lifecycle from data ingestion to business insight generation. It involves extracting raw retail order data using the Kaggle API, performing extensive data cleaning and feature engineering with Python, loading the refined dataset into MySQL, and executing advanced SQL queries to answer key business questions related to revenue growth and product performance.

## 🎯 Objectives

- Automate data ingestion from an external source (Kaggle)

- Clean and standardize raw data for database storage

- Engineer meaningful features for deeper analysis

- Load processed data into MySQL using SQLAlchemy

- Generate actionable business insights using advanced SQL

## 🛠️ Tech Stack

**Programming Language**

  - Python

**Libraries**

  - Pandas

  - NumPy

  - SQLAlchemy

  - PyMySQL

  - Zipfile

**Database**

  - MySQL

**Data Source**

  - Kaggle API

## 📂 Project Workflow
### 1️⃣ Data Ingestion & Preprocessing

- **API Extraction:** Downloaded the dataset dynamically using the Kaggle API and extracted the CSV file from a zip archive.

- **Handling Null Values:** Replaced "Not Available" and "unknown" values with proper nulls during ingestion.

- **Column Standardization:** Converted column names to lowercase and replaced spaces with underscores to ensure database compatibility.

- **Data Typing:** Transformed the order_date column from object type to datetime format.

### 2️⃣ Feature Engineering

To enhance analytical depth, the following calculated columns were created:

- **Discount:**
    list_price * discount_percent * 0.01

- **Sale Price:**
    list_price - discount

- **Profit:**
    sale_price - cost_price

### 3️⃣ Database Loading

- Established a connection to MySQL using SQLAlchemy.

- Loaded the processed dataset into a table named sales_data using append or replace methods.

## 📊 Business Insights (SQL Analysis)

Advanced SQL techniques such as CTEs, Window Functions, and Pivot Tables were used to derive the following insights:

- **Top 10 Revenue Generators:** Identified the highest-grossing products globally.

- **Regional Performance:** Determined the top 5 selling products within each region.

- **Year-over-Year Growth:** Compared monthly sales between 2022 and 2023 to uncover seasonal trends.

- **Peak Category Performance:** Found the month with the highest sales for each product category.

- **Growth Leader:** Identified the sub-category with the highest profit growth in 2023 compared to 2022.

## 🚀 How to Use
### 1️⃣ Configure Kaggle API

  - Place your kaggle.json file in the appropriate directory.

  - Ensure Kaggle API access is enabled.

### 2️⃣ Database Setup

  - Create a MySQL database.

  - Update the connection string in the notebook with:

    - MySQL username

    - Password

    - Database name

### 3️⃣ Run ETL Pipeline

  - Execute orders data analysis.ipynb to:

    - Download data

    - Clean and process it

    - Load it into MySQL

### 4️⃣ Run SQL Analysis

  - Open sql+python EDA project.sql in your SQL editor.

  - Execute queries to generate business insights.

## 📈 Key Takeaways

  - Built a fully automated ETL pipeline using Python

  - Applied data engineering best practices for cleaning and transformation

  - Demonstrated advanced SQL analytics skills

  - Delivered actionable insights for retail business decision-making

## 🔗 Connect With Me

If you’d like to discuss this project or collaborate on data analytics work, feel free to connect!

- **LinkedIn:** [Siddharth Sharma](https://www.linkedin.com/in/siddharthsh64)

- **Email:** [siddharthsh064@gmail.com](mailto:siddharthsh064@gmail.com)

---

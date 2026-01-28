# 🎬 Netflix Data Analytics Pipeline using dbt Cloud & Snowflake

## 📌 Project Overview
This project demonstrates an end-to-end analytics engineering pipeline built using **dbt Cloud** and **Snowflake**.  
The goal is to transform raw Netflix data into analytics-ready tables using modern data engineering best practices.

The pipeline follows the **Medallion Architecture (Bronze → Silver → Gold)** to ensure scalable, maintainable, and high-quality analytics models.



## 🏗️ Architecture

Raw Data (CSV / S3)
↓
Bronze Layer (Staging Models)
↓
Silver Layer (Clean & Transformed Data)
↓
Gold Layer (Business & Analytics Models)
↓
Snowflake Analytics / Dashboard


## 🛠️ Tech Stack

- **dbt Cloud** – Data transformation & modeling
- **Snowflake** – Data warehouse
- **GitHub** – Version control
- **SQL** – Transformations
- **CSV / S3** – Raw data source


## 🔄 Data Pipeline Explanation

### 1️⃣ Bronze Layer (Staging)
- Loads raw Netflix data into Snowflake
- Performs basic cleaning:
  - Remove null values
  - Standardize column names
  - Type casting

### 2️⃣ Silver Layer (Transformation)
- Business logic applied:
  - Aggregations (ratings, movies, users)
  - Joins between datasets
  - Data normalization

### 3️⃣ Gold Layer (Analytics)
- Final analytics tables created:
  - Movie performance metrics
  - User behavior insights
  - Rating trends
- These tables are optimized for dashboards and reporting.

## ▶️ How to Run the Project

```bash
dbt run
dbt test
````

## 🚀 Future Enhancements

* Connect real-time data source (API / streaming)
* Build dashboards using Power BI / Tableau / Snowflake
* Implement CI/CD for dbt models
* Add more data quality tests
* Deploy on AWS S3 / Airflow orchestration
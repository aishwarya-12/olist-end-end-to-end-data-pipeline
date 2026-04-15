## Olist End-to-End Data Pipeline 🚀

## 📌 Overview

This project implements a modern end-to-end data pipeline using the Olist e-commerce dataset. It focuses on building a scalable ETL workflow with incremental data processing, loading curated data into Snowflake, and enabling analytics on top of a structured data model.

---

## 🛠️ Tech Stack

* Databricks (Apache Spark)
* Snowflake (Data Warehouse)
* Python (PySpark, Pandas)

---

## 🔄 Pipeline Architecture

```
Raw Data → Bronze Layer → Silver Layer → Gold Layer → Snowflake → Analytics
```

* **Bronze Layer**: Raw ingestion of Olist dataset
* **Silver Layer**: Data cleaning, transformations, and joins
* **Gold Layer**: Aggregated and business-ready data
* **Snowflake**: Final storage for analytics and querying

---

## ⚙️ Key Features

* End-to-end ETL pipeline using Databricks
* Incremental data loading using timestamp-based filtering
* Efficient upsert operations using MERGE logic
* Structured data modeling for analytics
* Scalable and modular pipeline design

---

## 🔁 Incremental Data Processing

This project implements incremental loading to improve performance and avoid full data reloads.

* Tracks last processed timestamp
* Processes only new or updated records
* Uses MERGE operations to handle inserts and updates
* Reduces compute cost and improves efficiency

---

## 📊 Dataset

* Olist E-commerce Dataset (Brazilian marketplace data)
* Includes orders, customers, products, payments, and reviews

---

## 📁 Project Structure

```
olist-end-to-end-data-pipeline/
│
├── notebooks/        # Databricks notebooks (ETL, EDA)
├── src/              # ETL scripts (extract, transform, load)
├── snowflake/        # SQL scripts for schema and loading
├── data/             # Sample data (not full dataset)
├── README.md
└── requirements.txt
```

---

## 🚧 Project Status

Work in progress – currently implementing ETL pipeline and incremental data loading.

---

## 🚀 Future Enhancements

* Add advanced analytics and dashboards
* Implement ML models for predictive insights
* Automate pipeline with scheduling (Airflow / Databricks Jobs)

---


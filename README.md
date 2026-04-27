# 🚀 Databricks Incremental Data Pipeline

## 📌 Overview

This project demonstrates a real-world data engineering pipeline using Databricks and Delta Lake, implementing incremental data ingestion with MERGE INTO.

## 🧱 Architecture

Medallion Architecture:

* 🥉 Bronze: Raw data ingestion from CSV
* 🥈 Silver: Cleaned and deduplicated data
* 🥇 Gold: Aggregated business metrics

## ⚙️ Technologies

* Databricks
* Apache Spark (SQL & PySpark)
* Delta Lake

## 🔄 Pipeline

### Bronze Layer

* Ingest raw Walmart sales data from CSV

### Silver Layer

* Incremental processing using MERGE INTO
* Deduplication based on (Store, Date)

### Gold Layer

* Aggregated metrics:

  * Total sales per store
  * Sales by year

## 📊 Dashboard

Databricks SQL dashboard with:

* Revenue KPIs
* Sales trends
* Store performance

## 📸 Screenshots

<img width="1410" height="744" alt="dashbord-warmart project" src="https://github.com/user-attachments/assets/3eecac9b-03cc-434d-89d0-bd69f7a4c3d0" />

## 💡 Key Concepts

* Incremental ingestion
* Idempotent pipeline
* Delta Lake MERGE

## 🚀 Future Improvements

* Streaming ingestion
* Data quality checks
* Orchestration (Airflow)

# **Walmart Customer Purchases ETL Project**

## 📌 Project Overview

This project demonstrates the design and implementation of a robust ETL pipeline for processing Walmart customer purchase data extracted from Kaggle using the Medallion Architecture (Bronze → Silver → Gold layers) in Databricks. 
The goal is to efficiently ingest raw transactional data, apply data cleaning and transformation, and prepare curated analytical datasets that enable reporting on customer behavior, product performance, and sales trends.

## 🎯 Project Goals

•	Build an end-to-end ETL pipeline to process large-scale customer purchase data.

•	Apply data cleaning, deduplication, and enrichment to improve data quality.

•	Implement Incremental Data Loading to process only new/changed records.

•	Apply Slowly Changing Dimensions (SCD) Type 2 for maintaining historical changes.

•	Create gold-layer fact and dimension tables optimized for analytics.

•	Orchestrate and monitor pipeline execution using Databricks Lakeflow Jobs.

## 🏗️ Architecture

The pipeline follows the Medallion Architecture pattern:

🥉	Bronze Layer – Stores raw ingested purchase data using Delta Live Tables.

🥈	Silver Layer – Cleansed and standardized data (deduplication, data type corrections, incremental load).

🥇	Gold Layer – Business-ready fact and dimension tables for analytics (FactPurchases, DimCustomers with SCD2, DimProducts with SCD2, DimDate, DimPayments).

## ⚙️ Technologies & Tools Used

✅	Databricks – Unified platform for ETL and orchestration

✅	PySpark – Distributed data processing

✅	Delta Lake – ACID compliant storage format

✅	Databricks Lakeflow Jobs – Orchestration and scheduling





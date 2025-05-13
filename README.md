# 🚴‍♀️ RideWise: End-to-End Azure Data Engineering Project

**RideWise** is a data engineering project that analyzes bike sales data using the Medallion Architecture on Microsoft Azure. It demonstrates how to design a scalable analytics pipeline with technologies like Azure Data Factory, Azure Databricks, Azure Data Lake Storage (Gen2), Azure Synapse Analytics, and Power BI.

---

## 📊 Project Overview

This project takes you through the lifecycle of building a modern data platform using Azure services. It involves ingesting raw sales data, transforming it into curated insights using PySpark, storing it in a structured format, and visualizing it with Power BI for decision-making.

---

## 📌 Key Objectives

- Design a robust ETL pipeline using Azure-native tools.
- Apply the **Medallion Architecture**: Bronze → Silver → Gold layers.
- Analyze trends in bike sales, customer behavior, and regional performance.
- Build a Power BI dashboard for business users.

---

## 📈 Use Cases

- Track yearly and monthly bike sales performance.
- Analyze customer segments and return rates.
- Compare regional and product-category sales.
- Identify high-performing territories and trends.

---

## 🔧 Tools & Technologies

| Layer               | Technology                            |
|--------------------|----------------------------------------|
| Ingestion          | Azure Data Factory (ADF)              |
| Storage            | Azure Data Lake Storage Gen2 (ADLS)   |
| Processing         | Azure Databricks (PySpark)            |
| Warehouse Layer    | Azure Synapse Analytics (SQL Pools)   |
| Visualization      | Power BI                              |
| Orchestration      | Azure Data Factory Pipelines          |

---

## 🏗️ Architecture

               +------------------+
               | GitHub Dataset   |
               +------------------+
                        |
                        v
        +-----------------------------+
        | Azure Data Factory (Ingest) |
        +-----------------------------+
                        |
                        v
     +----------------------------------------+
     | Azure Data Lake (Bronze / Raw Layer)   |
     +----------------------------------------+
                        |
                        v
     +----------------------------------------+
     | Azure Databricks (Silver / Cleaned)    |
     +----------------------------------------+
                        |
                        v
     +----------------------------------------+
     | Azure Databricks (Gold / Aggregated)   |
     +----------------------------------------+
                        |
                        v
         +-----------------------------+
         | Azure Synapse SQL Analytics |
         +-----------------------------+
                        |
                        v
              +------------------+
              | Power BI Reports |
              +------------------+

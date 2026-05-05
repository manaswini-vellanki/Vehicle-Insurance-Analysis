# 🚗 Vehicle Insurance Claims Analytics Platform

## 📌 Overview
This project builds a data engineering pipeline on Databricks to process vehicle insurance data. It transforms raw datasets into structured insights for claims analysis and business reporting.

---

## 🏗️ Architecture
The solution follows the Medallion Architecture:

- **Bronze Layer** → Stores raw ingested data  
- **Silver Layer** → Cleans, validates, and standardizes data  
- **Gold Layer** → Generates KPIs and analytics-ready datasets  

---

## 🔄 Data Pipeline
Data flows through multiple stages:

1. Raw data is ingested into the Bronze layer  
2. Data is cleaned and transformed in the Silver layer  
3. Aggregations and KPIs are created in the Gold layer  

---

## ⚙️ Key Features
- Supports batch and streaming data processing  
- Performs data validation and cleaning  
- Implements fact and dimension data modeling  
- Generates business KPIs for reporting  
- Uses SCD Type 2 for historical tracking  
- Ensures secure data access using Unity Catalog  

---

## 🧩 Data Model
- **Fact Table**
  - `fact_claims` → Stores transactional claim data  

- **Dimension Tables**
  - `dim_customers` → Customer details and history  
  - `dim_policies` → Policy information and updates  
  - `dim_vehicles` → Vehicle-related attributes  

---

## 📊 KPIs
- Total number of claims  
- Average claim amount  
- Claim settlement rate  
- High-risk customer identification  

---


## Execution Steps
1. Load data  
2. Run Bronze  
3. Run Silver  
4. Run Gold  

## Future Scope
- Fraud detection using ML  
- Advanced analytics  

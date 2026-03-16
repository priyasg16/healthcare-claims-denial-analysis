# Healthcare Claims Integrity & Provider Performance Analysis

## 🏥 Project Overview
This repository contains an end-to-end data engineering and BI solution designed to analyze **3.15 GB of CMS Medicare Physician & Other Practitioners data**. The project identifies financial leakage by evaluating the variance between provider billing and actual Medicare payments.

## 🏗️ Architecture & Data Flow
The pipeline follows a professional **Star Schema** architecture:
1. **Ingestion:** Raw CMS datasets are hosted in **AWS S3** and ingested via Alteryx.
2. **Cleaning:** Technical CMS variables are normalized and mapped to professional Business Semantic names.
3. **Modeling:** Cleaned data is loaded into a **SQL Server Star Schema** (Fact & Dimension tables).
4. **Visualization:** Insights are surfaced via **Power BI**.

## 📊 Key Business Insights
* **Financial Leakage:** Quantifying the dollar-amount variance between `Avg_Billed_Amount` and `Avg_Paid_Amount`.
* **Provider Specialty Benchmarking:** Ranking specialties by service volume and payment variance.
* **Geographic Analysis:** Identifying regional trends in Medicare payment rates.
* **Operational Efficiency:** Analyzing impact of 'Facility' vs. 'Non-Facility' settings.

## 🛠️ Tech Stack
- **ETL:** Alteryx (Advanced Workflow Design)
- **Database:** SQL Server (Star Schema, Physical Modeling)
- **Visualization:** Power BI (DAX, Interactive Dashboards)
- **Cloud Storage:** AWS S3 ("Landing Zone" for raw data)

## 🚀 Getting Started & Prerequisites
* **Alteryx Designer:** (Required for ETL execution).
* **SQL Server 2022:** (For database hosting).
* **Power BI Desktop:** (For rendering final dashboard).
* **AWS S3 Access:** (Configured as the primary data lake landing zone).

# Healthcare Claims Integrity & Provider Performance Analysis

**Date:** January 15, 2026  
**Project Lead:** Priyanka saki gajendran
**Stakeholder:** Director, Provider Network Operations

## 🏥 Project Overview
This repository contains an end-to-end data engineering and BI solution designed to analyze **3.15 GB of CMS Medicare Physician & Other Practitioners data**. The project identifies financial leakage by evaluating the variance between provider billing and actual Medicare payments.

## 🛠️ Tech Stack
- **ETL:** Alteryx (Advanced Workflow Design & Automation)
- **Database:** SQL Server (Star Schema, Physical Modeling)
- **Programming:** Python (Outlier Detection)
- **Visualization:** Power BI (DAX, Interactive Dashboards)
- **Methodology:** Agile (Task-based documentation)

## 📐 Architecture & Data Flow
The pipeline follows a professional **Star Schema** architecture to ensure data integrity and query performance:
1. **Ingestion:** Loading 3.1 GB raw CMS CSV via Alteryx.
2. **Cleaning:** Renaming technical CMS variables to Business Semantic names.
3. **Modeling:** Loading data into a SQL Server Star Schema.
4. **Visualization:** Power BI dashboard for Executive Network Operations.

## 🚀 Scaling to the Cloud (Preferred Skills)
To align with enterprise requirements, this local architecture is designed to scale:
- **Storage:** Transition to **Azure Data Lake Gen2** or **AWS S3**.
- **Computing:** Use **Azure Data Factory** or **Alteryx Server** for automation.
- **Warehouse:** Migration to **Snowflake** or **Azure Synapse**.

## 📂 Repository Structure
- `/docs`: Project Charter and Data Dictionary.
- `/sql`: DDL scripts for Star Schema creation.
- `/alteryx`: .yxmd workflow files.
- `/power-bi`: .pbix dashboard templates.

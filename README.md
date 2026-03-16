# Healthcare Claims Integrity & Provider Performance Analysis

## 🚀 Executive Summary
The **Healthcare Claims Integrity & Provider Performance Analysis** initiative was launched to mitigate financial leakage within the CMS Medicare provider network. By leveraging a high-volume dataset (3.15 GB), this project engineered a scalable ETL pipeline to automate the identification of billing variances between "Submitted Charges" and "Actual Medicare Reimbursements." 
This solution establishes a "Single Source of Truth," enabling data-driven decision-making for network leadership by benchmarking provider performance against national specialty and geographic standards.

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

  ## 📂 Repository Structure
- `/docs`: Project Charter and Data Dictionary.
- `/sql`: DDL scripts for Star Schema creation.
- `/alteryx`: .yxmd workflow files.
- `/power-bi`: .pbix dashboard templates.

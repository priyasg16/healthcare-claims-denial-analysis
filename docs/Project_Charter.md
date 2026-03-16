# Project Charter: Healthcare Claims Integrity

**Date:** March 16, 2026  
**Project Lead:** Priyanka Saki Gajendran  
**Stakeholder:** Director, Provider Network Operations  

## 1. Project Objectives
* **Identify Financial Leakage:** Analyze the variance between billed charges and Medicare payments.
* **Optimize Provider Network:** Evaluate provider performance by specialty and geography.
* **Automate Data Engineering:** Build a repeatable pipeline to handle multi-gigabyte healthcare datasets.

## 2. Success Criteria
1. **Technical:** Successful ingestion and cleaning of the 3.15 GB source file.
2. **Analytical:** Identification of the top 5 specialties with the highest payment variance.
3. **Delivery:** Functional Power BI dashboard serving as a "Single Source of Truth."

## 3. Data Dictionary Mapping
| Raw Variable (CMS) | Business Name (SQL/BI) | Logic |
| :--- | :--- | :--- |
| `Rndrng_NPI` | `Provider_NPI` | Unique Identifier for provider. |
| `Rndrng_Prvdr_Type` | `Provider_Specialty` | Derived specialty. |
| `Avg_Sbmtd_Chrg` | `Avg_Billed_Amount` | Total billed by provider. |
| `Avg_Mdcr_Pymt_Amt` | `Avg_Paid_Amount` | Actual Medicare payment. |

## 4. Repository Structure
- `/docs`: Project Charter and Data Dictionary.
- `/sql`: DDL scripts for Star Schema creation.
- `/alteryx`: .yxmd workflow files.
- `/power-bi`: .pbix dashboard templates.

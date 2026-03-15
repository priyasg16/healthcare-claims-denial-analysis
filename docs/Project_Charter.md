# Project Charter: Claims Integrity & Provider Network Optimization

**Date:** March 15, 2026  
**Project Lead:** [Your Full Name]  
**Stakeholder:** Director, Provider Network Operations

---

## 1. Business Objective
To identify operational inefficiencies in provider billing practices that contribute to high claim denial rates. This project aims to pinpoint "leakage" in the claims adjudication process, enabling the Provider Relations team to deploy targeted provider education and reduce administrative rework.

## 2. Key Business Questions
* **What is the denial rate** across different provider specialties?
* **Which denial reason codes** are the primary drivers of administrative cost?
* **Are there specific geographic clusters** or high-volume providers that disproportionately contribute to claim denials?

## 3. Success Metrics (KPIs)
* **Primary Metric:** Percentage of "clean claims" (claims submitted without errors) across top-tier provider specialties.
* **Secondary Metric:** Reduction in the average time-to-resolution for denied claims.

## 4. Scope & Methodology
* **In-Scope:** Ingestion of CMS Medicare Provider Utilization data; data cleaning and validation; analysis of specialty-specific denial patterns; development of an interactive performance dashboard.
* **Out-of-Scope:** Longitudinal patient clinical outcomes; non-Medicare commercial insurance data.

## 5. Technology Stack
* **Ingestion:** SQL Server Integration Services (SSIS)
* **Data Cleaning:** Python (Pandas)
* **Modeling:** SQL Server (Star Schema)
* **Transformation:** Alteryx (for data blending and logic)
* **Visualization:** Power BI

## 6. Data Integrity & Ethics
* **Compliance:** This project utilizes publicly available, de-identified datasets from the Centers for Medicare & Medicaid Services (CMS). No Protected Health Information (PHI) is included.
* **Assumptions:** We assume `Denial_Reason_Code` is consistently populated. All outlier billing amounts (e.g., >$100,000) have been flagged for manual verification.

# 🧰 End-to-End Data Engineering Pipeline — FinTech Loans & Customers

A full-scale, multi-milestone data engineering project delivering a complete **ingestion → cleaning → transformation → feature engineering → orchestration → analytics → visualization** pipeline for a large FinTech dataset. The workflow integrates Python, Docker, PostgreSQL, PySpark, and Airflow, and concludes with an interactive analytics dashboard and business-ready insights.

---

## 🚀 Project Overview

This project implements a production-grade data pipeline for a FinTech dataset containing **customers, loans, income, and risk indicators**. The workflow covers:

* In-depth **Exploratory Data Analysis (EDA)**
* Full **data cleaning and preprocessing**
* **Feature engineering & categorical encoding**
* **Metadata tracking** with a programmatic lookup table
* **Containerized ETL** with Docker & Docker Compose
* **PostgreSQL data warehousing & analytical SQL**
* **PySpark-based scalable transformations**
* **Airflow orchestration** with automated DAGs
* **Interactive Dash dashboard** for insight communication

---

## 🧹 Data Cleaning & Preprocessing

* Standardized column names and fixed inconsistent labels
* Resolved duplicates and missing values using documented imputation strategies
* Detected and evaluated the impact of outliers
* Normalized and encoded categorical features (Label Encoding & One-Hot Encoding)
* Engineered multiple features including:

  * **Month number**
  * **Loan installment amounts**
  * **Salary-coverage boolean flag**
  * **Letter grading system**

---

## 📒 Lookup Table for Data Lineage

Created a fully programmatic **lookup table** tracking:

* All imputations
* All encoded categorical mappings
* Outlier replacements
* Any reversible transformations

Ensures **transparency, reproducibility, and data reversibility** across the pipeline.

---

## 🐳 Containerized ETL with Docker

* Converted notebooks into modular Python scripts
* Built a Docker image to run the entire cleaning pipeline
* Used **Docker Compose** to orchestrate:

  * Python ETL container
  * PostgreSQL database
  * Volume-mounted persistent storage
* Automated loading of:

  * Cleaned datasets
  * Lookup tables

---

## 🗃️ PostgreSQL Analytics

Designed SQL workflows to answer key business questions involving:

* Loan trends
* Customer state-wise patterns
* Grade distribution
* Risk and default indicators

---

## ⚡ PySpark Milestone — Scalable Data Processing

Using Parquet inputs, executed:

* Null handling at scale
* Categorical encoding
* Advanced feature engineering (historical loan metrics by **grade** & **state**)
* Side-by-side **SQL vs Spark** analytical comparisons
* Exported all Spark-cleaned data and lookup tables back to Parquet

---

## 🛠️ Workflow Orchestration with Apache Airflow

Built DAGs that automate:

```
Raw Data → Cleaning → Feature Engineering → Loading into PostgreSQL
```

Includes retries, scheduling, task dependencies, and modular Python operators.

---

## 📊 Interactive Dash Dashboard

Developed a multi-graph dashboard showcasing:

* Loan approval trends
* Customer distribution by state/grade
* Risk profiling insights

Designed for business stakeholders to support **loan decision-making** and **risk analysis**.

---

## 🏁 Final Deliverables

* Complete modular Python ETL package
* Dockerized environment with PostgreSQL
* Spark-based scalable transformation layer
* Airflow DAGs for end-to-end automation
* Lookup table for full data lineage
* Interactive Dash dashboard
* Business-oriented presentation with insights

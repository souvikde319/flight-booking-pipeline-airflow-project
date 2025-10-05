# ✈️ Flight Data Pipeline using Airflow, PySpark & GCP

An end-to-end data engineering project to build a **flight data ETL pipeline** using **Apache Airflow**, **PySpark**, and **Google Cloud Platform (GCP)**.  
It handles **data ingestion**, **transformation**, and **loading** into **BigQuery**, with environment support for **Dev** and **Prod** and a **CI/CD workflow** for automation.

---

## 🚀 Overview

- **Airflow** orchestrates the pipeline.  
- **PySpark** transforms and cleans flight data.  
- **GCS** stores raw and processed data.  
- **BigQuery** holds final analytics-ready data.  
- **CI/CD (GitHub Actions)** automates validation and deployment.  

---

## ⚙️ Workflow

1. **Ingest** `flight_data.csv` → GCS bucket  
2. **Transform** via `spark_transformationjob.py` (PySpark)  
3. **Load** cleaned data → BigQuery  
4. **Orchestrate** all steps with `airflowjob.py` DAG  
5. **Deploy** via GitHub Actions YAML  

---

## 🧩 Key Files

| File | Description |
|------|-------------|
| `dags/airflowjob.py` | Airflow DAG controlling the pipeline |
| `scripts/spark_transformationjob.py` | PySpark transformation logic |
| `data/flight_data.csv` | Sample flight dataset |
| `configs/dev_variables.json` | Dev environment config |
| `configs/prd_variables.json` | Prod environment config |
| `ci-cd/gcp_airflow_pipeline.yml` | CI/CD deployment pipeline |

---

## 🧰 Stack

- **Airflow**, **PySpark**, **BigQuery**, **GCS**
- **Python 3.x**
- **GitHub Actions** (CI/CD)
- **GCP Composer / Local Airflow**

---

## ✅ Features

- Environment-based configuration (Dev & Prod)  
- Automated ETL orchestration via Airflow  
- Scalable PySpark transformations  
- Seamless GCP integration  
- CI/CD for deployment & validation  

---

## 👨‍💻 Author

**Souvik De**  
💼 Data Engineer | Cloud & Pipeline Specialist  
📧 [techsj04@gmail.com](mailto:techsj04@gmail.com)  
🔗 [GitHub](https://github.com/souvikde319)

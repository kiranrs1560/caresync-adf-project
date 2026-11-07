# 🏥 CareSync Health Network - Metadata-Driven Azure Data Lakehouse

An end-to-end Healthcare Data Engineering project built on the Azure ecosystem that demonstrates Metadata-Driven Ingestion, Azure Data Factory Orchestration, Databricks Lakehouse Architecture, Delta Lake, Data Governance, Monitoring, and Analytics.

The platform ingests healthcare data from multiple source systems, processes it through a Bronze-Silver-Gold Medallion Architecture, and delivers curated datasets for reporting, dashboards, and AI-powered analytics.

---

## 📌 Project Overview

Healthcare organizations generate data from multiple operational systems and external partners. Building and maintaining separate pipelines for each source can lead to increased development effort, operational complexity, and maintenance overhead.

This project demonstrates a scalable and reusable approach using:

- Metadata-Driven ETL/ELT Design
- Azure Data Factory (ADF)
- Azure Databricks & PySpark
- Delta Lake
- Unity Catalog
- Azure Key Vault
- Azure Logic Apps
- GitHub CI/CD

The solution enables ingestion, transformation, governance, auditing, and consumption through a centralized architecture.

---

# 🏗️ Architecture Diagram

The platform follows a Metadata-Driven Azure Lakehouse Architecture that combines Azure Data Factory orchestration, Databricks-based transformations, centralized governance, and multiple consumption layers.

<p align="center">
  <img src=".assets/caresync-architecture.png" alt="CareSync Architecture" width="1000"/>
</p>
 
---

## Architecture Components

### Data Sources
- PostgreSQL Operational Database
- Azure Blob Storage Files

### Orchestration Layer
- Azure Data Factory (ADF)
- Azure SQL Database (Metadata & Audit Tables)

### Data Ingestion Layer
- Metadata-Driven Ingestion Framework
- Dynamic Pipeline Execution
- Full & Incremental Loads

### Data Transformation Layer
- Azure Databricks
- Apache Spark (PySpark)
- Delta Lake
- Bronze → Silver → Gold Medallion Architecture

### Governance & Security
- Unity Catalog
- Managed Identities
- Azure Key Vault
- Azure Logic Apps

### Consumption Layer
- Databricks Dashboards
- Databricks Genie Agents
- Databricks Genie One

### DevOps
- GitHub Version Control
- CI/CD Integration

---

# 🚀 Key Features

## Metadata-Driven Ingestion

A centralized metadata table controls:

- Source Object
- Source Type
- Target Table
- Load Type
- Watermark Columns
- Incremental Logic

New data sources can be onboarded through metadata configuration without creating new pipelines.

---

## Medallion Architecture

### Bronze Layer
- Raw source data ingestion
- Historical data retention
- Schema preservation

### Silver Layer
- Data cleansing
- Data quality validation
- Standardization
- Business rule application

### Gold Layer
- Business-ready datasets
- Reporting models
- Analytical consumption layer

---

## ETL / ELT Processing

Implemented reusable PySpark frameworks supporting:

- Full Load
- Incremental Load
- Append Load
- Merge / Upsert Strategies

---

## Governance & Security

Implemented secure access using:

- Unity Catalog
- Azure Key Vault
- Managed Identities
- Role-Based Access Control (RBAC)

No storage keys or passwords are embedded within pipelines.

---

## Monitoring & Auditing

The platform maintains audit information for:

- Pipeline Execution Status
- Start Time
- End Time
- Records Processed
- Error Messages

Operational alerts are automatically triggered using Azure Logic Apps.

---

## CI/CD Integration

Version control is maintained through GitHub repositories for:

- Azure Data Factory Artifacts
- Databricks Notebooks
- SQL Scripts
- Configuration Objects

---

# 🔄 End-to-End Data Flow

```text
PostgreSQL / Blob Storage
            │
            ▼
Azure Data Factory (ADF)
            │
            ▼
Azure Data Lake Storage
            │
            ▼
Bronze Layer (Raw)
            │
            ▼
Silver Layer (Cleansed)
            │
            ▼
Gold Layer (Curated)
            │
            ▼
Databricks Dashboards
Databricks Genie Agents
Databricks Genie One
```

---

# 🛠️ Technology Stack

| Category | Technologies |
|-----------|-------------|
| Cloud Platform | Microsoft Azure |
| Data Ingestion | Azure Data Factory |
| Storage | Azure Data Lake Storage Gen2 |
| Processing | Azure Databricks |
| Programming | Python, PySpark, SQL |
| Data Lake | Delta Lake |
| Governance | Unity Catalog |
| Security | Azure Key Vault, Managed Identities |
| Monitoring | Azure Logic Apps |
| Database | PostgreSQL, Azure SQL Database |
| Version Control | Git, GitHub |

---

# 📂 Repository Structure

```text
caresync-adf-project/
│
├── 01_Sources_Data/
│
├── 02_Metadata_Table_Queries/
│
├── 03_Gold_STTM/
│
├── 04_Azure_Data_Factory_Repository/
│   ├── pipelines/
│   ├── datasets/
│   ├── linkedServices/
│   └── triggers/
│
├── 05_Databricks_Repository/
│   ├── Bronze/
│   ├── Silver/
│   └── Gold/
│
├── assets/
│   └── caresync-architecture.png
│
└── README.md
```

---

# 📈 Business Value

- Reduces development effort through metadata-driven design.
- Accelerates onboarding of new data sources.
- Provides reusable and scalable ETL patterns.
- Improves data quality and governance.
- Enables secure and auditable healthcare analytics.
- Supports business intelligence and AI-driven insights.

---

# 🎯 Skills Demonstrated

### Azure
- Azure Data Factory (ADF)
- Azure Data Lake Storage (ADLS Gen2)
- Azure Databricks
- Azure SQL Database
- Azure Key Vault
- Azure Logic Apps

### Data Engineering
- ETL / ELT Development
- Data Lakehouse Architecture
- Medallion Architecture
- Metadata-Driven Pipelines
- Incremental Data Processing
- Delta Lake

### Databricks
- PySpark
- Delta Lake
- Unity Catalog
- Databricks SQL
- Databricks Dashboards
- Databricks Genie

### DevOps
- Git
- GitHub
- CI/CD

---

# 👨‍💻 Author

**Kiran RS**

📍 Bengaluru, India

- LinkedIn: https://www.linkedin.com/in/rs-kiran17
- GitHub: https://github.com/kiranrs1560

---

⭐ If you found this project helpful, consider starring the repository.

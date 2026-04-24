# azure-data-factory-project

📌 Overview

This project demonstrates an end-to-end data pipeline built using Azure Data Factory (ADF).
It includes data ingestion, transformation, and storage using Mapping Data Flows and Pipelines.

---

🧱 Architecture

The pipeline follows this flow:

1. Source Data (CSV / JSON)
2. Data Flow Transformation
3. Sink (Azure Data Lake Storage Gen2)
4. Orchestration using Pipeline

---

⚙️ Components Used

🔹 Pipeline

- Orchestrates the workflow
- Executes Data Flow activity
- Handles execution and monitoring

🔹 Data Flow

- Performs transformations:
  - Join operations
  - Column selection
  - Data mapping
- Processes structured data

🔹 Datasets

- Source: Delimited files / JSON
- Sink: Processed output files (CSV)

🔹 Linked Services

- Azure Data Lake Storage Gen2 connection
- Used for reading and writing data

---

🔄 Workflow

1. Data is ingested from source files
2. Data Flow performs:
   - Join between datasets
   - Column filtering and selection
3. Transformed data is written to output storage
4. Pipeline triggers and manages execution

---

📁 Repository Structure

├── pipeline/
├── dataflow/
├── dataset/
├── linkedService/
├── factory/
└── publish_config.json

---

🌿 Branch Strategy

- main → Development branch (ADF code)
- adf_publish → Deployment branch (ARM templates)

---

▶️ How to Run

1. Open Azure Data Factory Studio
2. Navigate to the pipeline
3. Click Debug or Trigger
4. Monitor execution in Monitor tab

---

📊 Output

- Processed data is stored in Azure Data Lake Storage
- Output format: CSV
- Contains joined and transformed data

---

🛠️ Technologies Used

- Azure Data Factory
- Azure Data Lake Storage Gen2
- GitHub (Version Control)
- Data Flow (ETL)

---

📌 Key Features

- End-to-end ETL pipeline
- Git integration with ADF
- Data transformation using Data Flows
- Automated deployment using "adf_publish"

---

👨‍💻 Author

Pavan Kumar SV
GitHub: https://github.com/svpavan761-oss

---

⭐ Notes

- Do not modify "adf_publish" branch manually
- Always use Publish in ADF to deploy changes
- Git integration helps in version control and collaboration

---

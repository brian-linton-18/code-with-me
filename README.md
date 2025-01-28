# code-with-me
Code with me through various technologies and projects using the latest and greatest in data engineering

# Databricks

### Questions
- Is there CDC associated with table logs?

### General Notes
- Data stays with cloud provider, Databricks provides control
- Two runtimes, Standard & ML. SQL Warehouse is specialized compute option for SQL
  - Can accelerate SQL Warehouse with Photon
  - Serverless compute is available and managed by DB
    - Faster startup time, less overhead for management
    - Pay what you consume
- Open Data Lake --> Delta Lake --> Unity Catalog (Security, Compliance) --> Databricks IQ (Semantic layer) --> Workflows,
Delta Live Tables, SQL, Dashboards, Genie, Mosaic AI
  - Unity Catalog allows for data, user, and access control 
- DB Marketplace and DB Clean Rooms are built on Delta Sharing
- DB IQ gives auto identification for search, assistant
  - Mosaic AI supports application development
- Orchestration and ETL
  - DB Workflows
    - Orchestrate tasks, including Delta Live Tables
    - Batch and streaming
  - Delta Live Tables
    - Define transforms w. SQL / Python, handles streaming data
- Databricks SQL allows for data warehouse / analytics like tasks
- AI / BI dashboards are available
- AI / BI Genie is available for natural language querying
- DB Workspace is space where your team works
- Unity Catalog
  - Solves manual configuration of workspaces
  - Centralized data lineage, access control
  - Metastore
    - Represents metadata about data / AI assets
    - Access Control Lists
    - Improved security and auditing
    - Metastore --> Catalog --> Schema --> Tables, Views, Models, Functions
    - Multiple metastores across workspace
    - Can assign same Metastore to multiple workspaces
- Notebook must be connected to compute to run

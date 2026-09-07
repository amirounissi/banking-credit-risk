# Banking Credit Risk – Modern Data Stack

End-to-end Credit Risk Analytics Platform built with Medallion Architecture.

## Project Status
- [x] Architecture design
- [ ] Bronze layer
- [ ] Silver layer
- [ ] Gold layer + dbt
- [ ] Power BI Dashboard

## Architecture
flowchart TD
    A[Data Sources<br/>CSV / Credit Applications<br/>Customers / Payments] --> B[Ingestion<br/>Databricks Notebooks<br/>ou Fabric Pipelines]
    
    B --> C[Bronze Layer<br/>Delta Lake - Raw Data<br/>+ Technical Columns]
    
    C --> D[Silver Layer<br/>Cleaned & Standardized<br/>stg_ tables]
    
    D --> E[Gold Layer<br/>Star Schema<br/>Facts + Dimensions<br/>Business KPIs]
    
    E --> F[Power BI / Fabric Semantic Model<br/>Dashboards + Advanced DAX]

## Tech Stack
- **Ingestion & Processing**: Databricks (Delta Lake)
- **Transformation**: dbt
- **Visualization**: Power BI
- **Orchestration**: GitHub Actions

## Project Structure

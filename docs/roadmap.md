# Project Roadmap

Build a reproducible pipeline using yellow taxi records for **May, June, and July 2026**.

## Milestones

### M1. Project Foundations

- **Environment:** establish development tools and dependencies.
- **Infrastructure:** prepare RustFS, Spark, and PostgreSQL.
- **Architecture:** define responsibilities, interfaces, and data flow.

### M2. Data Retrieval — Exercise 1

- **Dataset references:** identify monthly files, dictionaries, and lookup data.
- **Initial collection:** download locally and upload to RustFS.
- **Direct collection:** automate retrieval into RustFS.

### M3. Data Validation and Cleaning — Exercise 2, Branch 1

- **Data contract:** define schemas and data quality rules.
- **Cleaning:** handle missing, duplicate, and invalid records.
- **Publication:** store cleaned historical Parquet files in RustFS.

### M4. Warehouse and SQL Analytics — Exercises 3 and 2, Branch 2

- **Modeling:** define business questions, facts, and dimensions.
- **Database setup:** create tables, constraints, and reference data.
- **Ingestion:** implement the warehouse branch after creating its schema.
- **Analytics:** develop SQL queries for the selected business questions.

### M5. Dashboard — Exercise 4

- **Exploration:** investigate the data using Marimo.
- **Indicators:** select useful metrics and visualizations.
- **Dashboard:** connect to PostgreSQL and provide charts and filters.

### M6. Fare Prediction — Exercise 5

- **Problem definition:** define the price target and usable features.
- **Training:** establish a baseline and compare models using cleaned data.
- **Inference:** provide Python scripts and saved model artifacts.

### M7. Optional Extensions

- **Orchestration:** automate processing with Airflow or Argo Workflows.
- **Prediction interface:** provide an interactive Streamlit demonstration.
- **Governance:** explore metadata management and lineage with DataHub.

### M8. Final Delivery

- **Demonstration:** reproduce the complete workflow across all three months.
- **Report:** present architecture, decisions, results, screenshots, and limitations.
- **Submission:** prepare the required GitHub, source ZIP, and Teams deliverables.

## Transversal Activities

These activities run alongside the milestones rather than forming a final development phase.

### T1. Integration

**Related milestones: M1–M7, consolidated in M8.**

Connect components progressively as their inputs and outputs become available. Verify retrieval-to-cleaning, cleaning-to-warehouse, warehouse-to-dashboard, and cleaned-data-to-prediction flows.

### T2. Testing and Quality

**Related milestones: M1–M7, final acceptance in M8.**

Establish testing tools during foundations. Validate data contracts, processing behavior, SQL results, dashboard figures, and training/inference inputs within the relevant milestones. Evaluate prediction performance against the assignment target.

### T3. Documentation and Reproducibility

**Related milestones: M1–M8.**

Maintain setup instructions, execution commands, code documentation, diagrams, and technical decisions as the project evolves. Collect evidence and screenshots throughout development for the final report.

## Sequencing and Completion

- Complete the warehouse schema before its ingestion branch.
- Dashboard and prediction work can proceed in parallel once their inputs are available.
- A milestone is complete when its relevant transversal activities are also satisfied.
- Prioritize required exercises over optional extensions.
- Dates and collaborator assignments remain unset.

# Automated ETL Pipeline

End-to-end ETL workflows using **Azure Data Factory** and **Databricks**, with ML clustering via Scikit-learn (PCA + K-Means).

## Tech Stack
- **Orchestration**: Azure Data Factory
- **Processing**: Azure Databricks
- **ML**: Scikit-learn (PCA, K-Means), Pandas, NumPy
- **Storage**: Azure Data Lake / Azure SQL Database
- **CI/CD**: GitHub Actions

## Project Structure
```
etl-pipeline/
├── .github/workflows/       # CI/CD pipelines
├── adf/                     # ADF ARM templates & configs
├── databricks/notebooks/    # Databricks notebooks
├── src/
│   ├── etl/                 # Extract, transform, load modules
│   ├── ml/                  # PCA + K-Means clustering
│   └── utils/               # Logging & config helpers
├── sql/                     # DDL, stored procedures, queries
├── tests/                   # Unit & integration tests
├── config/                  # Environment config files
├── scripts/                 # Deploy & bootstrap scripts
└── docs/                    # Architecture & runbooks
```

## Getting Started
```bash
pip install -r requirements.txt
cp config/config.example.yml config/config.dev.yml
python scripts/bootstrap.py
```

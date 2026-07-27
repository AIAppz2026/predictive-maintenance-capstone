# Predictive Maintenance Capstone — Repository Structure

The interim repository follows this structure:

- data/
  - raw/
  - prepared/
- metadata/
- models/
- reports/
  - figures/
- src/
- .gitignore
- PROJECT_STRUCTURE.md
- README.md

## Directory Purpose

- `data/raw/` stores the original registered engine dataset.
- `data/prepared/` stores cleaned training and testing datasets.
- `metadata/` stores dataset metadata, static MLflow experiment exports, evaluation evidence, model metadata, checksums, and reproducibility records.
- `models/` stores the selected reusable model pipeline.
- `reports/figures/` stores charts used in analysis and reporting.
- `src/` stores reusable project scripts.

The local `mlflow_artifacts/` directory is intentionally excluded from GitHub because it contains the persistent MLflow runtime store. Evaluator-readable MLflow evidence is exported under `metadata/`.

Streamlit deployment files and GitHub Actions workflows will be added during the final submission phase.

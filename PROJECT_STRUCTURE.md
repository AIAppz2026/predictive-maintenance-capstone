# Predictive Maintenance Capstone — Repository Structure

The interim repository follows this structure:

- data/
  - raw/
  - prepared/
- metadata/
- mlflow_artifacts/
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
- `metadata/` stores dataset, model, and experiment metadata.
- `mlflow_artifacts/` stores controlled exported MLflow summaries or selected artefacts.
- `models/` stores the selected reusable model pipeline.
- `reports/figures/` stores charts used in analysis and reporting.
- `src/` stores reusable project scripts.

Streamlit deployment files and GitHub Actions workflows will be added during the final submission phase.

# Predictive Maintenance Model Card

## Selected Model

Tuned Bagging classifier packaged as a complete scikit-learn pipeline.

## Intended Use

Risk-sensitive screening and prioritisation of engines for inspection or additional diagnostic review.

The model must not independently authorise maintenance or replace engineering assessment.

## Input Features

- `engine_rpm`
- `lub_oil_pressure`
- `fuel_pressure`
- `coolant_pressure`
- `lub_oil_temperature`
- `coolant_temperature`

## Target

- `0`: documented non-fault / normal class
- `1`: documented faulty / maintenance-attention class

## Held-Out Test Performance

- Accuracy: 0.6583
- Precision: 0.6595
- Recall: 0.9468
- F1-score: 0.7775
- ROC-AUC: 0.7022
- False positives: 1204
- False negatives: 131

## Important Limitation

The model favours class-1 sensitivity and generates a large number of false-positive alerts. Predictions should be treated as inspection recommendations rather than confirmed failures.

## Reproducibility

- Training SHA-256: `f078873ac746b43e5dd2359d46e631283a556c42b2905dc4e3d369338af6c9d6`
- Testing SHA-256: `8f09a48e06d4a11b2efd9deb62fb25516c8b7fc7eab4f5179b1cc63a6d04723f`
- Model SHA-256: `11d427cd355f39a92a2cc4386151e6f0bd21126c2e966b8575cf8587c261a8da`
- Final model signature: `13f55b8bd88870b9fdf5f06b451631716b93ea273f6fa8747c3ce86516dba5ab`
- MLflow run ID: `beed90c71bd245778b995947f12e0b84`

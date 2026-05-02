# anhui_ltcf_dataset

Predicting Unplanned Hospitalization among Long-Term Care Facility (LTCF) Residents in Anhui Province, China.

## Overview

This repository contains baseline machine learning models for predicting 6-month unplanned hospitalization risk among residents in long-term care facilities.

## Dataset

- **Source**: Anhui Province LTCF cohort
- **Target variable**: `unplanned_hospitalization_6mo` (binary)
- **Required files** (not included in this repository):
  - `anhui_ltcf_dataset.xlsx` - Main dataset
  - `anhui_ltcf_routine_codebook.xlsx` - Variable codebook

## Notebook

- `cv5_unplanned_hospitalization_basic_CLEAN.ipynb`: 5-fold cross-validation baseline analysis

### Models Evaluated

| Model | Description |
|-------|-------------|
| Logistic Regression | Linear baseline |
| SVM (RBF) | Support Vector Machine with RBF kernel |
| Decision Tree | Single tree classifier |
| Random Forest | Ensemble of 400 trees |
| GBDT | Gradient Boosting Decision Trees |

### Metrics

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC

All metrics are reported as mean ± standard deviation across 5 stratified folds.

## Usage

1. Place `anhui_ltcf_dataset.xlsx` and `anhui_ltcf_routine_codebook.xlsx` in the same directory as the notebook
2. Run the Jupyter notebook

## Requirements

```
numpy
pandas
scikit-learn
matplotlib
openpyxl
```

## License

Please contact the authors for data access and usage permissions.

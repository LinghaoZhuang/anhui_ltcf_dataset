# anhui_ltcf_dataset

Code for predicting 6-month unplanned hospitalization among LTCF residents in Anhui, China.

## Data

- `anhui_ltcf_dataset.xlsx` - dataset (not included)
- `anhui_ltcf_routine_codebook.xlsx` - codebook (not included)

Target: `unplanned_hospitalization_6mo`

## Analysis

`cv5_unplanned_hospitalization_basic_CLEAN.ipynb` - 5-fold CV with:

- Logistic Regression
- SVM (RBF)
- Decision Tree
- Random Forest
- GBDT

Metrics: Accuracy, Precision, Recall, F1, ROC-AUC

## Requirements

```
numpy
pandas
scikit-learn
matplotlib
openpyxl
```

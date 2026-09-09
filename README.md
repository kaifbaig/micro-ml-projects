# Employee Turnover Prediction

A machine learning project predicting whether an employee is likely to leave the organization using Logistic Regression.

## Workflow

- Loaded and inspected employee data
- Separated features and target
- Performed stratified train-test split
- Trained baseline Logistic Regression
- Compared L1 (Lasso) and L2 (Ridge) regularization
- Evaluated models using accuracy, precision, recall, and F1-score

## Results

| Model | Accuracy |
|---|---:|
| Baseline Logistic Regression | 85.93% |
| L1 (Lasso) | **87.04%** |
| L2 (Ridge) | 85.93% |

L1 regularization achieved the best test accuracy.

## Tools

Python, Pandas, Scikit-learn, Jupyter Notebook
# ShopSmart – Purchase Prediction

A supervised machine learning project that predicts whether an e-commerce visitor is likely to make a purchase based on browsing behaviour and session characteristics.

## Objective

Build a **Decision Tree classification model** to predict the `Revenue` outcome. Since the target is imbalanced, **F1-score** is used as the primary metric, with **0.55** as the benchmark.

## Dataset

The dataset contains **12,330 user sessions** with numerical and categorical features related to visitor and browsing behaviour.

**Target:** `Revenue` — whether the visitor completed a purchase.

## Approach

- Performed data inspection and exploratory data analysis
- Examined class imbalance and behavioural patterns
- Applied an **80/20 stratified train-test split**
- Used `ColumnTransformer` with **One-Hot Encoding** for categorical features
- Built a `Pipeline` combining preprocessing and a **Decision Tree Classifier**
- Evaluated the baseline using accuracy, precision, recall, F1-score, classification report, and confusion matrix
- Used **5-fold GridSearchCV** with F1-score for hyperparameter tuning
- Applied **cost-complexity pruning** using `ccp_alpha`
- Evaluated the final model on the unseen test set

## Model

**Decision Tree Classifier**

Class imbalance was handled using:

```python
class_weight="balanced"
```

Tuned Hyperparameters:

- `max_depth`
- `min_samples_split`
- `min_samples_leaf`
- `ccp_alpha`

## Results

### Baseline

- Accuracy: 85.24%
- Precision: 52.47%
- Recall: 50.00%
- F1-score: 0.5121

### Tuned & Pruned

**Best Parameters:**

```text
max_depth = 3
min_samples_split = 2
min_samples_leaf = 1
ccp_alpha = 0.01
```

**Cross-validation F1:** 0.6667

**Test Performance:**

- Accuracy: 86.90%
- Precision: 55.49%
- Recall: 78.01%
- F1-score: 0.6485

### Improvement

```text
Baseline F1      : 0.5121
Tuned/Pruned F1  : 0.6485
Benchmark        : 0.5500
```

The final model achieved an **absolute F1-score improvement of 0.1364** over the baseline and exceeded the required benchmark.

## Technologies

Python • Pandas • NumPy • Matplotlib • Seaborn • Scikit-learn • Decision Trees • GridSearchCV • One-Hot Encoding • Pipeline • ColumnTransformer
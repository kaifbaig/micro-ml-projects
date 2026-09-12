# Micro ML Projects

A collection of hands-on machine learning projects built to practice **end-to-end machine learning workflows** using Python and Scikit-learn.

The repository covers **classification, regression, exploratory data analysis, feature engineering, preprocessing, regularization, ensemble learning, hyperparameter tuning, cross-validation, and model evaluation**.

---

## Projects

| Project | Type | Best Result | Key Concepts |
|---|---|---:|---|
| **NovaGen Research Labs — Health Risk Classification** | Classification | **94.25% F1** | Random Forest, KNN, AdaBoost, Voting, GridSearchCV |
| **Employee Turnover Prediction** | Classification | **87.04% Accuracy** | Logistic Regression, L1/L2 Regularization |
| **House Price Prediction** | Regression | **0.6195 R²** | Linear Regression, Data Cleaning, EDA, Encoding |
| **ShopSmart — Purchase Prediction** | Classification | **0.6485 F1** | Decision Trees, Imbalanced Data, GridSearchCV, Pruning |

---

## Project Overview

### 1. NovaGen Research Labs — Health Risk Classification

A supervised classification project that predicts whether an individual is **Healthy or Unhealthy** using demographic, physiological, lifestyle, and medical-history indicators.

The project compares multiple classification approaches and uses hyperparameter tuning and ensemble learning to select the final model.

**Models evaluated:**

- Logistic Regression
- KNN
- Random Forest
- AdaBoost
- Soft Voting Classifier

**Final Model:** Random Forest

**Test Results:**

| Metric | Score |
|---|---:|
| Accuracy | 93.87% |
| Precision | 92.38% |
| Recall | 96.18% |
| F1 Score | **94.25%** |

**Key concepts:**

- Exploratory Data Analysis
- StandardScaler
- ColumnTransformer
- Pipeline
- GridSearchCV
- 5-fold Cross-Validation
- Ensemble Learning
- Random Forest
- KNN
- AdaBoost
- Soft Voting

[View Project →](NovaGen/)

---

### 2. Employee Turnover Prediction

A classification project that predicts whether an employee is likely to leave an organization using Logistic Regression.

Different regularization approaches were compared to evaluate their effect on model performance.

**Models evaluated:**

- Baseline Logistic Regression
- L1 (Lasso) Regularization
- L2 (Ridge) Regularization

**Best Model:** L1 (Lasso) Logistic Regression

**Best Test Accuracy:** **87.04%**

**Key concepts:**

- Exploratory Data Analysis
- Logistic Regression
- L1 / L2 Regularization
- Feature Engineering
- Classification Metrics
- Confusion Matrix

[View Project →](employee-turnover/)

---

### 3. House Price Prediction

A regression project that predicts house sale prices using Linear Regression.

The project covers data cleaning, exploratory analysis, categorical encoding, model training, and regression evaluation.

**Model:** Linear Regression

**Test Results:**

| Metric | Score |
|---|---:|
| R² | **0.6195** |
| Adjusted R² | 0.5708 |
| MAE | 34,122.85 |
| RMSE | 54,022.75 |

**Key concepts:**

- Data Cleaning
- Exploratory Data Analysis
- Categorical Encoding
- Linear Regression
- R²
- Adjusted R²
- MAE
- RMSE

[View Project →](house-price-prediction/)

---

### 4. ShopSmart — Purchase Prediction

A classification project that predicts whether an e-commerce visitor is likely to make a purchase based on browsing behaviour and session characteristics.

Because the target is imbalanced, **F1-score** was used as the primary evaluation metric.

**Model:** Decision Tree Classifier

**Key concepts:**

- Exploratory Data Analysis
- Imbalanced Classification
- One-Hot Encoding
- Pipeline
- ColumnTransformer
- Decision Trees
- GridSearchCV
- Cross-Validation
- Cost-Complexity Pruning
- F1-score

**Tuned Test F1-score:** **0.6485**

[View Project →](shop-smart/)

---

## Skills & Tools

### Programming & Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

### Machine Learning

- Classification
- Regression
- Logistic Regression
- Linear Regression
- KNN
- Decision Trees
- Random Forest
- AdaBoost
- Voting Classifier
- Regularization
- Feature Engineering
- Hyperparameter Tuning
- Cross-Validation
- Imbalanced Classification

### Data & Model Workflow

- Data Loading & Inspection
- Data Cleaning
- Exploratory Data Analysis
- Train-Test Splitting
- Feature Preparation
- Categorical Encoding
- Feature Scaling
- Model Training
- Model Evaluation
- Confusion Matrix Analysis
- Model Comparison
- Model Optimization

### Scikit-learn Techniques

- Pipeline
- ColumnTransformer
- StandardScaler
- GridSearchCV
- L1 / L2 Regularization
- Cost-Complexity Pruning
- Ensemble Learning

---

## Repository Structure

```text
micro-ml-projects/
│
├── NovaGen/
│   ├── novagen.ipynb
│   ├── .gitignore
│   ├── README.md
│   └── images/
│       ├── correlation_heatmap.png
│       └── confusion_matrix.png
│
├── employee-turnover/
│   ├── employee_turnover_project.ipynb
│   ├── .gitignore
│   ├── README.md
│   └── images/
│       ├── turnover_distribution.png
│       ├── job_satisfaction_vs_turnover.png
│       ├── correlation_heatmap.png
│       └── confusion_matrix.png
│
├── house-price-prediction/
│   ├── house-price-prediction.ipynb
│   ├── .gitignore
│   ├── README.md
│   └── images/
│       ├── saleprice_distribution.png
│       ├── lotarea_vs_saleprice.png
│       └── correlation_heatmap.png
│
├── shop-smart/
│   ├── shop_smart.ipynb
│   ├── .gitignore
│   ├── README.md
│   └── images/
│       ├── target_distribution.png
│       ├── correlation_heatmap.png
│       └── confusion_matrix.png
│
├── .gitignore
├── requirements.txt
├── LICENSE
└── README.md
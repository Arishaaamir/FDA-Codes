# Fraud Detection Analysis

This repository contains a Python script designed to detect fraudulent insurance claims using machine learning methods.

## Dataset

The dataset `insurance_claims.csv` contains various attributes related to insurance claims.

## Libraries Used

* **Pandas, NumPy**: Data manipulation and analysis.
* **Matplotlib, Seaborn, Plotly**: Data visualization.
* **Scikit-learn**: Data preprocessing, model building, and evaluation.
* **Yellowbrick**: Enhanced visualization for model evaluation.
* **Imbalanced-learn**: Handling imbalanced datasets using SMOTE.

## Preprocessing Steps

1. **Dropped Irrelevant Columns:** Removed identifiers and redundant columns.
2. **Categorical Encoding:** Converted categorical variables using one-hot encoding.
3. **Correlation Analysis:** Visualized numeric feature correlations via heatmap.
4. **SMOTE:** Addressed class imbalance in the dataset.
5. **Feature Scaling:** Standardized numeric features for model training.

## Model

* **Logistic Regression** (balanced class weights to manage class imbalance).

## Model Evaluation

* **Accuracy:** 96.9%
* **Metrics:** Classification report, confusion matrix, ROC curve, and AUC score provided for detailed performance analysis.

## Insights and Recommendations

* The model achieves high accuracy, indicating strong predictive capabilities.
* ROC-AUC and confusion matrix suggest effective classification.
* Precision and recall should be interpreted cautiously due to imbalanced nature.

## Usage

Run the script in an environment where the specified libraries are installed:

```bash
pip install pandas numpy matplotlib seaborn plotly scikit-learn yellowbrick imblearn
```

Execute the script:

```bash
python FDA_assignment_2.py
```

Ensure the `insurance_claims.csv` dataset is in the specified path or adjust accordingly.



# FDA Midterm: Fraud Detection with XGBoost

This repository contains the final submission notebook for the midterm assignment of the Fraud Detection Analysis (FDA) course, utilizing an XGBoost classification model.

## Dataset

The analysis uses two datasets:

* `fda_trainingset.csv`: Training data containing features and the binary target variable (Y).
* `fda_testset.csv`: Test data for final prediction submissions.

## Libraries Used

* **Pandas, NumPy**: Data manipulation and preprocessing.
* **Scikit-learn**: Data preprocessing, train-test splitting, and model evaluation.
* **XGBoost**: Implementing the gradient boosting classification algorithm.

## Preprocessing Steps

1. **Missing Value Imputation:**

   * Median strategy applied to impute missing values.

2. **Feature Engineering:**

   * Created additional features: `feature_sum`, `feature_mean`, `feature_std`, `non_zero_count`, and `max_min_ratio`.

3. **Standardization:**

   * Standardized features for optimal model performance.

## Model

* **XGBoost Classifier** with hyperparameters optimized:

  * Number of estimators: 1000
  * Learning rate: 0.02
  * Max depth: 6
  * Subsample: 0.9
  * Colsample by tree: 0.8
  * Gamma: 0.4
  * Regularization parameters: Alpha=1.0, Lambda=2.0
  * Scale positive weight: 10

## Evaluation

* **Validation AUC-ROC:** 0.951
* **Classification Report:** Demonstrates high accuracy, though the precision and recall metrics indicate class imbalance challenges.

## Submission

* Predictions generated for the test dataset are stored in:

  * `xgb_boosted_final_submission.csv`

## Running the Notebook

Ensure the required libraries are installed:

```bash
pip install pandas numpy scikit-learn xgboost
```

Then, run the notebook:

```bash
jupyter notebook xgb_boosted_final_submission.ipynb
```

## Contribution

Feedback or improvements are welcome. Please submit an issue or pull request.

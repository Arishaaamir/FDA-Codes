# FDA Final Submission: Customer Credit Score Classification

This repository includes the final Jupyter notebook for the Fraud Detection Analysis (FDA) course, focused on classifying customer credit scores using advanced ensemble learning methods.

## Dataset

The analysis uses two datasets:

* `train.csv`: Training data including customer features and credit scores.
* `test.csv`: Test data used for final predictions.

## Libraries Used

* **Pandas, NumPy**: Data handling and manipulation.
* **Matplotlib, Seaborn**: Data visualization.
* **Scikit-learn**: Preprocessing, model training, evaluation.
* **XGBoost, LightGBM, CatBoost**: Ensemble models for prediction.

## Preprocessing Steps

1. **Data Cleaning:**

   * Converted numeric columns from string to numeric type.
   * Cleaned categorical placeholders and irrelevant values.

2. **Feature Engineering:**

   * Transformed `Credit_History_Age` into numerical format (months).

3. **Imputation:**

   * Filled missing numeric values with median.
   * Filled missing categorical values with mode.

4. **Column Reduction:**

   * Dropped irrelevant features like `ID`, `Customer_ID`, `Name`, `SSN`, and `Month`.

5. **Encoding:**

   * Encoded categorical features using Label Encoding.
   * Encoded target variable `Credit_Score`.

6. **Feature Scaling:**

   * Standardized features to improve model performance.

## Model Training

* Trained multiple ensemble models:

  * **RandomForestClassifier**
  * **XGBClassifier**
  * **LGBMClassifier**
  * **CatBoostClassifier**
* Used stacking techniques to enhance predictive accuracy.

## Evaluation

* Employed accuracy, classification reports, confusion matrices, and ROC-AUC scores for model evaluation.

## Submission

* Generated final predictions on the test dataset.

## Running the Notebook

Install required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost lightgbm catboost
```

Run the notebook:

```bash
jupyter notebook Untitled4.ipynb
```

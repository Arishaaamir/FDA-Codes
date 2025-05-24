# Customer Segmentation Analysis for HSBC

This repository contains a Jupyter Notebook designed for customer segmentation using KMeans clustering, applied to HSBC's customer dataset.

## Dataset

The notebook uses a dataset featuring customer profiles, including financial and demographic variables.

## Libraries Used

* **Pandas, NumPy**: Data handling and preprocessing.
* **Matplotlib, Seaborn, Plotly**: Visualizing data distributions and clusters.
* **Scikit-learn**: Implementing KMeans clustering and evaluating clusters using Silhouette Score.

## Analysis Steps

1. **Data Preprocessing:**

   * Scaling numeric features using StandardScaler.
   * Preparing data for cluster analysis.

2. **Cluster Analysis:**

   * Applied KMeans clustering algorithm.
   * Evaluated cluster quality using the Silhouette Score.
   * Compared results for varying cluster counts (k=2, 4, 6, 8).

3. **Optimal Cluster Identification:**

   * Optimal cluster count determined by highest silhouette score (k=6).

## Results

* **Optimal number of clusters:** 6 clusters provided the best balance according to the Silhouette Score (0.28).

### Real-World Implications for HSBC:

* **Cluster 1:** High TRB & Income → Priority customers → Recommend premium investment products.
* **Cluster 2:** Young, digitally active → Promote digital wallet, FX services.
* **Cluster 3:** Loan-heavy profile → Offer consolidation plans or MPF promotions.

## Usage

Install necessary libraries:

```bash
pip install pandas numpy matplotlib seaborn plotly scikit-learn
```

Run the notebook in a Jupyter environment:

```bash
jupyter notebook FDA_Assignment_3_Arisha.ipynb
```

## Contributions

Feedback and contributions are encouraged. Please create an issue or submit a pull request.

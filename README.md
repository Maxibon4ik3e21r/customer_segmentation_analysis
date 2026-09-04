# Customer Segmentation & Spending Score Analysis
 
Analysis of 200 mall customers using K-Means clustering and linear regression.
 
## Data
`Mall_Customers.csv` — Age, Gender, Annual Income (k$), Spending Score (1-100).
 
## What I did
1. **Clustering (K-Means)** — grouped customers into 5 segments based on income and spending score. Picked k=5 using the elbow method and silhouette score (0.555).
2. **Regression**  tried to predict Spending Score from Age and Income, with full diagnostics (R², p-values, VIF, residuals).
## Results
 
**5 customer segments:**
| Cluster | Profile |
|---|---|
| 0 | Mid income, average spenders |
| 1 | High income, high spenders >>> target segment |
| 2 | Low income, high spenders |
| 3 | High income, low spenders |
| 4 | Low income, low spenders |
 
**Regression:** weak fit (R² ≈ 0.11). Age was a significant predictor, Income was not — meaning the relationship isn't linear. This is why clustering worked better than regression for this data.
 
## Files
- `customer_segmentation_analysis.ipynb` — full notebook with code, plots, and output
- `cluster_summary.csv`


Python, pandas, scikit-learn, statsmodels, matplotlib/seaborn
 

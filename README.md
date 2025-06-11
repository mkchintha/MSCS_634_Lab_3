# MSCS_634_Lab_3

# Lab Assignment 3: K-Means and K-Medoids Clustering on Wine Dataset

*Author*: Murali Krishna Chintha  
*Course*: MSCS-634-M40 – Advanced Big Data and Data Mining Lab
---

## Purpose

The goal of this lab is to explore unsupervised learning techniques - specifically *K-Means* and *K-Medoids* clustering—on the Wine dataset. The lab aims to evaluate clustering quality using Silhouette Score and Adjusted Rand Index (ARI), and to compare both clustering methods visually and analytically.

---

## Key Insights

•⁠  ⁠*K-Means*:
  - Performs well when data is evenly distributed and features are scaled.
  - Achieved good *Silhouette Score* and *ARI*, indicating well-separated and label-aligned clusters.
  - Uses centroids which may not represent actual data points.

•⁠  ⁠*K-Medoids*:
  - More robust to outliers since it uses actual data points (medoids) as centers.
  - Slightly lower Silhouette Score than K-Means, but more interpretable clusters.
  - Performs better when data may contain noise or irregular shapes.

•⁠  ⁠*Visual Comparison*:
  - K-Means clusters appeared more symmetric and tighter.
  - K-Medoids clusters were more natural and aligned with actual samples, but with some overlap.

---

## Challenges & Decisions

•⁠  ⁠Faced a binary incompatibility issue between NumPy and ⁠ scikit-learn-extra ⁠ in Colab.
  - Resolved by downgrading NumPy to a stable version (⁠ 1.24.4 ⁠) before reinstalling ⁠ scikit-learn-extra ⁠.
•⁠  ⁠Chose ⁠ k=3 ⁠ based on domain knowledge (Wine dataset has 3 actual classes).
•⁠  ⁠PCA was used to visualize high-dimensional clustering in 2D for better interpretability.

---

## Conclusion

•⁠  ⁠Use *K-Means* for fast, efficient clustering on clean, scaled data.
•⁠  ⁠Use *K-Medoids* when interpretability and robustness to outliers are important.

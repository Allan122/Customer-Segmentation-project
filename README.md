# Customer Segmentation using RFM and K-Means Clustering 🛍️

**Source Dataset:** [Kaggle: Online Retail Dataset](https://www.kaggle.com/datasets/vijayuv/onlineretail)

## Project Overview
This project applies **unsupervised machine learning** to a transactional dataset to identify and profile distinct customer groups based on their purchasing behavior. The goal is to provide **actionable intelligence** for marketing, retention and sales strategies.

## Skills and Tools
* **Machine Learning:** K-Means Clustering, Unsupervised Learning
* **Feature Engineering:** RFM (Recency, Frequency, Monetary) Modeling
* **Data Analysis:** Python (Pandas, NumPy, Scikit-learn)
* **Statistics:** Log Transformation, Standard Scaling, Elbow Method
* **Visualization:** Matplotlib
* **Business Acumen:** Customer Profiling and Strategy Development

## Methodology
The project followed a strategic, data-driven approach:

1.  **Data Preparation:** Cleaned raw data and created the core **RFM features** (Recency, Frequency, Monetary Value) for each of the 4,339 unique customers.
2.  **Statistical Transformation:** Applied **Log Transformation** and **Standard Scaling** to the RFM features to successfully mitigate the severe positive skewness caused by high-value outliers. This ensured the K-Means algorithm provided reliable results.
3.  **Model Selection:** Used the **Elbow Method** to determine the optimal number of segments ($K=5$).
4.  **Clustering & Profiling:** Ran the final **K-Means model** and analyzed the mean RFM values of the resulting clusters to assign clear, business-focused names.

## Key Deliverables and Segments

The analysis successfully segmented the customer base into 5 distinct, high-value groups:

| Segment | Customer Count | Recency (Days) | Monetary (Value) | **Actionable Strategy** |
| :--- | :--- | :--- | :--- | :--- |
| **🏆 Champions** | 426 | **6.85** (Lowest) | **$11,327** (Highest) | Reward and prioritize retention to maximize lifetime value. |
| **💎 Loyal & High-Value** | 993 | 31.59 | $2,382$ | Encourage upgrade to 'Champions' status with premium offers. |
| **🌟 Potentials** | 958 | 119.85 | $1,097$ | Focus on re-engagement and cross-selling to improve purchase frequency. |
| **🌱 Newbies** | 729 | 19.63 | $448$ | Provide immediate guidance and incentives to encourage a second, larger purchase. |
| **🥀 At Risk/Losing** | 1233 | **193.04** (Highest) | $257$ (Lowest) | Launch aggressive win-back campaigns and personalized discounts. |

### Elbow Plot for Optimal K Selection
<img width="1035" height="649" alt="image" src="https://github.com/user-attachments/assets/7931fd64-5f9a-4c0e-bfaa-219b6f962ac5" />




---

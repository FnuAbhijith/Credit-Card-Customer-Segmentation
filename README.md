# Credit-Card-Customer-Segmentation

![Credit-Card-Customer-Segmentation](https://github.com/user-attachments/assets/1dbcb4f0-3dca-43bb-9f88-d54cf23827b5)


🔹 Problem Statement

Banks and financial institutions often need to group customers into meaningful segments for marketing, risk analysis, and product recommendations. Traditional demographic segmentation is not enough — here we cluster customers based on their behavioral attributes (e.g., spending, usage, credit limit).

Goal: Identify distinct groups of credit card users and generate insights to guide business strategy.

🔹 Dataset

- Source: BankChurners Kaggle Dataset

- Rows: 10,127 customers

- Features: Credit limit, balance, transaction counts, utilization ratio, tenure, etc.

- Target: Unsupervised (no labels; goal is clustering)

🔹 Approach

1. Data Cleaning

 - Removed unnecessary ID columns

 - Handled missing values

 - Encoded categorical features (gender, education, marital status)

2. Feature Scaling

 - StandardScaler to normalize skewed values

3. Dimensionality Reduction

 - PCA reduced dimensionality to 2D for visualization

 - Explained ~85% variance with top components

4. Clustering

 - KMeans clustering

 - Chose optimal k using Elbow Method and Silhouette Score

 - Final choice: k = 4

🔹 Results

- Identified 4 distinct customer segments:

  1. High spenders – high credit limit, high balance, frequent transactions

  2. Low spenders – low balance, low utilization, few transactions

  3. Revolvers – carry balance, high utilization, low payments

  4. New/Low tenure customers – short relationship with bank, low credit usage

- Visualization (PCA clusters):


🔹 Business Insights

📈 Upsell opportunities → Offer premium rewards to high spenders

⚠️ Risk monitoring → Closely track revolvers with high utilization

🎯 Retention campaigns → Target new/low tenure customers with onboarding offers

🔹 Metrics

- Silhouette Score: 0.42 (moderate cluster separation)

- Inertia: 2,870 (used for elbow method)

🔹 Tech Stack

- Python: pandas, numpy, scikit-learn, matplotlib, seaborn

- Clustering: KMeans, PCA

- Visualization: 2D scatter plots, bar charts

This project segments credit card customers into behavioral groups using unsupervised learning models like KMeans Clustering and PCA for dimensionality reduction and visualization.


## 📊 Results Summary

| Step                  | Method/Tool Used       | Outcome/Details                           |
|-----------------------|------------------------|--------------------------------------------|
| Clustering Algorithm  | KMeans                 | Segmented customers into 4 clusters        |
| Cluster Validation    | Silhouette Score       | Best score at **k = 4**                    |
| Dimensionality Reduction | PCA (2 Components) | Used for visualization                     |
| Preprocessing         | One-Hot Encoding + Scaling | Ensured data was model-ready           |
| Output                | Segmented_Customers.csv | Final dataset with `Cluster` labels      |


## 📈 Visual Outputs

- 📊 **Silhouette Score Plot** – Used to determine the optimal number of clusters  
- 📉 **PCA Scatter Plot** – Visualizes customer distribution across clusters  
- 🧾 **Segmented_Customers.csv** – Final dataset with an added `Cluster` column  
- 📌 **Cluster Count Summary** – Number of customers in each cluster

🚀 How to Run
git clone https://github.com/FnuAbhijith/CreditCard-Customer-Segmentation.git
cd CreditCard-Customer-Segmentation
pip install -r requirements.txt
jupyter notebook Customer_Segmentation.ipynb

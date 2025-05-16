# Credit-Card-Customer-Segmentation

This project segments credit card customers into behavioral groups using unsupervised learning models like KMeans Clustering and PCA for dimensionality reduction and visualization.

![Uploading Credit-Card-Customer-Segmentation.jpg…]()


🎯 Goal

To group credit card customers based on usage patterns and profile characteristics to help businesses personalize services, reduce churn, and improve customer targeting.

🧠 Key Features

Model Used:

KMeans Clustering

Optimal cluster selection using Silhouette Score

Visualization using PCA (Principal Component Analysis)

Exported segmented customer data for business use

📂 Dataset
Source: Kaggle (Bank Customer Dataset)

Includes demographic info, transaction patterns, and card activity metrics

Kaggle Dataset = https://www.kaggle.com/datasets/thedevastator/predicting-credit-card-customer-attrition-with-m/data (BankChurners.csv)

🛠️ Tools & Libraries
Python (Pandas, NumPy, Scikit-learn)

KMeans, PCA, StandardScaler

Matplotlib, Seaborn

Jupyter Notebook

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
bash

git clone https://github.com/YOURUSERNAME/credit-card-customer-segmentation.git
cd credit-card-customer-segmentation
pip install -r requirements.txt
jupyter notebook

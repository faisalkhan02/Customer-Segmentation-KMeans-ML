# Customer Segmentation using K-Means Clustering

Unsupervised Machine Learning project for Minor Project 2 (ML Internship) — segmenting mall customers 
into distinct groups based on Annual Income and Spending Score using K-Means Clustering.

## 📌 Problem Statement

Retail businesses often struggle to understand customer purchasing behavior because customer 
data is usually unlabeled. This project segments mall customers into distinct groups based on 
their Annual Income and Spending Score using K-Means Clustering, enabling targeted marketing 
strategies.

## 📊 Dataset

- **Source:** [Mall Customer Segmentation Dataset (Kaggle)](https://www.kaggle.com/datasets/hosseinbadrnezhad/mall-customer-segmentation-dataset)
- **Records:** 1000 customers
- **Features:** CustomerID, Gender, Age, Annual Income (k$), Spending Score (1-100)

## 🛠️ Tech Stack

- Python
- Pandas, NumPy
- Matplotlib, Seaborn (visualization)
- Scikit-learn (StandardScaler, KMeans, Silhouette Score, Davies-Bouldin Index)

## 🔍 Approach

1. **Data Preprocessing** — handled missing values (median/mode imputation), checked duplicates, scaled features
2. **Exploratory Data Analysis** — distribution plots, correlation heatmap, pairplot, boxplots
3. **Model Selection** — K-Means Clustering, chosen for its efficiency on numeric continuous data
4. **Finding Optimal K** — Elbow Method + Silhouette Score analysis → K = 3
5. **Model Evaluation** — Silhouette Score: 0.474, Davies-Bouldin Index: 0.720
6. **Cluster Interpretation** — profiled each cluster into a business-relevant customer segment

## 📈 Results — Customer Segments

| Cluster | Profile | Avg. Age | Avg. Income (k$) | Avg. Spending Score |
|---|---|---|---|---|
| 0 | Young, Moderate Income, High Spenders | 30.1 | 35.3 | 57.0 |
| 1 | Older, High Income, Low Spenders | 61.1 | 102.5 | 9.3 |
| 2 | Middle-Aged, Moderate-High Income, Average Spenders | 40.8 | 68.1 | 37.7 |

## 📁 Repository Structure
```
Customer-Segmentation-KMeans-ML/
│
├── Customer_Segmentation_Minor_Project_2.ipynb
│
├── Mall_Customers.csv   
│
├── Minor_Project_2_Report.pdf
|
└── README.md

```

## 🚀 How to Run

```bash
git clone https://github.com/faisalkhan02/Customer-Segmentation-KMeans-ML.git
cd Customer-Segmentation-KMeans-ML
pip install pandas numpy matplotlib seaborn scikit-learn
jupyter notebook notebook/Customer_Segmentation_Minor_Project_2.ipynb
```

## 👤 Author

**Faisal Khan**

Master of Computer Applications (MCA)

KIET Group of Institutions, Ghaziabad

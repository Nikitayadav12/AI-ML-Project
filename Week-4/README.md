🧾 Project Title

Customer Segmentation using Unsupervised Learning

📌 Objective

The goal of this project is to segment customers of an Online Retail store into meaningful groups using unsupervised machine learning techniques.
This helps businesses design targeted marketing strategies, improve customer retention, and increase sales revenue.

📊 Dataset

Source: Online Retail Dataset (UCI Repository / Kaggle)

Content: Transactions from a UK-based online retailer (2010–2011)

Features include:

InvoiceNo, StockCode, Description, Quantity, InvoiceDate, UnitPrice, CustomerID, Country

⚙️ Workflow

Data Loading & Cleaning

Removed missing CustomerID values

Removed negative/zero quantity and price

Created new feature: Revenue = Quantity × UnitPrice

Feature Engineering (RFM Analysis)

Recency → Days since last purchase

Frequency → Number of transactions

Monetary → Total spend

Preprocessing

Outlier treatment (Winsorization)

Log transformation

Standardization (z-scaling)

Clustering (Unsupervised Learning)

K-Means clustering

Cluster selection using Elbow method & Silhouette score

Final choice: k = 3 clusters (business-driven)

Dimensionality Reduction & Visualization

PCA (2D projection of clusters)

Scatter plots of clusters

Cluster Profiling & Interpretation

Cluster 0 → VIP Customers (High Frequency, High Spend)

Cluster 1 → Lost Customers (Old, Rare, Low Spend)

Cluster 2 → New Customers (Recent, Moderate Spend)

Added bar chart of cluster sizes

Bonus: Hierarchical Clustering (Dendrogram)

📈 Results & Business Insights

VIP Customers → Should be rewarded with loyalty programs & premium offers.

Lost Customers → Can be targeted with reactivation campaigns (“We miss you” offers).

New Customers → Encourage repeat purchases with welcome bundles & discounts.

📌 These insights show how unsupervised learning can support real business strategy.

🛠️ Tech Stack

Language: Python

Libraries: Pandas, NumPy, Matplotlib, scikit-learn, SciPy

Environment: Jupyter Notebook

📷 Sample Outputs

Elbow Plot

Silhouette Score Plot

PCA Cluster Visualization

Dendrogram (Hierarchical Clustering)

Cluster Profiling Table & Bar Chart

🚀 How to Run

Clone this repository

git clone https://github.com/yourusername/customer-segmentation.git
cd customer-segmentation


Install dependencies

pip install -r requirements.txt


Run the notebook

jupyter notebook "Week 4 Project GCT.ipynb"

✅ Conclusion

This project demonstrates the complete process of Customer Segmentation using unsupervised learning techniques, from data cleaning to business interpretation. It is an end-to-end trainer-ready project and can be extended with advanced clustering algorithms (DBSCAN, Gaussian Mixture Models) for future work.

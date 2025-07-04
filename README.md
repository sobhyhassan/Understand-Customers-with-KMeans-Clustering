# 🧠 Customer Segmentation with KMeans Clustering

This project aims to segment customers based on their behavior using unsupervised learning (KMeans Clustering).  
The goal is to uncover hidden patterns in customer data and group them into actionable clusters to support business decision-making.

---

## 📊 Project Workflow

1. **Exploratory Data Analysis (EDA)**  
   Understand distributions, correlations, and customer behavior patterns.

2. **Data Cleaning & Preprocessing**  
   - Handle missing values  
   - Scale numerical features  
   - Convert categorical values  
   - Filter out invalid or noisy entries

3. **Feature Engineering**  
   Based on RFM Model:
   - `Recency` – Time since last purchase  
   - `Frequency` – How often the customer buys  
   - `Monetary` – Total amount spent

4. **Outlier Detection**  
   Identify and handle outliers using statistical thresholds and isolate them for separate analysis.

5. **Clustering with KMeans**  
   Apply KMeans clustering on engineered features to group customers into behavior-based segments.

6. **Cluster Analysis & Naming**  
   Each cluster is analyzed and given a business-aware label and action strategy.

---

## 🏷️ Cluster Labels & Strategies

| Cluster | Label                | Description                                      |
|--------|----------------------|--------------------------------------------------|
| 0      | Inactive / Churned   | Low value, old activity                         |
| 1      | Re-engage / Growing  | Medium value, recent activity                   |
| 2      | Loyal / VIP          | High value and very active                      |
| 3      | Occasional           | Low spenders, not fully inactive                |
| -1     | PAMPER               | Outliers with very high spending                |
| -2     | UPSELL               | Frequent but low spenders                       |
| -3     | DELIGHT              | High-frequency + high-spending outliers (VIPs)  |

---

## 📈 Visualizations

- Violin plots for Recency, Frequency, and Monetary across clusters  
- Bar charts showing cluster distributions  
- Line plots for average values per cluster  
- Outlier segmentation charts

---

## 🧰 Technologies Used

- Python 3  
- Pandas, NumPy  
- Seaborn, Matplotlib  
- Scikit-learn  
- Jupyter Notebook

---

## ▶️ How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/customer-segmentation-kmeans.git
   cd customer-segmentation-kmeans

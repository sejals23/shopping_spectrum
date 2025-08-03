# 🛍️ Customer Segmentation using RFM and K-Means Clustering

## 📌 Project Overview
This project aims to segment customers of an online retail dataset using **RFM Analysis (Recency, Frequency, Monetary)** and unsupervised machine learning techniques such as **K-Means Clustering**. The segmentation helps businesses understand their customer base and design targeted marketing campaigns to improve engagement and revenue.

---

## 📂 Dataset Information
- The dataset contains transactions from an **online retail store** for one year.
- Key columns:
  - **InvoiceNo**: Invoice number of the transaction
  - **StockCode**: Product code
  - **Description**: Product description
  - **Quantity**: Number of items purchased
  - **InvoiceDate**: Date of purchase
  - **UnitPrice**: Price per unit
  - **CustomerID**: Unique customer identifier
  - **Country**: Country of the customer

---

## 🛠️ Steps Performed

### 1. **Data Cleaning**
- Removed duplicates and null values.
- Treated negative values in `Quantity` and `UnitPrice`.
- Filtered out cancelled transactions.

### 2. **Exploratory Data Analysis (EDA)**
- Analyzed transaction distribution by country.
- Identified top-selling products and purchase trends over time.
- Outlier detection using **boxplots** for `Quantity` and `UnitPrice`.

### 3. **RFM Analysis**
- **Recency**: Days since last purchase.
- **Frequency**: Number of transactions.
- **Monetary**: Total amount spent.
- Calculated and created an **RFM table** for all customers.

### 4. **Data Scaling**
- Applied **StandardScaler** to RFM values to standardize the features before clustering.

### 5. **Clustering**
- Used **Elbow Method** and **Silhouette Score** to determine optimal number of clusters.
- Applied **K-Means Clustering** and assigned each customer to a cluster.

### 6. **Visualization**
- Scatterplots for clusters based on Recency, Frequency, and Monetary values.
- Best-selling products bar chart.
- Heatmaps for product recommendations using **Customer-Product Matrix** and **Cosine Similarity**.

---

## 📊 Key Insights
- The majority of transactions came from the **United Kingdom**.
- The top-selling product was **World War 2 Gliders ASSTD Designs**.
- Purchase frequency increased steadily during the last quarter of the year.
- Clear segmentation of customers into groups such as high-value, loyal, and at-risk customers.

---

## 🚀 Business Impact
- Businesses can use the clusters to run **personalized marketing campaigns**.
- Helps to **retain high-value customers** and re-engage inactive customers.
- Identifies products to cross-sell based on customer similarity.

---


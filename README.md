# Shopping-trends-and-customer-behavior-cluster
#  Customer Segmentation with K-Means

This project analyzes a **synthetic dataset of 3,900 customer purchases** to uncover shopping behavior and segment customers into meaningful groups using **unsupervised machine learning (K-Means clustering)**.

### Project Highlights
- Identified **spending patterns**, **demographic trends**, and **actionable marketing insights**.
- Created **4 unique customer segments** to support targeted marketing strategies.
- Delivered **interactive visualizations** and **data-driven recommendations**.

---

## Dataset Overview

**Features:**
- **Demographics:** Age, Gender, Location  
- **Purchase Details:** Item, Category, Amount (USD), Size, Color  
- **Context:** Season, Review Rating (1–5), Subscription Status, Payment Method  

**Key Stats:**
- No missing values  
- Gender-balanced dataset (52% Female / 48% Male)  
- Average purchase amount: **$59.47**

---

##  Exploratory Data Analysis (EDA)

**Key Insights:**
- **Top Categories:** Clothing (50%) > Footwear > Electronics  
- **Seasonal Trends:** Peak spending in **Winter** (holiday-driven)  
- **Payment Preferences:** Credit Card (35%) > PayPal (30%) > Debit Card (25%)  
- **Review Ratings:** 80% are **4 stars and above** (positive bias)

**Sample Visuals:**

| Chart | Insight |
|-------|---------|
| Category Spend | Clothing dominates total sales |
| Age Histogram | Most shoppers are aged **30–50** |
| Payment methods| Credit cards are the most used |

---

##  Customer Segmentation (K-Means)

**Clustering Approach:**
- Optimal Clusters: **K = 4** (chosen via Elbow Method)
- Scaled data + PCA for dimensionality reduction

**Cluster Profiles:**

| Cluster | Description |
|---------|-------------|
| 0 | **Budget Shoppers** – Low spend, discount-focused |
| 1 | **Luxury Buyers** – High spend on Clothing & Electronics |
| 2 | **Subscription Loyalists** – Steady, mid-level purchases |
| 3 | **Occasional Shoppers** – Sporadic spending across categories |

**Validation Metrics:**
-  **Silhouette Score:** 0.52 (moderate clustering performance)  
-  PCA reveals **partial overlap**, suggesting some behavioral similarities

---

##  Recommendations

**Marketing Strategies:**
- Bundle premium products for **Luxury Buyers (Cluster 1)**
- Offer referral bonuses for **Subscription Loyalists (Cluster 2)**

**Data Improvements:**
- Add fields like **Purchase Frequency** or **Customer Lifetime Value**

**Further Experimentation:**
- **DBSCAN** for anomaly detection  
- **Hierarchical Clustering** for better interpretability

---

##  Tech Stack

- **Python Libraries:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `plotly`
- **Machine Learning:** `scikit-learn` (K-Means, PCA, StandardScaler)
- **Visualization:** Static plots + interactive visualizations via Plotly and PCA Biplots

---

>  *This project showcases end-to-end clustering—from EDA to insights—using real-world business logic on synthetic data. Ideal for marketing analytics, customer profiling, and segmentation models.*

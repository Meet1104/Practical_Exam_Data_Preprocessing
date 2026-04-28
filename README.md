# 📊 Customer Purchase Propensity - Data Cleaning & Feature Engineering Pipeline

## 📌 Project Overview
This project focuses on building a complete data preprocessing and feature engineering pipeline for an e-commerce dataset.

The goal is to prepare raw data from multiple sources for a future Machine Learning model that predicts whether a customer will make a purchase (binary classification).

---

## 🎯 Objectives
- Implement a full data preprocessing workflow
- Handle real-world messy data
- Apply feature engineering techniques
- Prepare data for machine learning

---

## 🧠 Problem Framing
- Type: Binary Classification  
- Target Variable: `purchased (0 or 1)`  
- Goal: Predict customer purchase behavior  

---

## 📂 Data Sources
- `customers.csv` → Customer demographics  
- `transactions.json` → Transaction records  
- `products.sql` → Product information  
- API → https://dummyjson.com/users  

---

## ⚙️ Workflow

### 1. Data Import & Merging
- Load CSV, JSON, SQL, API data  
- Merge using `customer_id` and `product_id`

### 2. Exploratory Data Analysis (EDA)
- Univariate: Histograms, skewness  
- Bivariate: Income vs Purchase  
- Multivariate: Heatmaps, pairplots  

### 3. Handling Missing Data
- Simple Imputer  
- Most Frequent  
- Missing Indicator + Random Sampling  
- KNN Imputer  
- MICE  
- Complete Case Analysis  

### 4. Outlier Detection
- Z-score  
- IQR  
- Percentile  
- Winsorization  

### 5. Date & Feature Engineering
- Convert dates  
- Create `days_since_last_purchase`  

### 6. Encoding
- Label Encoding  
- One-Hot Encoding  
- Ordinal Encoding  

### 7. Feature Scaling
- StandardScaler  
- MinMaxScaler  
- MaxAbsScaler  
- RobustScaler  
- Normalizer  

### 8. Feature Construction
- `purchase_per_day`  
- Log / sqrt / power transforms  
- Binning (income groups)  
- Binarization (`frequent_buyer`)

---

## 📊 Output
- Final cleaned dataset: `processed_customer_data.csv`

---

## 🚀 Tech Stack
- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Matplotlib / Seaborn  
- SQLite  

---

## 📌 Challenges
- Missing values  
- Data merging  
- Outliers  
- Feature scaling decisions  

---

## ✅ Conclusion
This project builds a complete preprocessing pipeline to transform raw data into a machine learning-ready dataset.

---

## 📎 Deliverables
- DataPreprocessing.ipynb  
- processed_customer_data.csv  
- feature_pipeline.py  
- README.md  

---

## 👨‍💻 Author
Meet Golakiya

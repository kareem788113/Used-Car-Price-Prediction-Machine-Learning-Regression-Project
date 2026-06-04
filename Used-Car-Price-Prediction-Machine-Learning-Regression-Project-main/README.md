# 🚗 Used Car Price Prediction – Machine Learning Regression Project

## 📌 Project Overview
This project focuses on building a **data-driven system to predict used car prices** using machine learning regression techniques.  
With the rapid growth of the used car market and the absence of standardized pricing, this project aims to provide **objective, fair, and accurate price estimation** based on real vehicle attributes.

The workflow covers the **entire data science pipeline**:
- Data cleaning & preprocessing  
- Exploratory Data Analysis (EDA)  
- Feature engineering  
- Model training & evaluation  
- Performance comparison  

---

## 🎯 Objectives
- Analyze the key factors affecting used car prices
- Handle real-world data issues such as missing values, noisy text fields, and outliers
- Compare regression models to identify the best-performing approach
- Build an interpretable and scalable regression pipeline

---

## 📂 Dataset Description
The dataset is sourced from **Kaggle** and represents used car listings across different cities in India.

### 🔑 Features
| Feature | Description |
|------|------------|
| Name | Full car name and variant |
| Cars | Extracted car brand + model |
| Location | City of sale |
| Year | Manufacturing year |
| Kilometers_Driven | Total kilometers driven |
| Fuel_Type | Petrol, Diesel, CNG, etc. |
| Transmission | Manual / Automatic |
| Owner_Type | Ownership history |
| Mileage | Fuel efficiency |
| Engine | Engine capacity (CC) |
| Power | Engine power (bhp) |
| Seats | Seating capacity |
| Price | Target variable (in Lakhs) |

---

## 🛠️ Technologies & Libraries
- **Python**
- **Pandas, NumPy**
- **Matplotlib, Seaborn, Plotly**
- **Scikit-learn**
- **XGBoost, CatBoost**
- **Google Colab**

---

## 🧹 Data Preprocessing
Key preprocessing steps include:
- Dropping irrelevant columns (`New_Price`, `Unnamed: 0`)
- Handling missing values using **median imputation**
- Cleaning text-based numerical features (`Mileage`, `Engine`, `Power`)
- Feature engineering:
  - Creating a new `Cars` feature to normalize vehicle naming
- Outlier removal using **IQR and percentile-based filtering**
- Encoding categorical features using **Label Encoding**
- Feature scaling using **StandardScaler**

---

## 📊 Exploratory Data Analysis (EDA)
EDA was conducted to understand data distribution and relationships:
- Price distribution & skewness analysis
- Count plots for categorical variables
- Boxplots & histograms for numerical features
- Correlation heatmap
- Interactive visualizations using **Plotly**

### 🔍 Key Insights
- Diesel cars dominate the dataset
- Newer cars and automatic transmission vehicles tend to be more expensive
- Engine power and manufacturing year show strong correlation with price

---

## 🤖 Machine Learning Models
Two supervised regression models were implemented:

### 1️⃣ Linear Regression
- Serves as a baseline model
- Simple and interpretable
- Assumes linear relationships between features and price

### 2️⃣ Decision Tree Regressor
- Captures non-linear relationships
- Handles feature interactions effectively
- Configured with max depth to reduce overfitting

---

## 📈 Model Evaluation Metrics
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score (Train & Test)

### 🏆 Results Summary
| Model | RMSE | Train R² | Test R² |
|-----|------|---------|--------|
| Linear Regression | Baseline | Moderate | Moderate |
| Decision Tree Regressor | Lower | High | Improved |

➡️ **Decision Tree Regression outperformed Linear Regression** by better modeling complex relationships.

---

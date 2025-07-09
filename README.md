# 📊 Customer Churn Prediction – Internship Project at Utkarsh Enterprises

Welcome to the repository for a **real-world churn prediction project**, completed as part of my internship at **Utkarsh Enterprises**, a B2B company that specializes in custom-printed T-shirts.

This end-to-end data science project focuses on identifying potential customer churn from the CRM system using Python, EDA, and machine learning.

## 🚀 Project Objective

> To predict whether a lead will **churn** (not place an order) or **convert** (place an order), using lead engagement behavior, sales data, and CRM metadata.

## 🧠 Problem Statement

In B2B sales, many leads drop out before placing orders due to delays, lack of follow-up, or disinterest. This model simulates churn by identifying which leads didn’t reach the final “Order” stage and trains a classifier to detect similar patterns in new leads.

## 📁 Project Structure
customer-churn-prediction/

├── data/
│   └── CRM Data.xlsx         # Dataset with Lead and Order info

├── churn.ipynb                     # Jupyter Notebook with full model pipeline

├── README.md                       # Project overview and guide

├── requirements.txt                # Python dependencies


## 🧾 Dataset Description

- **Source**: CRM dashboard used during internship at Utkarsh Enterprises
- **Sheets**: `Lead`, `Order`
- **Simulated Churn**: Leads not in Order sheet = Churned
- **Key Features**: State, Salesperson, Quantity, Start Date, Lead Age

## 📈 Exploratory Data Analysis (EDA)

Visualizations created:
- 📍 **Churn Rate by State** – Compare churn across regions
- 🧑‍💼 **Churn by Salesperson** – Performance comparison of sales reps
- ⏳ **Lead Age vs Churn Probability** – Time-based churn trends
- 🔄 **Lead Progression by Stage** – Overview of sales funnel stages


## 🏗️ Feature Engineering

- Extracted month, day, and weekday from engagement date
- Encoded `STATE`, `Salesperson`, `CLIENT NAME`
- Removed unnecessary columns (e.g., raw dates, IDs)

## 🤖 Model Used

- **Model**: `RandomForestClassifier` (Scikit-learn)
- **Why**: Handles categorical and numeric data, robust, interpretable
- **Performance**: ~86% accuracy on test set
- **Evaluation**: Confusion Matrix, Precision, Recall, F1-score

## 🔍 Feature Importance Insights

Top features influencing churn:
- `STATE` – Regional effect on conversion
- `Salesperson` – Individual performance
- `start_weekday` – Engagement timing
- `QUANTITY` – Larger orders converted better

## 💼 Business Impact

✅ Improved lead prioritization  
✅ Identified sales bottlenecks by region and rep  
✅ Informed strategy for follow-up timing  
✅ Real-world value delivered to sales team during internship

## 🚀 Tools & Libraries

- Python, Pandas, NumPy
- Seaborn, Matplotlib
- Scikit-learn (Random Forest Classifier)
- Jupyter Notebook


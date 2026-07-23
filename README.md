# 📊 Customer Churn Prediction using RFM Analysis & Machine Learning



## 📌 Project Overview

This project analyzes customer transaction data from an online retail company to understand purchasing behavior, identify valuable customer segments, and predict customers who are likely to stop buying from the business.

Using **Exploratory Data Analysis (EDA)**, **RFM Segmentation**, and **Machine Learning**, the project provides actionable business insights that help improve customer retention, increase revenue, and strengthen long-term customer relationships.

---

# ⭐ STAR Methodology

## 🟢 Situation

Customer retention is one of the biggest challenges in the retail industry. Although businesses collect large volumes of customer transaction data, they often struggle to identify customers who are likely to churn before they stop purchasing.

Without early identification, businesses lose valuable customers, resulting in reduced revenue and increased customer acquisition costs.

The project uses the **Online Retail Transaction Dataset**, which contains:

- Invoice Number
- Product Description
- Quantity Purchased
- Unit Price
- Purchase Date
- Customer ID
- Customer Country

The goal was to analyze customer purchasing behavior and develop a predictive model that identifies customers at risk of churn.

---

## 🎯 Task

The objectives of this project were to:

- Perform Exploratory Data Analysis (EDA) to understand customer purchasing behavior.
- Identify revenue patterns and seasonal sales trends.
- Segment customers using RFM Analysis.
- Build predictive machine learning models for customer churn prediction.
- Evaluate model performance using classification metrics.
- Generate business recommendations to improve customer retention.

---

## ⚙️ Action

### Data Preparation

- Cleaned missing and invalid transaction records.
- Converted transaction dates into datetime format.
- Calculated Total Revenue.
- Engineered customer-level features.
- Prepared RFM metrics.

---

### Exploratory Data Analysis (EDA)

Performed detailed analysis on:

- Revenue Distribution
- Monthly Revenue Trends
- Geographic Sales Distribution
- Customer Purchase Frequency
- Customer Revenue Contribution
- Customer Segmentation

---

## 🔍 Top 5 EDA Findings

### 1️⃣ Revenue Concentration Among a Small Group of Customers

### Observation

A relatively small percentage of customers generated the majority of total revenue.

### Business Takeaway

- Prioritize high-value customer retention.
- Introduce loyalty rewards.
- Offer exclusive promotions.
- Personalize customer experiences.

---

### 2️⃣ Seasonal Revenue Trends

### Observation

Monthly revenue fluctuated significantly, with certain months generating considerably higher sales.

### Business Takeaway

- Schedule marketing campaigns during low-performing months.
- Optimize inventory planning.
- Improve promotional timing.

---

### 3️⃣ Geographic Revenue Concentration

### Observation

Only a few countries contributed the majority of total revenue.

### Business Takeaway

- Increase investment in top-performing regions.
- Explore growth opportunities in underperforming markets.

---

### 4️⃣ Customer Purchase Frequency

### Observation

Most customers made only a few purchases, while a smaller group purchased frequently.

### Business Takeaway

- Encourage repeat purchases.
- Implement customer loyalty programs.
- Recommend personalized products.

---

### 5️⃣ RFM Customer Segmentation

### Observation

Customers were segmented into:

- 🏆 Champions
- ❤️ Loyal Customers
- ⚠️ At Risk Customers
- ❌ Lost Customers

### Business Takeaway

Each customer segment requires different marketing strategies.

Examples include:

- Rewards for Champions
- Loyalty benefits for Loyal Customers
- Re-engagement campaigns for At Risk Customers
- Win-back offers for Lost Customers

---

## 🤖 Machine Learning Models

Two supervised machine learning models were developed for customer churn prediction.

### Models Used

- Logistic Regression
- Random Forest Classifier

Dataset Split

- Training Data: **80%**
- Testing Data: **20%**

---

## 📊 Model Evaluation Metrics

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC Score

Special emphasis was placed on **F1 Score** and **ROC-AUC** because these metrics provide a balanced evaluation for identifying churned customers while minimizing false predictions.

---

## 🏆 Result

Among the two models,

### ✅ Random Forest achieved the best overall performance.

It provided:

- Higher Accuracy
- Better Precision
- Higher Recall
- Improved F1 Score
- Better ROC-AUC Score

The model successfully identified customers who are most likely to churn, enabling businesses to take proactive retention actions.

---

# 📈 Business Recommendations

## 1️⃣ Implement Targeted Customer Retention Campaigns

Customers predicted to be at risk of churn should receive:

- Personalized Emails
- Discount Coupons
- Reminder Notifications
- Re-engagement Campaigns

---

## 2️⃣ Strengthen Loyalty Programs

Reward high-value customers with:

- Exclusive Deals
- Loyalty Rewards
- Early Product Access
- VIP Membership Benefits

---

## 3️⃣ Optimize Marketing & Product Strategy

Use purchasing behavior insights to:

- Recommend Products
- Bundle Frequently Purchased Items
- Improve Cross-selling
- Increase Average Order Value

---

# 📌 Business Impact

This project demonstrates how combining customer analytics with predictive machine learning enables organizations to:

- Improve customer retention
- Increase customer lifetime value
- Reduce churn
- Enhance marketing effectiveness
- Support data-driven business decisions
- Increase long-term revenue

---

# 🛠️ Tech Stack

**Programming Language**

- R

**Libraries**

- dplyr
- tidyr
- ggplot2
- caret
- randomForest
- e1071
- corrplot

**Machine Learning**

- Logistic Regression
- Random Forest

**IDE**

- RStudio

---

# 📂 Project Workflow

```
Business Problem
        │
        ▼
Data Collection
        │
        ▼
Data Cleaning
        │
        ▼
Feature Engineering
        │
        ▼
Exploratory Data Analysis
        │
        ▼
RFM Analysis
        │
        ▼
Machine Learning
(Logistic Regression & Random Forest)
        │
        ▼
Model Evaluation
        │
        ▼
Business Insights
        │
        ▼
Business Recommendations
```

---

# 📊 Key Skills Demonstrated

- Business Analytics
- Customer Analytics
- Exploratory Data Analysis
- Customer Segmentation
- RFM Analysis
- Machine Learning
- Predictive Analytics
- Customer Churn Prediction
- Data Visualization
- Business Intelligence
- Statistical Analysis
- Customer Retention Strategy

---

# 📁 Repository Structure

```
Customer-Churn-Prediction/
│
├── data/
│     └── Online Retail Dataset
│
├── notebooks/
│     └── Customer_Churn_Prediction.ipynb
│
├── outputs/
│     ├── EDA Charts
│     ├── RFM Analysis
│     ├── Model Evaluation
│     └── Business Insights
│
├── README.md
│
└── requirements.txt
```

---

# 🚀 Future Improvements

- Deploy the model using Streamlit or Shiny.
- Create an interactive Power BI Dashboard.
- Build real-time customer churn prediction.
- Integrate automated customer recommendation systems.
- Improve model performance using XGBoost and LightGBM.

---

# 👨‍💻 Author

**Harendra**

MBA (Business Analytics)

📊 Data Analytics | Business Analytics | Machine Learning | Business Intelligence

---

## ⭐ Support

If you found this project helpful, please consider giving this repository a **⭐ Star**.

It helps others discover the project and motivates future improvements.

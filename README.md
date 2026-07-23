📌 Project Overview

⭐ Situation

Customer retention is a major challenge for online retail businesses. Although companies collect large volumes of transaction data, they often struggle to identify customers who are likely to stop purchasing.

This project analyzes the Online Retail Transaction Dataset to understand purchasing behavior, discover customer segments, and build a predictive machine learning model that identifies customers at risk of churn.

🎯 Task

The primary objectives were to:

Analyze customer purchasing patterns using Exploratory Data Analysis (EDA)

Identify high-value customer segments using RFM Analysis

Engineer behavioral features for churn prediction

Build and evaluate Machine Learning models

Generate actionable business recommendations for improving customer retention and revenue

⚙️ Action

📊 Data Preparation

Cleaned missing and duplicate records

Removed cancelled transactions and invalid values

Created new business metrics including:

Revenue

Recency

Frequency

Monetary Value (RFM)

Engineered customer-level features for modeling

📈 Exploratory Data Analysis (EDA)

Performed detailed analysis to understand customer behavior and revenue trends.

Key Insights

1️⃣ Revenue Concentration

A small percentage of customers generated the majority of total revenue.

Business Insight

Focus retention efforts on high-value customers through loyalty rewards and personalized offers.

2️⃣ Seasonal Revenue Trends

Monthly sales fluctuated significantly with clear peak purchasing periods.

Business Insight

Schedule promotional campaigns during low-performing months to stabilize revenue.

3️⃣ Geographic Revenue Distribution

Most revenue originated from a limited number of countries.

Business Insight

Increase investment in high-performing markets while exploring growth opportunities in emerging regions.

4️⃣ Customer Purchase Frequency

Most customers purchased only a few times.

A smaller segment demonstrated strong repeat purchasing behavior.

Business Insight

Encourage repeat purchases using recommendation systems and loyalty programs.

5️⃣ Customer Segmentation (RFM Analysis)

Customers were segmented into:

🏆 Champions

❤️ Loyal Customers

⚠️ At Risk

❌ Lost Customers

Business Insight

Design targeted marketing campaigns for each customer segment instead of applying one generic strategy.

🤖 Machine Learning

Two classification models were developed to predict customer churn.

Models Used

Logistic Regression

Random Forest Classifier

Data Split

Training Data: 80%

Testing Data: 20%

Evaluation Metrics

Accuracy

Precision

Recall

F1 Score

ROC-AUC Score

📊 Model Performance

Among the two models, Random Forest achieved the best overall performance.

It demonstrated:

Higher predictive accuracy

Better F1 Score

Stronger ROC-AUC performance

Improved capability to correctly identify churned customers while minimizing false predictions

📈 Business Recommendations

🎯 1. Target At-Risk Customers

Send personalized offers

Email reminders

Discount campaigns

Win-back promotions

🌟 2. Strengthen Loyalty Programs

Reward high-value customers through:

Exclusive discounts

Early product access

Reward points

VIP membership benefits

🛒 3. Improve Product & Marketing Strategy

Use purchasing behavior to:

Recommend relevant products

Bundle frequently purchased items

Personalize product suggestions

Increase Average Order Value (AOV)

🛠️ Tech Stack

Python

Pandas

NumPy

Matplotlib

Seaborn

Scikit-learn

Jupyter Notebook

✅ Result

The project successfully combined customer behavior analytics, RFM segmentation, and machine learning to predict customer churn and generate actionable business insights.

Business Impact

Improved customer retention strategy

Identified high-value customer segments

Enabled personalized marketing

Supported data-driven decision making

Increased opportunities for revenue growth through proactive customer engagement
